<h1>TASKS</h1>
<h2>0. Some early styling</h2>
<ul>
    <li>Create a new directory css_basic in the repository_First_Portfolio</li>
    <li>Copy into this directory the index.html and tweets.html that you created in the html_basic directory of the <a href="https://intranet.alxswe.com/projects/100581">previous project:</a></li>
    <li>Create an empty styles.css.</li>
    <li>Create the file base.css and set the content of this <a href="https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/misc/2021/3/969e3ace19a915eee6fa2ed2b2261497b0e45013.css?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20240625%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20240625T160118Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=354d5cfb6365823b2f0b42f40f41bfe0b5649326dcd25ce28784d567b8fd8da2">file</a></li>
</ul>
<p>
    In each of your HTML files, add these 2 lines which the <head> tag (do not confuse with the <header> tag!):
    <br> <link rel="stylesheet" href="base.css">
    <br> <link rel="stylesheet" href="styles.css">
    <br>
    If you refresh your webpages in your browser, they should now look a bit better! <br>
    We just told your webpages to use the CSS rules described in those two files, and to apply them to your HTML code.
</p>

<h3>Repo:</h3>
<ul>
    <li>GitHub repository: My_First_Portfolio</li>
    <li>Directory: css_basic</li>
    <li>File: base.css, styles.css, index.html, tweets.html</li>
</ul>

<h2>1. Positioning</h2>
<p>
    Even though each element of your webpages now has a different style, you may notice they still are stacked on top of each other, and that's probably not what you want. CSS brings a few different approaches to positioning that one may use depending on cases. <br>

    For this project, we're going to use CSS Flexbox, a recent set of CSS properties that work with recent browsers. <br>

    Our goal is to get a layout that looks like this:

    As a reminder, there are also two container tags playing critical roles here:
</p>
<ul>
    <li><main> contains the area that includes <articles> and <aside></li>
    <li><body> contains all of them together.</li>
</ul>

<p>
    Here are steps to get this layout, which you will have to write as CSS code in the styles.css file:
</p>

<ul>
    <li>
        Both container tags, <body> and <main> must be told that they are containers to flexible boxes: you need to apply the display: flex property to both of them.
    </li>
    <li>
        However, <body> contains a column of three boxes (<header>, <main> and <footer>), therefore you must apply the flex-direction: column property to <body>; whereas <main> contains a row of 2 boxes (<article> and <aside>), so you must apply the flex-direction: row property to <main>.
    </li>
    <li>
        Ensure the <main> tag keeps an automatic height and width, by applying the flex: auto property to it.
    </li>
    <li>
        To wrap up the layout, you want to be sure that your content (article) takes ⅔ of the width of the page, and your aside takes ⅓; you can assign to them the number of boxes they should fill in. This is done by applying the property flex: 2 to <article> (using up 2 boxes), and flex: 1 to <aside> (using up 1 box).
    </li>
    <li>
        Finally, you want to be sure that the user can scroll within your <article> and your <aside>. You can do this by applying the overflow-y: auto CSS property to both of them.
    </li>
</ul>

<p>
    If you've done all of those properly, and your HTML structure is correct, you should get exactly the layout we were trying to get.

    Do note that the exact rendering you're getting may be slightly different depending on your browser (namely, about whether header and footer are fixed or not when the user scrolls), but should always match the layout presented above.
</p>

<h3>Repo:</h3>
<ul>
    <li>GitHub repository: alx_html_css</li>
    <li>Directory: css_basic</li>
    <li>File: styles.css</li>
</ul>

<h2>2. Responsive web design</h2>
<p>
    You may notice that the website keeps this layout when you make your browser window smaller, or visit it from a smartphone, and it's unpleasant to use that way for your users. No worries, we covered this for you: just add the attribute class="works_on_smartphone" on the <body> tag in your index.html file, and the layout you just created will degrade nicely as you resize the window! <br>

    But you'll notice, if you visit your website on a smartphone, that it will still have that layout, and just seem “zoomed out”. That's because you need to adjust what is called the “viewport” of the browser when rendering the page. <br>

    Hint: this gets done by adding a certain tag to your HTML code. <br>

    <strong>
        NB: Do well to thoroughly go through the base css file that was provided to you to understand exactly which styles produces which result.
    </strong>
</p>


<h3>Repo:</h3>
<ul>
    <li>GitHub repository: alx_html_basic</li>
    <li>Directory: css_basic</li>
    <li>File: styles.css, index.html</li>
</ul>

<h2>3. Some more styling</h2>
<p>
    Your website is unique, and if you want it not to look like everyone else's, you may want to take some time to style everything of it as you wish!

What you're allowed to do:
</p>
<ul>
    <li>
        You may add any non-positioning-related CSS rules to styles.css (like colors, backgrounds, borders, …)
    </li>
    <li>
        You may do whatever you want with the HTML content and the CSS that applies inside the <article> tag.
    </li>
    <li>
        You may add a logo to the top-left of your page. To keep it simple, rather than use an image, feel free to use a unicode character, from this table for instance. One way to make it work: add a first item in the list in your <header>, before all other list items, and just put the HTML-code for the character in it (it starts with “&” and ends with “;”). To make it look like a logo, if you want the character to be bigger, you can add the class="logo" attribute on the
    </li>
    <li>
        tag, we added the CSS rule for you.
    </li>
    <h3>What you're not allowed to do:</h3>
    <li>
        Do not change the layout strategy, done with CSS Flexbox, as described above. Feel free to experiment with positioning within the <article> tag if you wish; but please refrain to do so anywhere else.
    </li>
</ul>


<h3>Repo:</h3>
<ul>
    <li>GitHub repository: alx_html_basic</li>
    <li>Directory: css_basic</li>
    <li>File: styles.css, index.html</li>
</ul>