# Frontend Mentor - FAQ accordion card solution

This is a solution to the [FAQ accordion card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/faq-accordion-card-XlyjD0Oam). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Overview

The FAQ accordion card challenge on Frontend Mentor is an extremely common front-end pattern, so it's a great opportunity to get some practice in! Innitialy this challenge was to be done with javaScript but there was a bonus point to one who used only HTML & CSS so I decided to go the hard way 🤣.

### The challenge

Users should be able to:

- View the optimal layout for the component depending on their device's screen size
- See hover states for all interactive elements on the page
- Hide/Show the answer to a question when the question is clicked

### Screenshot

![](./images/Frontend%20Mentor%20FAQ%20Accordion%20Card.png)

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

### Built with

- Semantic HTML5 markup
- CSS
- Flexbox

### What I learned

In this challenge I managed to research and read about the two ways of writting accordion tags more especially with HTML and CSS and also watched a youtube video and learnt the best way to style your `<details>Details Tags</details>` & `<summary>Summary Tags</summary>`.

```html
<details>
  <summary>What is the maximum file upload size?</summary>
  <p>
    No more than 2GB. All files in your account must fit your allotted storage
    space.
  </p>
</details>
```

```css
details > summary::after {
  content: "";
  background: url("./images/icon-arrow-down.svg") center no-repeat;
  width: 1rem;
  height: 1rem;
  transition: 0.5s ease;
}

details[open] > summary::after {
  transform: rotate(180deg);
}

/*for chrome, opera, safari & edge*/
details > summary::-webkit-details-marker {
  display: none;
}
```

### Continued development

During Development I successfully failed to style my accordion card to ensure that content doesn't overflow outside the card when the details tag is opened and am planning to continue researching about this issue untill I fully address the problem.

I'm also not certain how to implement this card with plain JS so am to dig more about the other way of coming up with this card and also ensuring that the functionality in the card works as expected.

### Useful resources

- [Accordion with HTML Elements "details" and "summary"](https://www.imarketinx.de/artikel/html-accordion-details-and-summary.html) - This wonderful article helped me to understand how to write the Accordion with HTML Elements **details** & **summary**.

## Author

- Frontend Mentor - [@ssembatya-dennis](https://www.frontendmentor.io/profile/ssembatya-dennis)
- Twitter - [@DennisSsembatya](https://twitter.com/DennisSsembatya)
