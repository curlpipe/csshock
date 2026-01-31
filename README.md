# CSShock ⚡

If you've ever found CSS cumbersome, try CSShock

## ✨ Features

- **🎯 Single-File Library** - Everything is in one CSS file, no JS required
- **🎨 Simple Theming** - Edit the CSS file with your styling preferences of colour, size and font
- **📐 Powerful Layout System** - Intuitive and powerful layout systems that sit on top of CSS
- **🚀 Utility Classes** - Tailwind-style utilities for rapid development
- **⚡ Zero Configuration** - No build tools or complicated setup required

## 📦 Installation

### Download

Download the `csshock.css` file directly and include it in your project:

```html
<link rel="stylesheet" href="path/to/csshock.css">
```

### Edit

There is a section at the top of the file that you can edit:

You can use the defaults, or you can modify them:

- Choose your colour palette
- Assign colors to your theme
- Modify the spacing used throughout your website
- Set up your font family, size and weights
- Provide border width and radius sizes
- Tweak how shadows will look

```css
:root {
  /* Palette */
  --red: #BD5757;
  --orange: #BD7057;
  --yellow: #BD9657;
  --green: #59BD57;
  --blue: #578BBD;
  --purple: #7457BD;
  --pink: #BD57BD;
  --white: #E0E0E0;
  --black: #1A1A2E;
  --dark-grey: #2E2E2E;
  --light-grey: #737373;
  
  /* Theme */
  --text-color: var(--black);
  --background-color: var(--white);
  --accent-color-1: var(--purple);
  --accent-color-2: var(--blue);
  --border-color: var(--accent-color-1);
  --code-background: var(--dark-grey);

  /* Spacing */
  --spacing-xxs: 0.25rem;
  --spacing-xs: 0.375rem;
  --spacing-sm: 0.5rem;
  --spacing-md: 1rem;
  --spacing-lg: 2.5rem;
  --spacing-xl: 5rem;
  --spacing-xxl: 9.5rem;

  /* Fonts */
  --font-family: 'DM Sans', sans-serif;
  --font-size-xxs: 0.6rem;
  --font-size-xs: 0.8rem;
  --font-size-sm: 1rem;
  --font-size-md: 1.2rem;
  --font-size-lg: 1.4rem;
  --font-size-xl: 1.8rem;
  --font-size-xxl: 2.5rem;
  --font-weight-light: 400;
  --font-weight-normal: 500;
  --font-weight-bold: 700;

  /* Border */
  --border-width: 1px;
  --border-radius-sm: 1rem;
  --border-radius-md: 1.4rem;
  --border-radius-lg: 2rem;

  /* Shadows */
  --shadow-sm: 0 1px 2px rgba(0, 0, 0, 0.1);
  --shadow-md: 0 4px 6px rgba(0, 0, 0, 0.1);
  --shadow-lg: 0 10px 20px rgba(0, 0, 0, 0.15);
}
```

### Use

See documentation below on how to get the best out of CSShock

## 📖 Documentation

### Basic Styling

#### Containers

Use these classes to add standardized padding to your main content areas:
`container-xxs`, `container-xs`, `container-sm`, `container-md`, `container-lg`, `container-xl`, `container-xxl`

These are great for breaking up sections with divs and adding nice spacing to the sides of your content

#### Colours

Add the following classes to style your components with your chosen theme colours

Backgrounds: `bg-red`, `bg-orange`, `bg-yellow`, `bg-green`, `bg-blue`, `bg-purple`, `bg-pink`, `bg-white`, `bg-black`, `bg-dark-grey`, `bg-light-grey`, `bg-accent`

Text (Foreground): `fg-red`, `fg-orange`, `fg-yellow`, `fg-green`, `fg-blue`, `fg-purple`, `fg-pink`, `fg-white`, `fg-black`, `fg-dark-grey`, `fg-light-grey`, `fg-accent`

Note that the accent colours are chosen in the `:root` part of your CSShock file.

#### Dark & Light Mode

Toggle your entire theme by adding a single class to the `<body>` tag:
- `theme-light`: Light mode
- `theme-dark`: Dark mode

#### Size and Spacing

Replace `[size]` with: `xxs`, `xs`, `sm`, `md`, `lg`, `xl`, or `xxl`.

