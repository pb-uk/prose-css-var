# prose-css-var

CSS 'prose' modifiers for putting things right after a hard reset.

## Quick start.

### 1. Install
```console
$ npm install @pbuk/prose-css-var
```

### 2. Include a CSS 'hard' reset and a font stack in your build
If you are using Tailwind CSS you already have this, otherwise you can use the
one at
`./node_modules/@pbuk/prose-css-var/src/css-hard-reset.css`.

### 3. Include the file
`./node_modules/@pbuk/prose-css-var/src/prose-css-var-styles.css`
in your CSS build.

### 4. Set the variables and any optional theme overrides
You can put this anywhere in your CSS build
```css
.prose {
  /* Main elements. */
  --heading-color: currentColor;
  --link-color: #55b;
  --link-hover-color: #33f;
  --code-color: #666;
  --code-bg-color: #ddd;
  --mark-color: currentColor;
  --mark-bg-color: greenyellow;
  --table-border-color: currentColor;
  --table-row-border-color: #777;
  --blockquote-border-color: #777;
  --hr-color: #777;
  --ul-marker-color: #999;
  --figcaption-color: currentColor;

  /* Inputs */
  --input-color: currentColor;
  --input-border-color: currentColor;
  --input-bg-color: transparent;
  --input-placeholder-color: #777;
  --button-hover-bg-color: #777;
}

.dark .prose {
  --link-color: #bbf;
  --link-hover-color: #ddf;
  --code-color: #888;
  --code-bg-color: #222;
  --mark-bg-color: darkslateblue;
  --ul-marker-color: #555;
}
```
### 5. Set the main colour and background colour
Something like the following: the `.dark` and `.light` modes are entirely
optional.
```css
html,
.light {
  color: #111;
  background-color: #eee;
}

.dark {
  color: #eee;
  background-color: #111;
}
```
