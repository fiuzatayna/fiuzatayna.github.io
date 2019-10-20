---
layout: post
title: "Conteúdo do Tutorial"
date: 2019-10-18
---

Aqui estão os conteúdos que devem ser inseridos em diferentes arquivos ao longo do tutorial. 

---

**index.html [1]**
---
<pre class="prettyprint pre-scrollable"><code>&lt;!DOCTYPE html&gt;
&lt;html&gt;
	&lt;head&gt;
		&lt;title&gt;[Seu Nome], primeiro site&lt;/title&gt;
	&lt;/head&gt;
	&lt;body&gt;
		&lt;nav&gt;
    		&lt;ul&gt;
        		&lt;li&gt;&lt;a href="/"&gt;Home&lt;/a&gt;&lt;/li&gt;
	        	&lt;li&gt;&lt;a href="/about"&gt;About&lt;/a&gt;&lt;/li&gt;
        		&lt;li&gt;&lt;a href="/cv"&gt;CV&lt;/a&gt;&lt;/li&gt;
        		&lt;li&gt;&lt;a href="/blog"&gt;Blog&lt;/a&gt;&lt;/li&gt;
    		&lt;/ul&gt;
		&lt;/nav&gt;
		&lt;div class="container"&gt;
    		&lt;div class="blurb"&gt;
        		&lt;h1&gt;Oi, eu sou [Seu Nome]!&lt;/h1&gt;
				&lt;p&gt;Estou criando essa página como parte de um tutorial da disciplina de &lt;em&gt;Geração de Aplicativos em Bioinformática;/em&gt; Saiba mais sobre mim &lt;a href="/about"&gt;aqui&lt;/a&gt;&lt;/p&gt;
    		&lt;/div&gt;&lt;!-- /.blurb --&gt;
		&lt;/div&gt;&lt;!-- /.container --&gt;
		&lt;footer&gt;
    		&lt;ul&gt;
        		&lt;li&gt;&lt;a href="mailto:seuemail@gmail.com"&gt;email&lt;/a&gt;&lt;/li&gt;
        		&lt;li&gt;&lt;a href="https://github.com/seugithub"&gt;github.com/seugithub&lt;/a&gt;&lt;/li&gt;
			&lt;/ul&gt;
		&lt;/footer&gt;
	&lt;/body&gt;
&lt;/html&gt;</code></pre>
---

**css/main.css [1]**
---
<pre class="prettyprint pre-scrollable">
body &lbrace;
    margin: 60px auto;
    width: 70%;
&rbrace;
nav ul, footer ul &lbrace;
    font-family:'Helvetica', 'Arial', 'Sans-Serif';
    padding: 0px;
    list-style: none;
    font-weight: bold;
&rbrace;
nav ul li, footer ul li &lbrace;
    display: inline;
    margin-right: 20px;
&rbrace;
a &lbrace;
    text-decoration: none;
    color: #999;
&rbrace;
a:hover &lbrace;
    text-decoration: underline;
&rbrace;
h1 &lbrace;
    font-size: 3em;
    font-family:'Helvetica', 'Arial', 'Sans-Serif';
&rbrace;
p &lbrace;
    font-size: 1.5em;
    line-height: 1.4em;
    color: #333;
&rbrace;
footer &lbrace;
    border-top: 1px solid #d5d5d5;
    font-size: .8em;
&rbrace;

ul.posts &lbrace; 
    margin: 20px auto 40px; 
    font-size: 1.5em;
&rbrace;

ul.posts li &lbrace;
    list-style: none;
&rbrace;
</pre>

---

**index.html [2]**
---
<pre class="prettyprint pre-scrollable"><code>&lt;!DOCTYPE html&gt;
&lt;html&gt;
	&lt;head&gt;
		&lt;title&gt;[Seu Nome], primeiro site&lt;/title&gt;
		<strong>&lt;!-- link to main stylesheet --&gt;</strong>
		<strong>&lt;link rel="stylesheet" type="text/css" href="/css/main.css"&gt;</strong>
	&lt;/head&gt;
	&lt;body&gt;
		&lt;nav&gt;
    		&lt;ul&gt;
        		&lt;li&gt;&lt;a href="/"&gt;Home&lt;/a&gt;&lt;/li&gt;
	        	&lt;li&gt;&lt;a href="/about"&gt;About&lt;/a&gt;&lt;/li&gt;
        		&lt;li&gt;&lt;a href="/cv"&gt;CV&lt;/a&gt;&lt;/li&gt;
        		&lt;li&gt;&lt;a href="/blog"&gt;Blog&lt;/a&gt;&lt;/li&gt;
    		&lt;/ul&gt;
		&lt;/nav&gt;
		&lt;div class="container"&gt;
    		&lt;div class="blurb"&gt;
        		&lt;h1&gt;Oi, eu sou [Seu Nome]!&lt;/h1&gt;
				&lt;p&gt;Estou criando essa página como parte de um tutorial da disciplina de &lt;em&gt;Geração de Aplicativos em Bioinformática;/em&gt; Saiba mais sobre mim &lt;a href="/about"&gt;aqui&lt;/a&gt;&lt;/p&gt;
    		&lt;/div&gt;&lt;!-- /.blurb --&gt;
		&lt;/div&gt;&lt;!-- /.container --&gt;
		&lt;footer&gt;
    		&lt;ul&gt;
        		&lt;li&gt;&lt;a href="mailto:seuemail@gmail.com"&gt;email&lt;/a&gt;&lt;/li&gt;
        		&lt;li&gt;&lt;a href="https://github.com/seugithub"&gt;github.com/seugithub&lt;/a&gt;&lt;/li&gt;
			&lt;/ul&gt;
		&lt;/footer&gt;
	&lt;/body&gt;