- **Padding (All sides):** `p-[size]`
- **Padding (Left and Right):** `px-[size]`
- **Padding (Top and Bottom):** `py-[size]`
- **Padding (Top):** `pt-[size]`
- **Padding (Bottom):** `pb-[size]`
- **Padding (Left):** `pl-[size]`
- **Padding (Right):** `pr-[size]`

- **Margin (All sides):** `m-[size]`
- **Margin (Left and Right):** `mx-[size]`
- **Margin (Top and Bottom):** `my-[size]`
- **Margin (Top):** `mt-[size]`
- **Margin (Bottom):** `mb-[size]`
- **Margin (Left):** `ml-[size]`
- **Margin (Right):** `mr-[size]`

#### Typography

- **Alignment:** `font-left`, `font-center`, `font-right`
- **Weight:** `font-weight-light`, `font-weight-normal`, `font-weight-bold`
- **Sizing:** `font-xxs`, `font-xs`, `font-sm`, `font-md`, `font-lg`, `font-xl`, `font-xxl`.

#### Components

Most components in CSShock already have styles applied to them by default, so no need to add 100 classes to your elements.

#### Buttons

There are two classes you can add to `<button>` elements:

- `primary` - the button that is recommended to click
- `secondary` - the other option

By default, buttons will be styled as primary by default.

#### Navigation

The `<nav>` tag is pre-configured to handle layouts automatically.

It is stack by default, and will bunch when on mobile.

### Layout System

The most innovative part of CSShock is its layout system.

The layout system is called stack-bunch.

Let's say you have some HTML elements you want to display.

In CSShock, there are two main ways to organise this data

#### Stack

Think of a Stack like a stack of pancakes. Each element you place inside it sits directly on top of the next, growing vertically.

