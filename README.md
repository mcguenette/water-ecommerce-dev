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
1. This is my favorite part of the website! The animation of waves was made with HTML and CSS only.
It's using an SVG with a `<g>` group element and several `<use>` elements referencing parts of the SVG by their IDs using the 
`xlink:href` attribute`. The effect is using a repeated pattern to create the illusion of a wave effect.
### Below shows the HTML of the waves effect
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
### Here is the front-end preview on mobile:
![](https://github.com/mcguenette/water_demo_site/blob/main/2023-10-15%2018-45-27.gif)

2. I did research to look for subscription products and on one of the websites I stumbled upon I really liked the way they used a container
and divided the top section where the title was and added a gradient. It was a unique style that I thought would fit our vibe! I went ahead
and created a reponsive design that I hope would make it inticing to purchase.
### Below shows the HTML and CSS for the 1 Month Subscription product _(the HTML is similar for all 4 products, simply content is changed)_
#### HTML:
```
<div class="column column-one">
  <div class="column-title"><h2><span>1</span> Month Subscription</h2></div>
  <img src="./assets/img/1-month.png">
  <h3>$30.<sup>00</sup></h3>
  <p> Get <span>1 case</span> once a month</p>
  <input type="button" class="primary-button" value="Add to cart">
</div>
```
#### CSS:
```
.column {
    -webkit-box-align: center;
    align-items: center;
    background: rgb(255, 255, 255);
    border-radius: 16px;
    box-shadow: rgba(0, 0, 0, 0.1) 0px 8px 24px 0px;
    display: flex;
    flex-direction: column;
    overflow: hidden;
    padding-bottom: 20px;
    position: relative;
}
.column-title {
    color: rgb(56, 56, 56);
    padding: 12px 0px;
    text-align: center;
    font-weight: 900;
    font-size: 18px;
    background: linear-gradient(60deg, rgb(62 92 230) 9%, rgb(110 167 255) 100%);
    width: 100%;
}
```

### Here is the front-end preview on desktop:
![](https://github.com/mcguenette/water_demo_site/blob/main/subs_products.png)





