---
layout: post
title: Example content
---


<div class="message">
  This is a dummy post to just test the various features provided on this theme. This will also serve as a quick lookup for any mark down option that I'll be needing ;)
</div>

<!--more-->
Here is a <a href="#">link</a>, and a word in *italics*

> Hello quoted text

Now that was a **bold** move. Some vicious HTML managed to `<h1>Escape</h1>`. And that is how you get plain texts even in markdown.

## Inline HTML elements

HTML defines a long list of available inline tags, a complete list of which can be found on the [Mozilla Developer Network](https://developer.mozilla.org/en-US/docs/Web/HTML/Element).

- **To bold text**, use `<strong>`.
- *To italicize text*, use `<em>`.
- Abbreviations, like <abbr title="HyperText Markup Langage">HTML</abbr> should use `<abbr>`, with an optional `title` attribute for the full phrase.
- Citations, like <cite>&mdash; Mark otto</cite>, should use `<cite>`.
- <del>Deleted</del> text should use `<del>` and <ins>inserted</ins> text should use `<ins>`.
- Superscript <sup>text</sup> uses `<sup>` and subscript <sub>text</sub> uses `<sub>`.

Most of these elements are styled by browsers with few modifications on our part.


## Heading
Some more random text under a heading with 2 #'s.

### Code
because JavaScript.

{% highlight js %}
// Example can be run directly in your JavaScript console

// Create a function that takes two arguments and returns the sum of those arguments
var adder = new Function("a", "b", "return a + b");

// Call the function
adder(2, 6);
// > 8
{% endhighlight %}



### Lists

A list of lists.

Lets start off!

* blah
* bleh
* bluh

Now for some *law* and **order**

1. Foo
2. Bar
3. `Thunk calls`

Lists and their indentation - let's use some `<dl>, <dt> and <dd>`

<dl>
  <dt>HyperText Markup Language (HTML)</dt>
  <dd>The language used to describe and define the content of a Web page</dd>

  <dt>Cascading Style Sheets (CSS)</dt>
  <dd>Used to describe the appearance of Web content</dd>

  <dt>JavaScript (JS)</dt>
  <dd>The programming language used to build advanced Web sites and applications</dd>
</dl>

### Tables

These are HTML tables :( I want my github flavoured markdown :(

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


-----

Want to see something else added? <a href="https://github.com/poole/poole/issues/new">Open an issue.</a>
