### Styling with CSS – Zara the Butterfly Joins the Fun

One sunny morning, Andy and Samy sat under a tree, looking at their website.

“It’s coming together nicely, Alhamdulillah,” Andy said.

“But it’s so plain,” Samy frowned. “How can we make it more beautiful?”

Just then, a colorful butterfly named Zara landed gracefully beside them. “Salam, friends! I heard you want to add some style to your website. I’m Zara, the meadow’s design expert!”

Samy’s eyes widened. “MashAllah, you look amazing! Can you teach us how to style our website?”

Zara smiled. “Of course! Let’s start with **CSS**, the secret to making websites beautiful.”
### What is CSS?

“CSS stands for **Cascading Style Sheets**,” Zara explained. “It’s like giving your website a makeover! It allows us to change colors, fonts, sizes, and more.”

Samy tilted his head. “Where do we write CSS?”


### Where to write CSS ?

Zara pointed to the HTML file. “We can write CSS in three ways:

1. **Inline CSS:** Inside an HTML tag.
2. **Internal CSS:** In a `<style>` section inside the HTML file.
3. **External CSS:** In a separate `.css` file.”
### CSS Selectors

 “How does CSS know which parts of your webpage to style?” Samy asked.

“Great Question, That’s where **selectors** come in,” Zara explained. “Selectors tell CSS exactly which parts of the HTML to style. It’s like picking specific flowers from a garden to arrange a bouquet. Let me show you.”

“Here’s a quick guide to the selectors” Zara said, spreading her wings:


1. `tagname` – Type Selector (Specific tag like `<p>` or `<h1>`)
2. `.classname` – Class Selector (A group of elements)
3. `#idname` – ID Selector (One unique element)
4. `tag1, tag2` – Group Selector (Style multiple elements the same way)
5. `parent child` – Descendant Selector (Elements inside a specific parent)
6. `:hover`, `:active` – Pseudo-Classes (Interaction-based styling)
7.  `*` – Universal Selector (selects Everything!)

Samy buzzed happily. “SubhanAllah, CSS selectors are like tools to arrange a garden perfectly!”

Activity: https://flukeout.github.io/ 
### Adding Internal CSS

“For now, let’s start with **internal CSS** to keep things simple,” Zara said.
Zara showed them how to add a `<style>` section inside the HTML file:

```html
<!DOCTYPE html>
<html>
<head>
    <title>Andy and Samy’s Website</title>
    <style>
        body {
            background-color: lightblue;
        }
    </style>
</head>
<body>
    <h1>Welcome to Our Website!</h1>
    <p>Sharing Allah’s blessings with the world.</p>
</body>
</html>

```

“See? This adds a light blue background to the whole page,” Zara explained.

Samy buzzed with excitement. “SubhanAllah! That already makes a big difference!”

---

### Changing Colors

“Let’s add more color to the text,” Zara suggested:

```html
<style>
    h1 {
        color: green;
    }
    p {
        color: darkblue;
    }
</style>
```

“The `color` property changes the text color,” Zara explained. “Here, the heading is green like grass, and the paragraph is dark blue like the sky.”

Samy clapped his wings. “It’s so vibrant now!”

---

### Adjusting Text

“Now let’s make the text look better by changing its size and alignment,” Zara said:

```css
h1 {
	color: green;
	font-size: 36px;
	text-align: center;
}
p {
	color: darkblue;
	font-size: 18px;
	font-family: Arial, sans-serif;
}
```

- `font-size` changes the size of the text.
- `text-align` centers the heading.
- `font-family` sets the font style.

Samy buzzed happily. “Wow! Now it’s easy to read and looks great!”

---

### Styling the List

“Remember your list of blessings? Let’s style it too!” Zara said.

```css
ul {
	list-style-type: square;
	color: darkgreen;
}
li {
	font-weight: bold;
	margin: 5px 0;
}
```

- `list-style-type` changes the bullet style.
- `font-weight` makes the text bold.
- `margin` adds space between list items.

Samy admired the changes. “SubhanAllah, now the list looks so organized!”

---

### Adding Borders

“Let’s give your image a nice border,” Zara suggested:

```css
img {
	border: 3px solid darkblue;
	border-radius: 8px;
	width: 300px;
}
```

- `border` adds a border around the image.
- `border-radius` makes the corners rounded.
- `width` adjusts the image size.

Samy buzzed in excitement. “Now it looks like a framed picture! This is so much fun!”

---


### Positioning in CSS

Zara gently landed on a large rock. “There are five main ways to position elements in CSS. Imagine you’re arranging pebbles in a garden path.”

She drew five spots in the sand and labeled them:

