---
title: Circular text with CSS?
description: Exploring how to lay out text in a circle with new CSS trigonometric functions
oghue: 130
ogtitle: Circular text with CSS?
oggradient: 9
slug: circular-text-with-css
# If you can find an author with this title, do it. Else fallback to main. You can change it easily in the CMS.
author: CSS 
heroDemo:
heroImage:
heroImageAlt:
heroImageAttribution:
tags: CSS, HTML, JavaScript
publishedAt: 2023-01-26
---
Have you ever wanted to lay out some text in a circle but it felt like a lot of prodding in the dark? How might you do it today? Could you do it with CSS alone in an accurate way? Let's take a look at a new way 👀

<TableOfContents></TableOfContents>

## How you might solve this today
You've definitely got options. Before we go down the CSS route, you could use images. The least maintainable route could be creating an image each time you need to change the text. Make sure to use the `alt` attribute to describe the text that's shown.

<INSERT TEXT RING CREATED IN FIGMA>

Or you could use an inline image with SVG. SVG has a `textPath` feature. For the most part, it's pretty good too.

<INSERT SVG DEMO>

Here's a demo using inline SVG and `textPath`. You can change the text and see how it responds. But, you may notice an issue. What's that issue? The radius doesn't scale, it's not content-aware. And this is what I meant when I alluded to "Prodding in the dark" earlier.

For the most part, working in code, we're somewhat wired to assume some degree of accuracy. That is, minus some rounding and other JavaScript quirks. So for me, punching numbers in until it "looks right", sometimes doesn't sit quite well with me.

---

This is also seen when we tackle this with a rudimentary CSS approach. Take a string of text, split it into elements per character, and transform them into a circle.

<INSERT CSS CODE>

## Introducing CSS trigonometric functions

<BrowserSupport></BrowserSupport>

Try not to fear the word "trigonometric". I know, I know. When I hear it, I start thinking of "Differential equations", "Mechanics", and so on. 

<Aside>
Small fact. Not meeting the grade in advanced Mathematics in school put me on the programming path. But, that's a story for another day.
</Aside>

__Stay Awesome!__

