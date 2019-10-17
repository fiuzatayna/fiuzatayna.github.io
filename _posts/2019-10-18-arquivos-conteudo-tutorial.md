---
layout: post
title: "Conteúdo do Tutorial"
date: 2019-10-18
---

Well. Finally got around to putting this old website together. Neat thing about it - powered by [Jekyll](http://jekyllrb.com) and I can use Markdown to author my posts. It actually is a lot easier than I thought it was going to be.

O que acontece se eu inserir HTML aqui?


**index.html [1]**
---
<pre class="prettyprint pre-scrollable"><code>&lt;!DOCTYPE html&gt;
&lt;html&gt;
	&lt;head&gt;
		&lt;title&gt;Hank Quinlan, Horrible Cop&lt;/title&gt;
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
        		&lt;h1&gt;Hi there, I'm Hank Quinlan!&lt;/h1&gt;
				&lt;p&gt;I'm best known as the horrible cop from &lt;em&gt;A Touch of Evil&lt;/em&gt; Don't trust me. &lt;a href="/about"&gt;Read more about my life...&lt;/a&gt;&lt;/p&gt;
    		&lt;/div&gt;&lt;!-- /.blurb --&gt;
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

**main.css [1]**
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
		&lt;title&gt;Hank Quinlan, Horrible Cop&lt;/title&gt;
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
        		&lt;h1&gt;Hi there, I'm Hank Quinlan!&lt;/h1&gt;
				&lt;p&gt;I'm best known as the horrible cop from &lt;em&gt;A Touch of Evil&lt;/em&gt; Don't trust me. &lt;a href="/about"&gt;Read more about my life...&lt;/a&gt;&lt;/p&gt;
    		&lt;/div&gt;&lt;!-- /.blurb --&gt;
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

**default.html [1]**
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
	&lt;h1&gt;Hi there, I'm Hank Quinlan!&lt;/h1&gt;
	&lt;p&gt;I'm best known as the horrible cop from &lt;em&gt;A Touch of Evil&lt;/em&gt; Don't trust me. &lt;a href="/about"&gt;Read more about my life...&lt;/a&gt;&lt;/p&gt;
&lt;/div&gt;&lt;!-- /.blurb --&gt;</code></pre>
---
