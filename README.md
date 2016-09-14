# tooltip
A simple jQuery plugin to enable quick tooltips.

# Installation
To get this to work, you'll need both the JavaScript and CSS files.

```html
<link rel="stylesheet" href="dist/css/tooltip.css" type="text/css" />
<script src="dist/tooltip.js" type="text/javascript"></script>
```

# Usage
Tooltips can be set up on any item, and when the user puts the mouse over that item, the tooltip will show. By default the title attribute will be used to select what text is shown.

```html
<ul id="menu">
    <li><a href="#" title="This is a tooltip!">Option 1</a></li>
    <li><a href="#" title="This is another tooltip!">Option 2</a></li>
</ul>
```

```javascript
$('#menu a').tooltip();
```

# Options
| Option        | Type      | Default   | Description       |
| ------------- | --------- | --------- | ----------------- |
| title         | String    | ""        | What text to show in the tooltip. If blank, it will use either the title attribute or the data-title attribute on the element. |
| delay         | Integer   | 0         | The delay in milliseconds befor the tooltip shows on mouseover. |
| direction     | String    | "below"   | What direction to show the tooltip. By default the tooltip will show below the element if it's in the top two-thirds of the screen, and above it if it's below that. Can be either "above," "below," or "left" for now. |
