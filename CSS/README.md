# CSS

- known as Cascading Stylesheet
- describes how you will design your HTML elements in your web page.

> When you see CSS, think 'Design'.

###**File Extension: .css**

> **Ways to add it in your HTML File:**
>
> 1. By writing it inline with your HTML element (Inline CSS)
>
>	```
>		<h1 style="color:blue;">Hello World</h1>
>	``` 
>
> 2. By inserting it to your HTML file using the style tag in the `<head> </head> section`. (Internal CSS)
>
>	```
>	    <style>
>			h1 { color: blue; }
>       </style>
>   ```	
>
> 3. By linking your CSS file in the head section of your HTML file using the link tag (External CSS)
>
>	HelloWorld.html
>
>	```
>		<head>
>			<link rel="stylesheet" href="HelloWorldStyle.css">
>		</head>
>
>		<body>
>			<h1>Hello World</h1>
>		</body>
>   ```
>
>   HelloWorldStyle.css
>
>   ```
>		h1 {
>	       color: blue;
>     	}
>
>   ```
>

###**Syntax**

**CSS Declaration:**

Compose of:

1. Property - identifies the feature of the HTML elements you want to manipulate (eg. color)
2. Value - describes the characteristics of your feature (eg. blue)

*Example:*

* property - color
* value - blue
* : - separates the property and value
* ; - separates two declaration 

> **Syntax style:** `property : value`

` color: blue; `

> To separate two declaration, we use `;`.


**CSS Declaration Blocks:**

- when you have a group of declarations, you grouped it in a block.
- a block is starts with `{` and ends with `}`. The content goes inside the curly braces.

Delimeter: { } - opening brace `{` and closing brace `}`

```
{
	color: blue;
 	background-color: red;
}
```

**CSS rulesets**

Ruleset 
- pair selector-declaration block
- a.k.a. rule

Parts:

1. Selector - part of the HTML element that you want to target. It is written before the declaration block
2. Declaration Block
3. Declarations


Single Selector - h1

```
h1 {
	color: blue;
 	background-color: red;
}
```

Group of Selectors - div h1

```
div h1 {
	color: blue;
 	background-color: red;
}
```

**Cascade Algorithm** 
- determines which rule will affect what element based on several ruleset since it is possible that one element of a web page can be affected by multiple declarations or declaration blocks.


NOTE:
CSS are not intended to insert text content. That's the responsibility of HTML. But for this practice, we will be doing this so we can write "Hello World" using CSS. 

The only way you can add in text using CSS is with the `content` property. This will only work on pseudo elements `:before` and `:after`.

Pseudo elements are not selecting anything on the html file rather it adds something on the html.

```
<style>
	h1:before { 
		content: "Hello";
	}

	h2:after { 
		content: "World";
	}
</style>
```

**Screenshot of Result here:**

![Hello World CSS Output](https://raw.githubusercontent.com/michieriffic/say-hello-world/master/CSS/HelloWorldCSS_WebScreenShot.png)
