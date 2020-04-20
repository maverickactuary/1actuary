---
layout: default
folder: /content/5resources/
title: Transformaction
---

## Inline HTML elements

HTML defines a long list of available inline tags, a complete list of which can be found on the [Mozilla Developer Network](https://developer.mozilla.org/en-US/docs/Web/HTML/Element).

<ul>
  <li><strong>To bold text</strong>, use <code>&lt;strong&gt;</code>.</li>
  <li><em>To italicize text</em>, use <code>&lt;em&gt;</code>.</li>
  <li>Abbreviations, like <abbr title="HyperText Markup Langage">HTML</abbr> should use <code>&lt;abbr&gt;</code>, with an optional <code>title</code> attribute for the full phrase.</li>
  <li>Citations, like <cite>&mdash; Mark otto</cite>, should use <code>&lt;cite&gt;</code>.</li>
  <li><del>Deleted</del> text should use <code>&lt;del&gt;</code> and <ins>inserted</ins> text should use <code>&lt;ins&gt;</code>.</li>
  <li>Superscript <sup>text</sup> uses <code>&lt;sup&gt;</code> and subscript <sub>text</sub> uses <code>&lt;sub&gt;</code>.</li>
</ul>

Most of these elements are styled by browsers with few modifications on our part.

## Heading

### Code

<pre><code>// Example can be run directly in your JavaScript console
// Create a function that takes two arguments and returns the sum of those arguments
var adder = new Function(&quot;a&quot;, &quot;b&quot;, &quot;return a + b&quot;);

// Call the function
adder(2, 6);
// &gt; 8</code></pre>

### Lists

+ Praesent commodo cursus magna, vel scelerisque nisl consectetur et.
+ Donec id elit non mi porta gravida at eget metus.
+ Nulla vitae elit libero, a pharetra augue.

1. Vestibulum id ligula porta felis euismod semper.
1. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.
1. Maecenas sed diam eget risus varius blandit sit amet non magna.

<dl>
  <dt>HyperText Markup Language (HTML)</dt>
    <dd>The language used to describe and define the content of a Web page</dd>
  <dt>Cascading Style Sheets (CSS)</dt>
    <dd>Used to describe the appearance of Web content</dd>
  <dt>JavaScript (JS)</dt>
    <dd>The programming language used to build advanced Web sites and applications</dd>
</dl>

### Images

<img src="https://placehold.it/800x400" alt="placeholder" title="Large example image">
<img src="https://placehold.it/400x200" alt="placeholder" title="Medium example image">
<img src="https://placehold.it/200x200" alt="placeholder" title="Small example image">

### Tables

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Upvotes</th>
      <th>Downvotes</th>
    </tr>
  </thead>
  <tfoot>
    <tr>
      <td>Totals</td>
      <td>21</td>
      <td>23</td>
    </tr>
  </tfoot>
  <tbody>
    <tr>
      <td>Alice</td>
      <td>10</td>
      <td>11</td>
    </tr>
    <tr>
      <td>Bob</td>
      <td>4</td>
      <td>3</td>
    </tr>
    <tr>
      <td>Charlie</td>
      <td>7</td>
      <td>9</td>
    </tr>
  </tbody>
</table>

### Blockquote

<blockquote>
Jekyll is a simple, blog aware, static site generator. It takes a template directory [...] and spits out a complete, static website suitable for serving with Apache or your favorite web server. This is also the engine behind GitHub Pages, which you can use to host your project’s page or blog right here from GitHub.
</blockquote>
