# Read Topics 17:

## **Scrapping** 'Static V.S. Dyncamic websites':

Scraping static and dynamic websites involve different techniques and considerations. Here are the key differences between scraping static and dynamic websites:

1- **Content Rendering:** Static websites are pre-rendered and served as HTML, Dynamic websites, on the other hand, generate content dynamically using JavaScript and AJAX calls. 

2- **JavaScript Execution:** Static websites do not rely heavily on JavaScript, In contrast, dynamic websites heavily utilize JavaScript to render content dynamically.

3- **Interactivity and User Input:** Dynamic websites often have interactive elements that require user input or trigger events to load content.


## Avoid Blocking while scraping:


To avoid getting blocked while scraping websites, you can employ several techniques and best practices. Here are three commonly used approaches:

1- **Respectful Crawling:** Adhering to the guidelines set by the website and being respectful of its resources is crucial to avoid being blocked.

2- **Implement IP Rotation and Proxies:** By rotating your IP addresses and using proxies, you can distribute your scraping requests across multiple IP addresses, reducing the chances of being detected and blocked.

3- **Use Headless Browsers:** Headless browsers simulate a real browser environment, enabling the execution of JavaScript, handling of cookies, and rendering of dynamic content. 


## Playwright:


Playwright is an open-source automation framework developed by Microsoft. It provides a high-level API for browser automation and is particularly useful for web scraping tasks. 

Here's an example of a use case where Playwright would be beneficial:

Suppose you need to scrape data from a website that heavily relies on client-side rendering, JavaScript, and AJAX calls. Traditional scraping techniques that only fetch the initial HTML source may not capture the dynamically loaded content. In such cases, Playwright shines by providing a headless browser environment to automate the scraping process.


## XPath

The purpose of using XPath in web scraping is to precisely target and extract desired data from a webpage. XPath expressions allow you to traverse the HTML document's hierarchy and select elements based on their relationships with other elements, their attributes, or the text they contain. XPath expressions can be used with various programming languages and libraries to extract data from HTML pages.

Here's an example of an XPath expression to select a specific HTML element from a webpage:
```
//h1[@class="title"]
```