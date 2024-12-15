# Introduction to HTML
The goal of this unit is to introduce you to the fundamentals of HTML, one of the languages essential to developing websites.

After this unit, you will be able to:

- Understand how HTML is used for web development
- Use HTML to build a structure for a website
- Create tables in HTML documents
- Write clearer, more accessible HTML using Semantic HTML tags

![[Pasted image 20241205211222.png]]

Let’s quickly review each part of the element pictured:

- HTML element (or simply, element) — a unit of content in an HTML document formed by HTML tags and the text or media it contains.
    
- HTML Tag — the element name, surrounded by an opening (`<`) and closing (`>`) angle bracket.
    
- Opening Tag — the first HTML tag used to start an HTML element. The tag type is surrounded by opening and closing angle brackets.
    
- Content — The information (text or other elements) contained between the opening and closing tags of an HTML element.
    
- Closing tag — the second HTML tag used to end an HTML element. Closing tags have a forward slash (`/`) inside of them, directly after the left angle bracket.

### The Body

One of the key HTML [elements](https://www.codecademy.com/resources/docs/html/elements) we use to build a webpage is the _body_ element. Only content inside the opening and closing body  [tags](https://www.codecademy.com/resources/docs/html/tags) can be displayed to the screen. Here’s what opening and closing body tags look like:

```html
<body>

</body>
```

Once the file has a body, many different types of content – including text, [images](https://www.codecademy.com/resources/docs/html/images) , and buttons – can be added to the body.

```html
<body>  

<p>What's up, doc?</p>

</body>
```

### Divs

7 min

One of the most popular elements in HTML is the `<div>` element. 
[`<div>`](https://www.codecademy.com/resources/docs/html/elements/div?page_ref=catalog) is short for “division” or a container that divides the page into sections. These sections are very useful for grouping elements in your HTML together.

```html
<body>  
	<div>    
		<h1>Why use divs?</h1>    
		<p>Great for grouping elements!</p>  
	</div>
</body>
```

`<div>`s don’t inherently have a visual representation, but they are very useful when we want to apply custom styles to our HTML elements. `<div>`s allow us to group HTML elements to apply the same styles for all HTML elements inside. We can also style the `<div>` element as a whole. You can see how this can be done in the [Learn CSS](https://www.codecademy.com/learn/learn-css) course.

`<div>`s can contain any text or other HTML elements, such as links, images, or videos. Remember to always add two spaces of indentation when you nest elements inside of `<div>`s for better readability.

### Attributes

7 min

If we want to expand an element’s tag, we can do so using an attribute. 
[Attributes](https://www.codecademy.com/resources/docs/html/attributes?page_ref=catalog) are content added to the opening tag of an element and can be used in several different ways, from providing information to changing styling. Attributes are made up of the following two parts:

- The _name_ of the attribute
- The _value_ of the attribute

One commonly used attribute is the `id`. We can use the `id` attribute to specify different content (such as `<div>`s) and is really helpful when you use an element more than once. `id`s have several different purposes in HTML, but for now, we’ll focus on how they can help us identify content on our page.

When we add an `id` to a `<div>`, we place it in the opening tag:

```
<div id="intro">  <h1>Introduction</h1></div>
```

### Attributes

7 min

If we want to expand an element’s tag, we can do so using an attribute. 

Preview: Docs Attributes can be added to the opening tag of an HTML element to change its default behavior or provide additional data about it.

[Attributes](https://www.codecademy.com/resources/docs/html/attributes?page_ref=catalog)

 are content added to the opening tag of an element and can be used in several different ways, from providing information to changing styling. Attributes are made up of the following two parts:

- The _name_ of the attribute
- The _value_ of the attribute

One commonly used attribute is the `id`. We can use the `id` attribute to specify different content (such as `<div>`s) and is really helpful when you use an element more than once. `id`s have several different purposes in HTML, but for now, we’ll focus on how they can help us identify content on our page.

When we add an `id` to a `<div>`, we place it in the opening tag:

```html
<div id="intro">  
	<h1>Introduction</h1>
</div>
```

### Displaying Text

10 min

If you want to display text in HTML, you can use a _paragraph_ or _span_: [_Paragraphs_ (`<p>`)](https://www.codecademy.com/resources/docs/html/elements/p) contain a block of plain text.


[`<span>`](https://www.codecademy.com/resources/docs/html/elements/span?page_ref=catalog) contains short pieces of text or other HTML. They are used to separate small pieces of content that are on the same line as other content.

Take a look at each of these elements in action below:

```html
<div>  <h1>Technology</h1></div><div>  <p><span>Self-driving cars</span> are anticipated to replace up to 2 million jobs over the next two decades.</p></div>
```

In the example above, there are two different `<div>`. The second `<div>` contains a `<p>` with `<span>Self-driving cars</span>`. This `<span>` element separates “Self-driving cars” from the rest of the text in the paragraph.

It’s best to use a `<span>` element when you want to target a specific piece of content that is _inline_, or on the same line as other text. If you want to divide your content into _blocks_, it’s better to use a `<div>`.

### Styling Text

You can also style text using HTML tags. The `<em>` tag emphasizes text, while the `<strong>` tag highlights important text.

Later, when you begin to style websites, you will decide how you want browsers to display content within `<em>` and `<strong>` tags. Browsers, however, have built-in style sheets that will generally style these tags in the following ways:

- The `<em>` tag will generally render as _italic_ emphasis.
- The `<strong>` will generally render as **bold** emphasis.

Take a look at each style in action:

```html
<p><strong>The Nile River</strong> is the <em>longest</em> river in the world, measuring over 6,850 kilometers long (approximately 4,260 miles).</p>
```

In this example, the `<strong>` and `<em>` tags are used to emphasize the text to produce the following:

**The Nile River** is the _longest_ river in the world, measuring over 6,850 kilometers long (approximately 4,260 miles).

As we can see, “The Nile River” is bolded and “longest” is in italics.

### Line Breaks

4 min

The spacing between code in an HTML file doesn’t affect the positioning of elements in the browser. If you are interested in modifying the spacing in the browser, you can use HTML’s _line break_ element: `<br>`.

The line break element is unique because it is only composed of a starting tag. You can use it anywhere within your HTML code and a line break will be shown in the browser.

```html
<p>
The Nile River is the longest river 
<br> 
in the world, measuring over 6,850 
<br> 
kilometers long (approximately 4,260 
<br> 
miles).
</p>
```

The code in the example above will result in an output that looks like the following:

The Nile River is the longest river  
in the world, measuring over 6,850  
kilometers long (approximately 4,260  
miles).

### Unordered Lists

6 min

In addition to organizing text in paragraph form, you can also display content in an easy-to-read list.

In HTML, you can use an _unordered list_ tag (`<ul>`) to create a list of items in no particular order. An unordered list outlines individual _list items_ with a bullet point.

The 

Preview: Docs Represents an unordered list of items.

[`<ul>` element](https://www.codecademy.com/resources/docs/html/elements/ul?page_ref=catalog)

 should not hold raw text and won’t automatically format raw text into an unordered list of items. Individual list items must be added to the unordered list using the `<li>` tag. The `<li>` or list item tag is used to describe an item in a list.

```html
<ul>  
	<li>Limes</li>  
	<li>Tortillas</li>  
	<li>Chicken</li>
</ul>
```

In the example above, the list was created using the `<ul>` tag and all individual list items were added using `<li>` tags.

The output will look like this:

- Limes
- Tortillas
- Chicken

### Ordered Lists

3 min

Preview: Docs Represents an ordered list of items.

[_Ordered lists_ (`<ol>`)](https://www.codecademy.com/resources/docs/html/elements/ol?page_ref=catalog)

 are like unordered lists, except that each list item is numbered. They are useful when you need to list different steps in a process or rank items for first to last.

You can create the ordered list with the `<ol>` tag and then add individual list items to the list using `<li>` tags.

```html
<ol>  <li>Preheat the oven to 350 degrees.</li>  <li>Mix whole wheat flour, baking soda, and salt.</li>  <li>Cream the butter, sugar in separate bowl.</li>  <li>Add eggs and vanilla extract to bowl.</li></ol>
```

The output will look like this:

1. Preheat the oven to 350 degrees.
2. Mix whole wheat flour, baking soda, and salt.
3. Cream the butter, sugar in separate bowl.
4. Add eggs and vanilla extract to bowl.
### Images

5 min

All of the elements you’ve learned about so far (headings, paragraphs, lists, and spans) share one thing in common: they’re composed entirely of text! What if you want to add content to your web page that isn’t composed of text, like 

Preview: Docs Loading link description

[images](https://www.codecademy.com/resources/docs/html/images?page_ref=catalog)

?

The `<img>` tag allows you to add an image to a web page. Most elements require both opening and closing tags, but the `<img>` tag is a _self-closing tag_. Note that the end of the `<img>` tag has a forward slash `/`. Self-closing tags may include or omit the final slash — both will render properly.

```html
<img src="image-location.jpg" 
```

The `<img>` tag has a required _attribute_ called `src`. The `src` attribute must be set to the image’s _source_, or the location of the image. In this case, the value of `src` must be the _uniform resource locator_ (URL) of the image. A URL is the web address or local address where a file is stored.

### Image Alts

4 min

Part of being an exceptional web developer is making your site accessible to users of all backgrounds. In order to make the Web more inclusive, we need to consider what happens when assistive technologies such as screen readers come across image [tags](https://www.codecademy.com/resources/docs/html/tags).

The `alt` attribute, which means alternative text, brings meaning to the [images](https://www.codecademy.com/resources/docs/html/images) on our sites. The `alt` attribute can be added to the image tag just like the [`src`](https://www.codecademy.com/resources/docs/html/attributes/src) attribute. The value of `alt` should be a description of the image.

```html
<img src="#" alt="A field of yellow sunflowers" />
```

The `alt` attribute also serves the following purposes:

- If an image fails to load on a web page, a user can mouse over the area originally intended for the image and read a brief description of the image. This is made possible by the description you provide in the `alt` attribute.
- Visually impaired users often browse the web with the aid of screen reading software. When you include the `alt` attribute, the screen reading software can read the image’s description out loud to the visually impaired user.
- The `alt` attribute also plays a role in Search Engine Optimization (SEO), because search engines cannot “see” the images on websites as they crawl the internet. Having descriptive `alt`  [attributes](https://www.codecademy.com/resources/docs/html/attributes) can improve the ranking of your site.

If the image on the web page is not one that conveys any meaningful information to a user (visually impaired or otherwise), the `alt` attribute should be left empty.

### Videos

7 min

In addition to images, HTML also supports displaying [videos](https://www.codecademy.com/resources/docs/html/videos?page_ref=catalog). Like the `<img>` element, the `<video>` element requires a `src` attribute with a link to the video source. Unlike the `<img>` element however, the `<video>` element requires an opening and a closing tag.

```html
<video src="myVideo.mp4" width="320" height="240" controls>  Video not supported</video>
```

In this example, the video source (`src`) is `"myVideo.mp4"`. The source can be a video file that is hosted alongside your webpage, or a URL that points to a video file hosted on another webpage.

After the `src` attribute, the `width` and `height` attributes are used to set the size of the video displayed in the browser. The `controls` attribute instructs the browser to include basic video controls such as pausing and playing.

The text, `Video not supported`, between the opening and closing video tags will only be displayed if the browser is unable to load the video.

### Review

2 min

Congratulations on completing the first lesson of HTML! You are well on your way to becoming a skilled web developer.

Let’s review what you’ve learned so far:

- **HTML** stands for **H**yper**T**ext **M**arkup **L**anguage and is used to create the structure and content of a webpage.
- Most HTML elements contain opening and closing tags with raw text or other HTML tags between them.
- HTML elements can be nested inside other elements. The enclosed element is the child of the enclosing parent element.
- Any visible content should be placed within the opening and closing `<body>` tags.
- Headings and sub-headings, `<h1>` to `<h6>` tags, are used to provide titles for sections of content.
- `<p>`, `<span>` and `<div>` tags specify text or blocks.
- The `<em>` and `<strong>` tags are used to emphasize text.
- Line breaks are created with the `<br>` tag.
- Ordered lists (`<ol>`) are numbered and unordered lists (`<ul>`) are bulleted.
- Images (`<img>`) and videos (`<video>`) can be added by linking to an existing source.

Here are a few more resources to add to your toolkit:

- Preview: Docs HTML, short for HyperText Markup Language, is the foundation of all web pages. It was created by Tim Berners-Lee in 1993 to define the structure of a web page.
    
    [Codecademy Docs: HTML](https://www.codecademy.com/resources/docs/html)
    
- [Codecademy Workspaces: HTML](https://www.codecademy.com/workspaces/new)

Make sure to bookmark these links so you have them at your disposal.

In the next lesson, we’ll take the content that you’ve added to this website and transform it into an HTML document that’s ready to go on the web.

Full lesson HTML:
```html
<body>
  <h1>The Brown Bear</h1>
  <div id="introduction">
    <h2>About Brown Bears</h2>
    <p>The brown bear (<em>Ursus arctos</em>) is native to parts of northern Eurasia and North America. Its conservation status is currently <strong>Least Concern</strong>.<br /><br /> There are many subspecies within the brown bear species, including the Atlas bear and the Himalayan brown bear.</p>
    <h3>Species</h3>
    <ul>
      <li>Arctos</li>
      <li>Collarus</li>
      <li>Horribilis</li>
      <li>Nelsoni (extinct)</li>
    </ul>
    <h3>Features</h3>
    <p>Brown bears are not always completely brown. Some can be reddish or yellowish. They have very large, curved claws and huge paws. Male brown bears are often 30% larger than female brown bears. They can range from 5 feet to 9 feet from head to toe.</p>
  </div>
  <div id="habitat">
    <h2>Habitat</h2>
    <h3>Countries with Large Brown Bear Populations</h3>
    <ol>
      <li>Russia</li>
      <li>United States</li>
      <li>Canada</li>
    </ol>
    <h3>Countries with Small Brown Bear Populations</h3>
	    <p>Some countries with smaller brown bear populations include Armenia, Belarus, Bulgaria, China, Finland, France, Greece, India, Japan, Nepal, Poland, Romania, Slovenia, Turkmenistan, and Uzbekistan.</p>
  </div>
  <div id="media">
    <h2>Media</h2>
    <img src="https://content.codecademy.com/courses/web-101/web101-image_brownbear.jpg" alt="A Brown Bear"/>
    <video src="https://content.codecademy.com/courses/freelance-1/unit-1/lesson-2/htmlcss1-vid_brown-bear.mp4" width="320" height="240" controls>
    Video not supported
    </video>
  </div>
</body>

```

![[Pasted image 20241205214221.png]]
