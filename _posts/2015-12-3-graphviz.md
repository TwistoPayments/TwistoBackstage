---
layout: post
title: Graphviz pro vizualizaci dat
---

Graphviz je open source nástroj na vizualizaci dat pomocí grafů/diagramů. My jej používáme např. pro vizualizaci vztahů mezi zákazníky.

<a href="/images/graphviz-post/full-chart.png"><img src="/images/graphviz-post/demo-chart.png"></a>

Na tomto konkrétním grafu každý uzel představuje jedno konkrétní vyhodnocení (pokus o nákup) a hrany zobrazují vztahy mezi jednotlivými pokusy o nákup, tj. na základě kterých informací jsme vyhodnotili, že se jedná o stejného zákazníka. V praxi mají hrany samozřejmě přesné popisky jako např. e-mail, nebo session, na ukázce je vše z pochopitelných důvodů anonymizováno.

Výhodou je, že grafy jsou popsané pouze jednoduchým textovým jazykem a nemusíte tak nic “kreslit”. Samozřejmě je možnost změnit výsledný vzhled výstupu, ale např. při přidání uzlu se Graphviz sám postará o to, aby výsledek vypadal dobře a žádné popisky se nepřekrývaly.

Navíc jako výstup podporuje SVG a další vektorové i bitmapové výstupy, takže není problém s integrací výstupu v podstatě kamkoliv. Při použití SVG výstupu je navíc možné vkládat HTML kód, což používáme pro odkazy do administrace při kliknutí na konkrétní vyhodnocení.

Ukázka zápisu diagramu:

```
// The Round Table

digraph {
    A [label="King Arthur"]
    B [label="Sir Bedevere the Wise"]
    L [label="Sir Lancelot the Brave"]
        A -> B
        A -> L
        B -> L [constraint=false]
}
```

![_config.yml]({{ site.baseurl }}/images/graphviz-post/simple-chart.png)

Náš ukázkový graf je hodně jednoduchý, takže používáme pouze textovou šablonu, ale k dispozici je i Python knihovna, která usnadňuje (a trochu i zpřehledňuje) zápis. Stejný graf jako je nahoře se potom může generovat např. takto:

```python
>>> from graphviz import Digraph
>>> dot = Digraph(comment='The Round Table')
>>> dot
<graphviz.dot.Digraph object at 0x...>

>>> dot.node('A', 'King Arthur')
>>> dot.node('B', 'Sir Bedevere the Wise')
>>> dot.node('L', 'Sir Lancelot the Brave')

>>> dot.edges(['AB', 'AL'])
>>> dot.edge('B', 'L', constraint='false')
```

Pokud vás zajímá víc detailů, podívejte se např. na úvod do Graphvizu zde:
[http://matthiaseisen.com/articles/graphviz/](http://matthiaseisen.com/articles/graphviz/)
