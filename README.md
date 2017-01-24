# Intro to Coding
To practice what we've just learnt, we're going to build a very basic HTML and CSS Page. If you have atom/sublime or some another code editor installed, then [click here to download the starter code](https://github.com/wdi-sg/intro-to-coding/archive/master.zip). If not you can head over to [codepen](http://codepen.io/pen) and just practice online.

_NB. If you are working in a code editor like Atom, then be sure to open the html page in your web browser and reload after each change you make._

## Part 1: Adding Context to Content with HTML
This is the copy we will be using for our example but feel free to replace it with your own.
```txt
Ada Lovelace

https://upload.wikimedia.org/wikipedia/commons/thumb/a/a4/Ada_Lovelace_portrait.jpg/220px-Ada_Lovelace_portrait.jpg" alt="image desc

Augusta Ada King-Noel, Countess of Lovelace (née Byron; 10 December 1815 – 27 November 1852) was an English mathematician and writer, chiefly known for her work on Charles Babbage's early mechanical general-purpose computer, the Analytical Engine. 

Her notes on the engine include what is recognised as the first algorithm intended to be carried out by a machine. As a result, she is often regarded as the first computer programmer.

Read More on Wikipeadia https://en.wikipedia.org/wiki/Ada_Lovelace

Other influential people include
Charles Babbage
Alan Turing
Percy Ludgate
```

Copy and paste the above into your HTML Page or HTML tab in Codepen. We can now start to wrap it in HTML.

### Heading 1

Wrap Ada's name in a __h1 tag__ as it is our main page title.
```html
<h1>Ada Lovelace</h1>
```

### Image
Wrap the image URL in a __img tag__. Give it an alternative text option using the __alt tag__.
```html
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/a/a4/Ada_Lovelace_portrait.jpg/220px-Ada_Lovelace_portrait.jpg" alt="Ada Lovelace">
```

### Paragraphs
We have two paragraphs of text, wrap each one in __p tags__.
```html
<p>Augusta Ada King-Noel, Countess of Lovelace (née Byron; 10 December 1815 – 27 November 1852) was an English mathematician and writer, chiefly known for her work on Charles Babbage's early mechanical general-purpose computer, the Analytical Engine.</p>
<p>Her notes on the engine include what is recognised as the first algorithm intended to be carried out by a machine. As a result, she is often regarded as the first computer programmer.</p>
```

### Strong
Let's make the last sentence in the second paragraph more important using a __strong tag__. This will be nested inside the existing p tag.
```html
...As a result, <strong>she is often regarded as the first computer programmer.</strong></p>
```

### Link
Wrap the link in an __a tag__ so that user can click on it to follow to Wikipedia. Let's also set the target attribute to _blank - this means it will open in a new tab/window rather than leaving the current page.
```html
<a href="https://en.wikipedia.org/wiki/Ada_Lovelace" target="_blank">Read More on Wikipedia</a>
```

### Aside
The information about other people is kind of an aside from our main text, so let's wrap the whole section in an __aside tag__. 

```html
<aside>
  Other influential people include
  Charles Babbage
  Alan Turing
  Percy Ludgate
</aside>
```

### Aside Heading
Let's take the first line in the aside as use it as a heading by wrapping it in a __h2 tag__. 
```html
<aside>
  <h2>Other influential people include</h2>
  Charles Babbage
  Alan Turing
  Percy Ludgate
</aside>
```
### Aside List
Let's make the list of people a bullet pointed (unordered) list by wrapping in an __ul tag__. 
```html
<aside>
  <h2>Other influential people include</h2>
  <ul>
    <li>Charles Babbage</li>
    <li>Alan Turing</li>
    <li>Percy Ludgate</li>
  <ul>
</aside>
```
---

## Part 2: Adding Style to Content with CSS
Now that we've learnt about CSS, let's add some style to our site. In your CSS file or CSS tab in Codepen let's add the following rules. 

### Body
Let's tell our page body to have 0 margin and a nice background-color e.g. thistle.
```css
body {
  background-color: thistle;
  
  margin: 0;
}
```

### h1
Let's tell our heading level 1 to be aligned to the right and have a right margin of 10px.
```css
h1 {
  text-align: right;
  
  margin-right: 10px;
}
```

### h2
Let's tell our heading level 2 to have a left margin of 10px.
```css
h2 {
  margin-left: 10px;
}
```

### img
Let's tell our img to have a 2 pixel wide solid border in purple. Let's change the corner radius to be 5px. Let's give it a 10px margin on all sides except the top. Also we can tell it to float to the left, this means that the text will wrap round.
```css
img {
  border: 2px solid purple;
  border-radius: 5%;
  
  margin-right: 10px;
  margin-bottom: 10px;
  margin-left: 10px;
  
  float: left;
}
```

### aside
Let's give our aside a background-color or white and change the text color to purple to create some contrast. Let's also change the position so it is absolutely positioned at the bottom of the page and fills the full width.

```css
aside {
  background-color: white;
  color: purple;
  
  position: absolute;
  bottom: 0;
  
  width: 100%;
}
```

### li
Let's have a little bit more fun by adding a hover state to our list items, so that they become bold whenever we hover over them.
```css
li:hover {
  font-weight: bold;
}
```
---

## Part 3
All done! View the results, smile and play around with some styling ideas of your own :-) 

---

## Licensing
1. All content is licensed under a CC-BY-NC-SA 4.0 license.
2. All software code is licensed under GNU GPLv3. For commercial use or alternative licensing, please contact legal@ga.co.
