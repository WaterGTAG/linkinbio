# watergtag/linkinbio
**Starter link in bio template in HTML/CSS**

When making my own link-in-bio for **[links.watergtag.com](https://links.watergtag.com)**, I realized how amazing it is to make your own link-in-bio page. It's super customizable, but not everyone knows how to code a page like that from scratch. I made a **simple starter template** using parts from my own link-in-bio to allow people to make their own page. You can use the README as a tutorial to get started, or put your code to the test & add completely new features.

The page itself is also super lightweight, only using 9.61 KB of code, and 190 KB if you count the SVGs and fonts.

## Beginner Tutorial
### 🔗 How do I add & customize links?
Right between where the links start & the footer starts (line 24-31), you should see an `<a>` block with the class name `class="linkinbio"`. Inside, you'll find `<p>` tags. This is where you customize the title & URL.
> 💡 Make sure the change the href of the `<a>` property, this is how the button actually redirects you!
```
    <a href="ENTER URL HERE" class="linkinbio">
      <div class="w-element linkinbio-div"><img class="linkinbio-img" alt="" src="ENTER IMAGE HERE>
        <div class="linkinbio-text">
          <p class="linkinbio-title">ENTER TITLE HERE</p>
          <p class="linkinbio-url">ENTER URL HERE</p>
        </div>
      </div>
    </a>
```
### 🎨 How do I change colors & font?
To change colors, on the top of style.css, you should see color & font variables. These variables affect the whole page.

To add your own font, you must import your own font file & change the following to point to your own font:
- `<link rel="preload" href="YOUR FONT FILE NAME HERE" as="font" crossorigin="anonymous" />` in index.html (for both preloads)
- `@font-face` in style.css, change `font-family` to the font's name, and `src` to the file name.
- `--global-font: Clash Grotesk, sans-serif;` in style.css, change this to the font name you used in Step 2.

For fonts that are pre-installed on most computers such as Arial, Times New Roman, e.t.c, you only need to do steps 2-3, and you can delete the preloads from step 1. (or keep them, but it might affect your site's speed a tiny bit.)
### ✏️ How do I add my name & description?
Below `<header>`, you should see all the information on top of the page, such as header-banner, header-pfp, header-name, or header-desc. For text, edit inside the tag. For images, edit the src.