🌿 **Static** – The default way elements appear. They follow the normal flow of the page.  
🌿 **Relative** – The element stays in the normal flow, but you can move it slightly using `top`, `right`, `bottom`, or `left`.  
🌿 **Absolute** – The element is removed from the normal flow and placed exactly where you want it, relative to the nearest positioned ancestor.  
🌿 **Fixed** – The element stays in the same spot, even when you scroll. Like a butterfly sitting on your screen!  
🌿 **Sticky** – The element sticks when scrolling but only within a certain area. Like a floating leaf!

Zara showed them an example:

```css
.box {     
	position: relative;     
	top: 50px;     
	left: 100px; 
}
```

“This places the `.box` exactly **50 pixels down** and **100 pixels from the left**.”

Samy gasped. “That’s like placing a flowerpot exactly where I want it!”

### Block vs. Inline – Understanding Element Behavior

Zara flapped her wings. “Before arranging elements, we need to understand **how they behave**.”

She pointed to two rows of stones:

🪨 **Block elements** (like `<div>`, `<p>`, `<h1>`) take up the full width and push the next element to a new line.  
🌸 **Inline elements** (like `<span>`, `<a>`, `<strong>`) stay in the same line and only take up as much space as needed.

Samy looked at the stones and laughed. “So **block elements** are like big boulders—you can’t put two in the same row. And **inline elements** are like small flowers—they fit together side by side!”

Zara nodded. “Exactly! You can change an element’s behavior with `display: block;` or `display: inline;`.”
### Layouts with Flexbox and Grid

Zara then pointed to a row of perfectly aligned pebbles.

"Now, let's organize our garden neatly using **layouts**."

Samy tilted his head. "Layouts?"

"Yes! There are **two powerful ways** to arrange elements in CSS: **Flexbox and Grid**."

#### Flexbox – Arranging Elements in a Row or Column

"Flexbox is great when you want to arrange elements **in a straight line**—either **horizontally or vertically**."

She showed an example:

```css
.container {     
	display: flex;     
	justify-content: center; /* Aligns items in the center */     
	align-items: center; /* Aligns items vertically */     
	gap: 20px; /* Adds space between items */ 
}
```

📌 **Key Flexbox Properties:**  
✅ `display: flex;` – Enables flexbox layout.  
✅ `flex-direction: row | column;` – Defines direction.  
✅ `justify-content: start | center | space-between;` – Aligns items horizontally.  
✅ `align-items: start | center | stretch;` – Aligns items vertically.

Samy clapped. “So Flexbox is like arranging flowers **in a straight row**!”

Zara nodded. “Yes! But what if you need a full garden layout?”

---
####  CSS Grid – Organizing the Whole Page

Zara pointed to a **flower bed** with rows and columns.

“**Grid** lets you place elements **in both directions—rows and columns.**”

She showed another example:

```css
.container {     
	display: grid;     
	grid-template-columns: 1fr 2fr 1fr;     
	grid-template-rows: auto;     gap: 10px; 
}
```

📌 **Key Grid Properties:**  
✅ `display: grid;` – Enables grid layout.  
✅ `grid-template-columns` – Defines column structure.  
✅ `grid-template-rows` – Defines row structure.  
✅ `gap` – Adds spacing between items.

Samy gasped. “So **Grid is like a flowerbed where each plant has a perfect spot!**”

Zara smiled. “Exactly! **Flexbox** is great for arranging elements **in a row**, while **Grid** is perfect for **complex layouts**.”
### Putting It All Together

By the end of their session, their styled website looked like this:

```html
<!DOCTYPE html>
<html>
<head>
    <title>Andy and Samy’s Website</title>
    <style>
        body {
            background-color: lightblue;
        }
        h1 {
            color: green;
            font-size: 36px;
            text-align: center;
        }
        p {
            color: darkblue;
            font-size: 18px;
            font-family: Arial, sans-serif;
        }
        ul {
            list-style-type: square;
            color: darkgreen;
        }
        li {
            font-weight: bold;
            margin: 5px 0;
        }
        img {
            border: 3px solid darkblue;
            border-radius: 8px;
            width: 300px;
        }
    </style>
</head>
<body>
    <h1>Welcome to Our Website!</h1>
    <p>Sharing Allah’s blessings with the world.</p>
    <ul>
        <li>Sunlight</li>
        <li>Fresh air</li>
        <li>Water</li>
        <li>Beautiful flowers</li>
    </ul>
    <img src="meadow.jpg" alt="A beautiful meadow full of flowers">
</body>
</html>

```

---

### Zara’s Final Words

“With just a few lines of CSS, your website now looks beautiful!” Zara said.

Samy buzzed happily. “Alhamdulillah, CSS is like the art of the meadow—it brings everything to life!”

Andy smiled. “Thanks to Zara, we’ve learned how to style our website step by step. Now, we’re ready to inspire others!”

Zara fluttered her wings. “And remember, the best designs are those that reflect the beauty and blessings of Allah. Salam, my friends!”