![Stack of pancakes](https://static.wikia.nocookie.net/goodfood/images/e/e9/Stack-of-pancake-mix.jpg/revision/latest?cb=20180619222536)

This is good if you're creating vertical lists or forms.

Stack works really nicely on mobile devices, where there is limited screen width.

The good news is that you don't need to decipher lots of ugly HTML classes, you can use stack like this:

```html
<stack>
    <img src="/path/to/img1.png">
    <img src="/path/to/img2.png">
    <img src="/path/to/img3.png">
</stack>
```

All images will be on top of each other

#### Bunch

Think of a Bunch like a bunch of bananas hanging side-by-side. Elements are placed in a horizontal row.

![Bunch of bananas](https://upload.wikimedia.org/wikipedia/commons/6/69/Banana.png)

This is good if you're creating a navbar, gallery of images side-by-side or some horizontal group of buttons.

The good news is that you don't need to decipher lots of ugly HTML classes, you can use bunch like this:

```html
<bunch>
    <img src="/path/to/img1.png">
    <img src="/path/to/img2.png">
    <img src="/path/to/img3.png">
</bunch>
```

All images will be shoulder to shoulder, next to each other

#### How do I control the spacing between them?

Use the `gap` attribute, which can be `xxs`, `xs`, `sm`, `md`, `lg`, `xl`, or `xxl`.

This can be used with stacks or bunches.

Here's an example:

```html
<bunch gap="md">
    <img src="/path/to/img1.png">
    <img src="/path/to/img2.png">
    <img src="/path/to/img3.png">
</bunch>
```

#### How do I create columns?

Really really easy! You'll need to use a bunch.

```html
<bunch>
	<div share="quarter">
        <h1>Column 1</h1>
        <h2>Loreum Ipsum</h2>
    </div>
    <div share="quarter">
        <h1>Column 2</h1>
        <h2>Loreum Ipsum</h2>
    </div>
    <div share="quarter">
        <h1>Column 3</h1>
        <h2>Loreum Ipsum</h2>
    </div>
    <div share="quarter">
        <h1>Column 4</h1>
        <h2>Loreum Ipsum</h2>
    </div>
</bunch>
```

This will create 4 columns, each sharing a quarter of the total space, thanks to the `share` attribute.

This share attribute can be:

- `"half"`
- `"third"`
- `"quarter"`
- `"fifth"`
- `"sixth"`
- `"seventh"`
- `"eighth"`
- `"ninth"`
- `"tenth"`
- `"eleventh"`
- `"twelth"`
- Any number (in quotes) from 1 to 12 to share up the space

If you want six columns, you can assign each child element a `"sixth"`, for example.

You could also have 3 elements in a row, and have one with `"half"` and the other two as `"quarter"` to fill up the rest of the space.

There are many combinations.

*What happens when I make elements share more space than there exists*

Like, what happens when you have 4 elements each trying to share a half of the space?

Default behaviour is that it will overflow, however, you can wrap them around, so you can create a grid of columns!

simply add `wrap` to your bunch:

```html
<bunch wrap>
	<div share="half">
        <h1>Column 1</h1>
        <h2>Loreum Ipsum</h2>
    </div>
    <div share="half">
        <h1>Column 2</h1>
        <h2>Loreum Ipsum</h2>
    </div>
    <div share="half">
        <h1>Column 3</h1>
        <h2>Loreum Ipsum</h2>
    </div>
    <div share="half">
        <h1>Column 4</h1>
        <h2>Loreum Ipsum</h2>
    </div>
</bunch>
```

This creates a 2x2 grid of columns! Don't forget that `wrap` in the bunch opening tag!

You can have different rows, with different proportions, observe this layout, with two columns in the first row, and 3 in the second row:

```html
<bunch wrap>
	<div share="half">
        <h1>Column 1</h1>
        <h2>Loreum Ipsum</h2>
    </div>
    <div share="half">
        <h1>Column 2</h1>
        <h2>Loreum Ipsum</h2>
    </div>
    <!--     columns wrap around here (two halfs fill the space) -->
    <div share="third">
        <h1>Column 3</h1>
        <h2>Loreum Ipsum</h2>
    </div>
    <div share="third">
        <h1>Column 4</h1>
        <h2>Loreum Ipsum</h2>
    </div>
    <div share="third">
        <h1>Column 5</h1>
        <h2>Loreum Ipsum</h2>
    </div>
</bunch>
```

With that, you can now create all kinds of column configurations to suit your needs.

Quick tip: if you have a stack/bunch and you want things to fill the full space of the stack bunch, just add `share="1"` to all child elements, and they will fill the space

#### How do I make this responsive?

Say you have a bunch - this uses a lot of width. If you open your website on mobile, you might want to instead display the HTML elements under each other (as a stack). 
Good news - you can have a bunch that dynamically changes to be a stack on certain screen sizes

The following attributes can be either `"stack"` or `"bunch"`:

- `on-mobile` - decide whether to be stack or bunch on a mobile device
- `on-tablet` - decide whether to be stack or bunch on a tablet device
- `on-desktop` - decide whether to be stack or bunch on a laptop/desktop device

Here's an example of a gallery of images side-by-side that will dynamically change to be under each other when the website is opened on a mobile device

```html
<bunch on-mobile="stack">
    <img src="/path/to/img1.png">
    <img src="/path/to/img2.png">
    <img src="/path/to/img3.png">
</bunch>
```

It really is that easy.

Best practice: when using stacks or bunches, define all of the above attributes to firmly decide how your content should look across devices

Here's another example:

```html
<bunch on-mobile="stack" on-tablet="stack">
    <img src="/path/to/img1.png">
    <img src="/path/to/img2.png">
    <img src="/path/to/img3.png">
    <img src="/path/to/img4.png">
    <img src="/path/to/img5png">
    <img src="/path/to/img6.png">
</bunch>
```

Here we have a bunch on desktop, but as soon as the viewport width goes into tablet/mobile territory, it switches to a stack.

#### How can I align things?

Gone are the days where you struggled to center a div!

There are 2 main attributes you can use to align content on both stacks and bunches:

- `yalign` - this will align on the y axis (top to bottom)
    - `"top"` - keeps elements at the top of the stack/bunch
    - `"center"` - keeps elements in the middle of the stack/bunch
    - `"bottom"` - keeps elements at the bottom of the stack/bunch
    - `"around"` - evenly puts space around each element in the stack/bunch
    - `"between"` - puts space between each element in the stack/bunch
- `xalign` - this will align on the x axis (left to right)
    - `"left"` - keeps elements in the left of the stack/bunch
    - `"center"` - keeps elements in the middle of the stack/bunch
    - `"right"` - keeps elements in the right of the stack/bunch
    - `"around"` - evenly puts space around each element in the stack/bunch
    - `"between"` - puts space between each element in the stack/bunch

Play around with each value to see what you can do.

Here is an example:

```html
<bunch yalign="center" xalign="around">
    <img src="/path/to/img1.png">
    <img src="/path/to/img2.png">
    <img src="/path/to/img3.png">
</bunch>
```

This will create a nice image gallery that is centered in the bunch, and are equally spaced out.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

**Made with ⚡ by [curlpipe](https://github.com/curlpipe)**
