## Sandbox v.1.1

## Concepts

### 1. Generative ColorFlow

prompt
```
use sass to create an animated gradient with values based on complimentary colors with a 3rd color being a neutral gray to near 100% black that uses"colorFlow" as its selector and name of animation in the sass
```
scss
```scss
$color1: #3498db; // Example primary color (blue)
$color2: #e74c3c; // Complementary color (red)
$neutral-color: #333; // Neutral gray to near black

@keyframes colorFlow {
  0% {
    background: linear-gradient(to right, $color1, $color2, $neutral-color);
  }
  50% {
    background: linear-gradient(to right, $color2, $neutral-color, $color1);
  }
  100% {
    background: linear-gradient(to right, $neutral-color, $color1, $color2);
  }
}

.colorFlow {
  animation: colorFlow 5s infinite alternate;
}

```
---

### 2. EventHandling Ui/Ux

abstract
> elements of a component that inform the User and action has completed or an error was encountered through icons, color, and common language contextualization.

html
```html
<div class="notification success" id="success-message">
  <span class="icon">&#10004;</span>
  <span class="message">Action completed successfully!</span>
</div>

<div class="notification error" id="error-message">
  <span class="icon">&#10006;</span>
  <span class="message">An error was encountered. Please try again.</span>
</div>
```

---
---
## Read Me
You can use the [editor on GitHub](https://github.com/joeldom/sandbox/edit/main/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [Basic writing and formatting syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/joeldom/sandbox/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
