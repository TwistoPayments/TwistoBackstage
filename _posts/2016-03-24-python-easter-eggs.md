---
layout: post
title: Easter eggs v pythonu
---

Velikonoce se nám blíží, vybrali jsme proto pár Easter eggů schovaných v pythonu. Vyzkoušejte si je. :-)

<style>
td.linenos { background-color: #f0f0f0; padding-right: 10px; }
span.lineno { background-color: #f0f0f0; padding: 0 5px 0 5px; }
pre { line-height: 125%; }
body .hll { background-color: #ffffcc }
body  { background: #f8f8f8; }
body .c { color: #408080; font-style: italic } /* Comment */
body .err { border: 1px solid #FF0000 } /* Error */
body .k { color: #008000; font-weight: bold } /* Keyword */
body .o { color: #666666 } /* Operator */
body .cm { color: #408080; font-style: italic } /* Comment.Multiline */
body .cp { color: #BC7A00 } /* Comment.Preproc */
body .c1 { color: #408080; font-style: italic } /* Comment.Single */
body .cs { color: #408080; font-style: italic } /* Comment.Special */
body .gd { color: #A00000 } /* Generic.Deleted */
body .ge { font-style: italic } /* Generic.Emph */
body .gr { color: #FF0000 } /* Generic.Error */
body .gh { color: #000080; font-weight: bold } /* Generic.Heading */
body .gi { color: #00A000 } /* Generic.Inserted */
body .go { color: #888888 } /* Generic.Output */
body .gp { color: #000080; font-weight: bold } /* Generic.Prompt */
body .gs { font-weight: bold } /* Generic.Strong */
body .gu { color: #800080; font-weight: bold } /* Generic.Subheading */
body .gt { color: #0044DD } /* Generic.Traceback */
body .kc { color: #008000; font-weight: bold } /* Keyword.Constant */
body .kd { color: #008000; font-weight: bold } /* Keyword.Declaration */
body .kn { color: #008000; font-weight: bold } /* Keyword.Namespace */
body .kp { color: #008000 } /* Keyword.Pseudo */
body .kr { color: #008000; font-weight: bold } /* Keyword.Reserved */
body .kt { color: #B00040 } /* Keyword.Type */
body .m { color: #666666 } /* Literal.Number */
body .s { color: #BA2121 } /* Literal.String */
body .na { color: #7D9029 } /* Name.Attribute */
body .nb { color: #008000 } /* Name.Builtin */
body .nc { color: #0000FF; font-weight: bold } /* Name.Class */
body .no { color: #880000 } /* Name.Constant */
body .nd { color: #AA22FF } /* Name.Decorator */
body .ni { color: #999999; font-weight: bold } /* Name.Entity */
body .ne { color: #D2413A; font-weight: bold } /* Name.Exception */
body .nf { color: #0000FF } /* Name.Function */
body .nl { color: #A0A000 } /* Name.Label */
body .nn { color: #0000FF; font-weight: bold } /* Name.Namespace */
body .nt { color: #008000; font-weight: bold } /* Name.Tag */
body .nv { color: #19177C } /* Name.Variable */
body .ow { color: #AA22FF; font-weight: bold } /* Operator.Word */
body .w { color: #bbbbbb } /* Text.Whitespace */
body .mb { color: #666666 } /* Literal.Number.Bin */
body .mf { color: #666666 } /* Literal.Number.Float */
body .mh { color: #666666 } /* Literal.Number.Hex */
body .mi { color: #666666 } /* Literal.Number.Integer */
body .mo { color: #666666 } /* Literal.Number.Oct */
body .sb { color: #BA2121 } /* Literal.String.Backtick */
body .sc { color: #BA2121 } /* Literal.String.Char */
body .sd { color: #BA2121; font-style: italic } /* Literal.String.Doc */
body .s2 { color: #BA2121 } /* Literal.String.Double */
body .se { color: #BB6622; font-weight: bold } /* Literal.String.Escape */
body .sh { color: #BA2121 } /* Literal.String.Heredoc */
body .si { color: #BB6688; font-weight: bold } /* Literal.String.Interpol */
body .sx { color: #008000 } /* Literal.String.Other */
body .sr { color: #BB6688 } /* Literal.String.Regex */
body .s1 { color: #BA2121 } /* Literal.String.Single */
body .ss { color: #19177C } /* Literal.String.Symbol */
body .bp { color: #008000 } /* Name.Builtin.Pseudo */
body .vc { color: #19177C } /* Name.Variable.Class */
body .vg { color: #19177C } /* Name.Variable.Global */
body .vi { color: #19177C } /* Name.Variable.Instance */
body .il { color: #666666 } /* Literal.Number.Integer.Long */

</style>

<div class="highlight"><pre><span class="gp">&gt;&gt;&gt; </span><span class="kn">from</span> <span class="nn">__future__</span> <span class="kn">import</span> <span class="n">braces</span>
  File <span class="nb">&quot;&lt;stdin&gt;&quot;</span>, line <span class="m">1</span>
<span class="gr">SyntaxError</span>: <span class="n">not a chance</span>


<span class="gp">&gt;&gt;&gt; </span><span class="kn">import</span> <span class="nn">this</span>
<span class="go">The Zen of Python, by Tim Peters</span>

<span class="go">Beautiful is better than ugly.</span>
<span class="go">Explicit is better than implicit.</span>
<span class="go">Simple is better than complex.</span>
<span class="go">Complex is better than complicated.</span>
<span class="go">Flat is better than nested.</span>
<span class="go">Sparse is better than dense.</span>
<span class="go">Readability counts.</span>
<span class="go">Special cases aren&#39;t special enough to break the rules.</span>
<span class="go">Although practicality beats purity.</span>
<span class="go">Errors should never pass silently.</span>
<span class="go">Unless explicitly silenced.</span>
<span class="go">In the face of ambiguity, refuse the temptation to guess.</span>
<span class="go">There should be one-- and preferably only one --obvious way to do it.</span>
<span class="go">Although that way may not be obvious at first unless you&#39;re Dutch.</span>
<span class="go">Now is better than never.</span>
<span class="go">Although never is often better than *right* now.</span>
<span class="go">If the implementation is hard to explain, it&#39;s a bad idea.</span>
<span class="go">If the implementation is easy to explain, it may be a good idea.</span>
<span class="go">Namespaces are one honking great idea -- let&#39;s do more of those!</span>


<span class="gp">&gt;&gt;&gt; </span><span class="kn">import</span> <span class="nn">__hello__</span>
<span class="go">Hello world...</span>


<span class="gp">&gt;&gt;&gt; </span><span class="kn">import</span> <span class="nn">antigravity</span>
<span class="go"># Opens this URL in you browser: http://xkcd.com/353/</span>


<span class="gp">&gt;&gt;&gt; </span><span class="n">love</span><span class="o">=</span><span class="n">this</span>
<span class="gp">&gt;&gt;&gt; </span><span class="n">this</span> <span class="ow">is</span> <span class="n">love</span>
<span class="go">True</span>
<span class="gp">&gt;&gt;&gt; </span><span class="n">love</span> <span class="ow">is</span> <span class="bp">True</span>
<span class="go">False</span>
<span class="gp">&gt;&gt;&gt; </span>
<span class="gp">&gt;&gt;&gt; </span><span class="n">love</span> <span class="ow">is</span> <span class="bp">False</span>
<span class="go">False</span>
<span class="gp">&gt;&gt;&gt; </span>
<span class="gp">&gt;&gt;&gt; </span><span class="n">love</span> <span class="ow">is</span> <span class="ow">not</span> <span class="bp">True</span> <span class="ow">or</span> <span class="bp">False</span><span class="p">;</span> <span class="n">love</span> <span class="ow">is</span> <span class="n">love</span>
<span class="go">True</span>
<span class="go">True</span>
<span class="go">&gt;&gt;&gt;</span>
</pre></div>
