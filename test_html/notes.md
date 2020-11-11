# Notes from html course:
- Websites to assist you:
	* [w3schools](https://www.w3schools.com/html/) : There is a tutorial for html
	* [MDN web docs](https://developer.mozilla.org/en-US/docs/Web/HTML/Element) : Mozilla docs for html references, etc.

## Introduction
- The attributes of `<font>` are inside the brackets, eg. `size` `style`
- `<br>` to break a line in the webpage
- `&nbsp` for making a non-breakable space. You have to place it next to the text, without any spaces, and this command will make a space in the output webpage
- For `<a href = "..."> Click here </a>` the computer starts searching from the path that this code is in. You need relative path, not full path to another .html file
- You create an anchor by `<a name = " name of anchor" >  ... </a> Then you refer to it by the code above.
- Don't modify both `width` and `height` of a photo. It will change it's dimensions.
- For image mapping, you have three area options:
	1. Rectangle
	2. Circle
	3. Polygon
- For `iframe` you can embed your own website, or if you want to embed youtube or google maps, it's really easy, just click share, then embed, and you will see the whole code generated.
- Tables have four components:
	1. Caption (title of table)
	2. Header (first row)
	3. Data
	4. Footer (last row of table)
- For forms, change the attribute `method="post"` so that the answers aren't shown on the link when you submit it.
- In head attributes or body, `<script src = "...">  </script>` is for writing Javascript or importing Javascript, `<style> </style>` is for CSS.
- For head attributes: 
	* `<meta>` is data for search engines so that they can identify your website.
	* `<base>` is for assigning the default path to use later for src directory.
	
	
## CSS introduction
- Syntax of CSS code consists of: `selector {property : value ;}` eg. `body {color : navy;}`
- When using CSS to change elements in html, eg. color of body text, you can overwrite these CSS rules, by using a font tag `<font> ... </font>`. Then you can write whatever you want inside the tag.
- Selectors in CSS, which are `element` , `class`, `id` and `inline` have a priority difference. So, if you have `inline` and `element` describing an `<h1>` tag, then `inline` will be the one applied.
- There are different type of combinators and multiple selectors:
	* Multiple: `h1 , h2 , h3 { ... }` this prevents redundancy of code.
	* `div h1 { ... }` selects `<h1>` inside `<div>` tag. `<h1>` tag doesn't necessarly have to be the immediate child. it can be inside `<p>` tag
	* `div > h1 { ... }` selects `<h1>` that is immediate child of `<div>`
	* `div + h1 { ... }` selects the first `<hl>` that is after `<div>` tag. If there is another `<h1>` tag after, it won't be selected.
	* `div ~ h1 { ... }` selects all `<h1>` tags after `<div>` tag. It can be one or multiple `<h1>` tags.
- Attributes in CSS `[]` `^` `*` `$` `~`
- **Very important that spaces in CSS file have meaning eg. `div [width="50px"] { ... }` is different from `div[width="50px"] {}`**
- There is difference between pseudo-element selector `::selection` and `:hover`
- Remember to place the `css-reset.css` file before your actual `css` file, so that it will reset everything then will apply your customization



