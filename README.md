# Slate Design System

[Documentation](https://docs.google.com/document/d/118aDqtW2AZp0_o0QN7OenJNZCx94AkmqtjTJDl3uX4o/edit?usp=sharing)


## The Core 
These Global Content items include Core Design System Properties and Core Design System Styles. Properties such as colors, sizes, and other predefined style values. The Styles serve as a foundation to the encompassing page templates and components while maintaining consistency across all.
> Include this snippet in a code module in the uppermost band of all pages using Slate Design System.
```
<!-- Slate Design System Core Styles and Props -->
[%DS117.data.globalContentLocalized.value.content, $key=slate-core-props%]
[%DS117.data.globalContentLocalized.value.content, $key=slate-core-styles%]
```

## Slate Core Templates

### Template 1
Max Originals & Single Title Landing Pages
```
https://preview.hbomax-web.com/a/template-1
```

### Template 2
Collections
```
https://preview.hbomax-web.com/a/template-2
```

## Slate Core Components
Most components will fall under the Core components category and be available for use on all page templates, only in a few cases will components be used by a single page template.
> Include the relative snippet in a code module in the upper-left-most slot in a band. 
> Style overrides should be added below the snippet, this ensures that the specificity of the overriding styles is higher in the cascade.

### Hero Image
```
[%DS117.data.globalContentLocalized.value.content, $key=slate-hero-image-styles%]
```
with style overrides
```
[%DS117.data.globalContentLocalized.value.content, $key=slate-hero-image-styles%]
<style>
  /* style overrides */
  .slate-section__hero-image {}
</style>
```
### Hero Video 
```
[%DS117.data.globalContentLocalized.value.content, $key=slate-hero-video-styles%]
```
### Hero 3-Up 
```
[%DS117.data.globalContentLocalized.value.content, $key=slate-hero-three-up-styles%]
```
### Watch Band 
```
[%DS117.data.globalContentLocalized.value.content, $key=slate-watch-band-styles%]
```
### Single Video 
```
[%DS117.data.globalContentLocalized.value.content, $key=slate-single-video-styles%]
```
### Double Video 
```
[%DS117.data.globalContentLocalized.value.content, $key=slate-double-video-styles%]
```
### Get Even More (GEM) 
```
[%DS117.data.globalContentLocalized.value.content, $key=slate-gem-styles%]
```
### Grid of Titles (GOT) 
```
[%DS117.data.globalContentLocalized.value.content, $key=slate-got-styles%]
```
### Streaming Devices
```
```
### Supported Devices
```
```

## Core Assets

### HBO Logo in the bottom corners
Include this snippet in a code block in a Hero band for an HBO attribution in either lower corner. These are both included in Template-1.
```
[%DS117.data.globalContentLocalized.value.content, $key=hbo-hero-logo-bottom-left%]
||
[%DS117.data.globalContentLocalized.value.content, $key=hbo-hero-logo-bottom-right%]
```

The color, size or any other style values can be easily over-written by including a `<style>` specification above the snippet. For example...
```
<style>
  [%DS117.data.globalContentLocalized.value.content, $key=hbo-hero-logo-bottom-left%]
  .hbo-hero-logo svg {
    fill: currentColor;
  }
</style>
```

#### Notes
Component styles are marked as .css files although they technically become .html files with the addition of the <style> tag.