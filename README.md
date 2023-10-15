# Water eCommerce website (no js)

## Description
This was our very first web project with MITT / software developer program.
The requirements were to create a website that included a **homepage**, **about us** page as well as a **contact us** page.
All of this was made for a _fake_ company that we invented, I say we because my partner and I worked on this together.

## Decisions and considerations
- Create a new fake company
- Discuss and implement branding
  - Select colour palette, logos and fonts.
- Consider light mode or dark mode
- What products to sell
- Who the founders are
- Utilize chat gpt for content

## Challenges
From my perspective, dark mode was the more difficult challenge as we tried it first and by the time things we're being styled
something didn't sit right and together we agreed that even with a little more work light mode would make it easier for us at 
this time, and next time after more practice we can try again. I would love to try and create both light and dark modes for this 
project. With a switch or automatically through OS settings.

The other challenge was working together at the same time to create elements, etc. Because we only had one day in class and the 
rest was remote we needed to find a solution on how to work on the website at the same time. From industry experience in git 
command, I thought that would be the best solution. However we had to compromise as many other peers are not yet familiar and
instead using github desktop would be a great alternative. We were able to work with github desktop and create commits and merge
requests to complete our work.

## Here are some examples of code
This is my favorite part of the website! The animation of waves was made with HTML and CSS only.
It's using an SVG with a `<g>` group element and several `<use>` elements referencing parts of the SVG by their IDs using the 
`xlink:href` attribute`. The effect is using a repeated pattern to create the illusion of a wave effect.
```
<div class="waves-container">
    <svg class="waves" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"
    viewBox="0 24 150 28" preserveAspectRatio="none" shape-rendering="auto">
    <defs>
        <path id="gentle-wave" d="M-160 44c30 0 58-18 88-18s 58 18 88 18 58-18 88-18 58 18 88 18 v44h-352z" />
    </defs>
        <g class="parallax">
            <use xlink:href="#gentle-wave" x="48" y="0"/>
            <use xlink:href="#gentle-wave" x="48" y="3"/>
            <use xlink:href="#gentle-wave" x="48" y="5"/>
            <use xlink:href="#gentle-wave" x="48" y="7"/>
        </g>
    </svg>
</div>
```





