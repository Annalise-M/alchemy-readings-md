CT-Reading Notes 05 - Scraping
---
Web Scraping JavaScript
    @ https://www.scrapingbee.com/blog/web-scraping-javascript/
MDN - querySelector
    @ https://developer.mozilla.org/en-US/docs/Web/API/Document/querySelector
MDN - querySelectorAll
    @ https://developer.mozilla.org/en-US/docs/Web/API/Document/querySelectorAll

---
Understanding Node: A breif introduction
    NodeJS, the crux of the idea was to make Javascript capable of running not only client-side but also server-side.

Request 
    is one of the most widely used HTTP clients in the Javascript ecosystem, however, though currently, the author of the Request library has officially declared that it is deprecated.

Axios
    is a promise-based HTTP client that runs both in the browser and NodeJS.

Superagent
    Much like Axios, Superagent is another robust HTTP client that has support for promises and the async/await syntax sugar. It has a fairly straightforward API like Axios, but Superagent has more dependencies and is less popular.

Regular Expressions
    aren't as flexible and quite a lot of people both professionals and amateurs struggle with writing the correct regular expression.
    
Cheerio
    Cheerio is an efficient and light library which allows you to use the rich and powerful API of JQuery on the server-side.

JSDOM 
    is a pure Javascript implementation of the Document Object Model to be used in NodeJS, as mentioned previously the DOM is not available to Node, so JSDOM is the closest you can get. It more or less emulates the browser.

Puppeteer
    allows you to manipulate the browser programmatically just like how a puppet would be manipulated by its puppeteer. It achieves this by providing a developer with a high-level API to control a headless version of Chrome by default and can be configured to run non-headless.

Nightmare 
    is also a high-level browser automation library like Puppeteer, that uses Electron but is said to be roughly twice as faster as it's predecessor PhantomJS and more modern.

---
querySelector()
    returns the first Element within the document that matches the specified selector, or group of selectors. If no matches are found, null is returned.
        ie.
            element = document.querySelector(selectors);

querySelectorAll() 
    returns a static (not live) NodeList representing a list of the document's elements that match the specified group of selectors.
        ie.
            elementList = parentNode.querySelectorAll(selectors);

            