Pre Class Session 5 March 2, 2021  Notes 

New tools to use to improve your site:

1. [a11y Color Contrast Accessibility Validator](https://color.a11y.com/Contrast/) (WCAG 2.1 AA SC 1.4.3 Test for Color Contrast): Also referred to as "A11y" and "A11Y," a11y is an abbreviation for "accessibility" that is more compact for the character limits on social media. The “11” in the middle stems from conventions in software engineering and Information and Communication Technology that shortens long words by substituting middle letters with the number of middle letters instead. There are 11 letters between the "a" and the "y," so accessibility becomes a11y. For another example, “l10n” refers to "localization," because 10 letters come between the “l” and the “n.”

Coincidentally, a11y looks like it would read phonetically as ally, which has been the topic of controversy in some circles on social media.

No less, many technologists see a11y as a movement, and not just the simple act of making websites more accessible. To learn more about a11y, please visit [What is a11y?](https://www.boia.org/blog/what-is-a11y#:~:text=May%204%2C%202017,character%20limits%20on%20social%20media.).

2. [W3C HTML Markup validation Service](https://validator.w3.org/#validate_by_uri+with_options) - validates your HTML markup (and more)

When you use the W3C Markup Validation Service, make sure to select the following:

a. First make sure that you have selected the Validate by URI tab.

b. First make sure that you expand the More Options dropdown arrow.

c. For Character Encoding, select utf-8 (Unicode, Worldwide)

d. For Document Type, select HTML5 (experimental)

e. Select the List Messages Sequentially radio button.

f. Check the Show Source checkbox.

g. Check the Show Outline checkbox.

h. Check the Clean up Markup with HTML-Tidy checkbox.

i. Check the Validate error pages checkbox.

Then click the Check button to validate your HTML page. The link has to point to a page on a live site. Not to a page n a local server on your computer.

3. Lighthouse Chrome Extension (I mentioned this before, but it really is an essential tool for web design and development today): even lets you know what is wrong or not semantic about your HTML markup.

I have uploaded my portfolio.html page (along with my other "dummy pages") to my domain name on Namecheap. I made a few changes afterwards, and this is what it looks like now: [letsbsocial.nyc](https://www.letsbsocial.nyc/portfolio.html)

Please be sure to also check out the HTML markup and CSS code changes I made available for viewing(and as a guide) on the [Sectioning HTML](https://github.com/interglobalmedia/sectioning-html) slide deck repository on Github.

If there is anything else I can think of before class on Tuesday, March 2, 2021, I will add it here. Thanks!

Notes  re portfolio.html semantic HTML  2.27.21: 

At first, as you know, I had only had used the section semantic html element to wrap around three figure elements at a time. This meant I ended up with 4 sections, each containing 3 figure elements with their corresponding figcaptions.

However, when I tested for semantic HTML and how it affected my SEO, I thought I should add a main heading to the page (h1), and then h2 headings to each section. However, I could not place these headings inside their corresponding sections, because the section element is the CSS Grid container, and anything else added to that container would throw off the columns. I had to think of another way.

At first I tried to use the hgroup element which was still listed in the HTML Living Standard, but has been announced for a while everywhere that it had been removed from the HTML5 specification. So that was no long er a valid option!

I decided to circumvent my section h2 heading issue by wrapping an article element around the h2 element and its subsequent section element containing 3 figure elements in each section element. So now for each "section" containing 3 birds each, it starts off with the article element, followed by the h2 element, then the section element, then the three figure elements with their corresponding figcaption elements.

I placed the h1 element at the bottom of the header element below the nav element.

I hope the evolutionary process as well as the thought process behind structuring my portfolio.html page based both on taking semantic HTML into consideration and taking into account the CSS styles being used and how change in page structure could affect it, will be of some help to you all. Thanks!