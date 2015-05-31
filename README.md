# Vanilla JS smooth scroll

A simple vanilla javascript implementation of smooth scrolling that implements
event delegation and requestAnimationFrame (includes polyfill).

This is the most stripped down, un-complicated version of vanilla javascript scroll I could find. It is a modified
version of [Robin Leve](http://codepen.io/rleve/) smooth-scroll. Restructured to include requestAnimationFrame,
event delegation (instead of forEach loop), and adding an offset option (mostly for fixed headers).

I prefer to have my polyfills in one .js file that I include before everything else. However, I went ahead
and added the rAF polyfill at the top of the script. Feel free to remove it if you already have a rAF polyfill or
you whatever.

## Usage

 - Include the script in your project
 - Add a class of 'scroll' to your anchor tags
 - Options data-scroll-speed (default 500), data-scroll-offset (default false)

## Example

**HTML**
```
    <a href="#about" class="scroll" data-scroll-offset="40">About</a>

    <!-- lot's of page markup -->

    <section id="about">
    <!-- about section markup -->
    </section>
```

This will smooth scroll to the about section with a 40px offset

## Todo

Add built-in and customizable easing functions