&lt;/html&gt;</code></pre>
---

**_layouts/default.html [1]**
---
<pre class="prettyprint pre-scrollable"><code>&lt;!DOCTYPE html&gt;
	&lt;html&gt;
		&lt;head&gt;
			&lt;title&gt;&lbrace;&lbrace; page.title &rbrace;&rbrace;&lt;/title&gt;
			&lt;!-- link to main stylesheet --&gt;
			&lt;link rel="stylesheet" type="text/css" href="/css/main.css"&gt;
		&lt;/head&gt;
		&lt;body&gt;
			&lt;nav&gt;
	    		&lt;ul&gt;
	        		&lt;li&gt;&lt;a href="/"&gt;Home&lt;/a&gt;&lt;/li&gt;
		        	&lt;li&gt;&lt;a href="/about"&gt;About&lt;/a&gt;&lt;/li&gt;
	        		&lt;li&gt;&lt;a href="/cv"&gt;CV&lt;/a&gt;&lt;/li&gt;
	        		&lt;li&gt;&lt;a href="/blog"&gt;Blog&lt;/a&gt;&lt;/li&gt;
	    		&lt;/ul&gt;
			&lt;/nav&gt;
			&lt;div class="container"&gt;
			
			&lbrace;&lbrace; content &rbrace;&rbrace;
			
			&lt;/div&gt;&lt;!-- /.container --&gt;
			&lt;footer&gt;
	    		&lt;ul&gt;
	        		&lt;li&gt;&lt;a href="mailto:hankquinlanhub@gmail.com"&gt;email&lt;/a&gt;&lt;/li&gt;
	        		&lt;li&gt;&lt;a href="https://github.com/hankquinlan"&gt;github.com/hankquinlan&lt;/a&gt;&lt;/li&gt;
				&lt;/ul&gt;
			&lt;/footer&gt;
		&lt;/body&gt;
	&lt;/html&gt;</code></pre>
---

**index.html [3]**
---
<pre class="prettyprint pre-scrollable"><code>---
layout: default
title: Hank Quinlan, Horrible Cop
---
&lt;div class="blurb"&gt;
    &lt;h1&gt;Oi, eu sou [Seu Nome]!&lt;/h1&gt;
            &lt;p&gt;Estou criando essa página como parte de um tutorial da disciplina de &lt;em&gt;Geração de Aplicativos em Bioinformática;/em&gt; Saiba mais sobre mim &lt;a href="/about"&gt;aqui&lt;/a&gt;&lt;/p&gt;

&lt;/div&gt;&lt;!-- /.blurb --&gt;</code></pre>
---


**_layouts/post.html [1]**
---
<pre class="prettyprint pre-scrollable"><code>---
layout: default
---
&lt;h1&gt;&lbrace;&lbrace; page.title &rbrace;&rbrace;&lt;/h1&gt;
&lt;p class="meta"&gt;&lbrace;&lbrace; page.date | date_to_string &rbrace;&rbrace;&lt;/p&gt;

&lt;div class="post"&gt;
  &lbrace;&lbrace; content &rbrace;&rbrace;
&lt;/div&gt;</code></pre>
---

**_posts/2019-10-21-hank-quinlan-site-launched.md**
---
<pre class="prettyprint pre-scrollable"><code>---
layout: post
title: "[Seu Nome] lança site"
date: 2019-10-21
---

Aqui estamos, esse é meu primeiro post no blog do site que criei nesse tutorial do GitHub. 
</code></pre>
---

**blog/index.html**
---
<pre class="prettyprint pre-scrollable"><code>---
layout: default
title: Blog de [Seu Nome]
---
	&lt;h1&gt;&lbrace;&lbrace; page.title &rbrace;&rbrace;&lt;/h1&gt;
	&lt;ul class="posts"&gt;

	  &lbrace;&percnt; for post in site.posts &percnt;&rbrace;
	    &lt;li&gt;&lt;span&gt;&lbrace;&lbrace; post.date | date_to_string &rbrace;&rbrace;&lt;/span&gt; &raquo; &lt;a href="&lbrace;&lbrace; post.url &rbrace;&rbrace;" title="&lbrace;&lbrace; post.title &rbrace;&rbrace;">&lbrace;&lbrace; post.title &rbrace;&rbrace;&lt;/a&gt;&lt;/li&gt;
	  &lbrace;&percnt; endfor &percnt;&rbrace;
	&lt;/ul&gt;</code></pre>
---
