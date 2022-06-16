# BEM Methodology

BEM (Block, Element, Modifier) methodology is based on the principle of partitioning the interface into independent blocks. It allows easy and quick make a page of any complexity and to reuse already existing code.

## Block
**Block** — independient component of the page which can be used several times.<br/>
<br/>
Before naming block class, we have to answer the question *«What is it?»*<br/>
<br/>
Names are written in **lowercase Latin letters**.<br/>
<br/>
Words are separated by a **hyphen *(-)***<br/>
<br/>
In CSS for blocks **you shouldn't use external geometry and positioning**. Thus, block becomes independent and it can be reused.<br/>
<br/>
For example:
```html
<div class="title"></div>
<form action="#" class="search-form"></form>
```
```sass
.title {
  text-transform: uppercase
  font-size: 34px
  letter-spacing: 8.95px
  // Don't do this:
  margin: 0 0 20px 0
  padding: 0 20px 
}
```
Blocks can be nested. Any nesting level is allowed. Example:
```html
<!-- "about" block -->
<div class="about">
  <!-- "title" nested block -->
  <div class="title"></div>
  <!-- "subtitle" nested block -->
  <div class="subtitle"></div>
</div>
```
