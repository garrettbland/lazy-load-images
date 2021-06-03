# lazy-load-images

> 11ty plugin that adds lazy loading attribute to images

## Get Started

Install the package

```bash
npm install -D lazy-load-images
```

Then add the plugin to your `.eleventy.js` file

```javascript
// .eleventy.js
module.exports = (eleventyConfig) => {
  eleventyConfig.addPlugin(require("lazy-load-images"));
};
```

## Usage

No need to do anything else. The plugin will check every image and add the `loading="lazy"` attribute automatically.

## How does it work

This plugin uses `jsdom` to analyze the rendered `html` pages and then adds the `loading="lazy"` atrribute to every `<img/>` element.
