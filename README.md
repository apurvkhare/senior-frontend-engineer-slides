# Becoming a Senior Frontend Engineer

-- [Apurv Khare](https://www.linkedin.com/in/apurvkhare/)

## About me

- Web developer with 7 years of experience building large scale frontend applications
- Software Engineer 3 @ Adobe
- I love teaching and dancing
- I have a youtube channel [WhatTheCode](https://www.whatthecode.academy/) where I teach and a [discord server](https://discord.com/invite/EpsnK6csnM) of 1400+ developers
- I have mentored and taught 1000+ developers and made them a better developer. Some of my mentees work in Amazon, Flipkart, Freshworks, etc.
- I teach what I know and learn what I don't

## Agenda

- Technical capabilities
- Non-technical capabilities
- How do you realize that you have become a senior engineer

## The basics

- [Semantic HTML authoring](https://developer.mozilla.org/en-US/docs/Web/HTML/Reference)
- [CSS fundamentals](https://web.dev/learn/css/) - how to render your UI on screen, paper, in [speech](https://www.w3.org/TR/css-speech-1/) and other media
- [Javascript](https://javascript.info/) in depth - keep learning as much as you can

## Web fundamentals

- [Critical Rendering Path](https://www.udacity.com/course/website-performance-optimization--ud884)
- [DNS](https://www.cloudflare.com/learning/dns/what-is-dns/)
- [HTTP](https://developer.mozilla.org/en-US/docs/Web/HTTP) - HTTP 1.0, 1.1, 2, 3
- [Broweser dev tools](https://developer.chrome.com/docs/devtools/) - Network, Performance, Memory
- [Web storage](https://developer.mozilla.org/en-US/docs/Web/API/Web_Storage_API) - local storage, session storage, [cookies](https://developer.mozilla.org/en-US/docs/Web/HTTP/Cookies)
- [Web security](https://www.youtube.com/playlist?list=PL1y1iaEtjSYiiSGVlL1cHsXN_kvJOOhu-) - familiarize with [OWASP top 10](https://owasp.org/www-project-top-ten/)

## Command over the UI framework

- Understand how the framework works internally
- Be aware of the design patterns of the framework like [compound components](https://advanced-react-patterns.netlify.app/2)
- Debugging in the performance in the framework - [React profiler](https://react-performance.netlify.app/7)
- Optimizing the performance - [not immaturely but when needed](https://kentcdodds.com/blog/usememo-and-usecallback)

## What does it take to build large scale frontend application?

What does 'scaling' mean on the frontend?

## Scale on the Frontend

- Adaptive UI
- Observability & Monitoring
- Application deployment infrastructure
- Web app performance optimization
- Accessibility
- Internationalization

## Adapative UI

- Responsive: web app that adapt to their environments like screens sizes
- OS Theme: Dark/Light
- Interaction methods: mouse, keyboard, touch, stylus, screen reader

## [Observability](https://www.splunk.com/en_us/data-insider/what-is-observability.html) & Monitoring

- Observability is the practice of instrumenting systems to gather actionable data depicting not only when and where an issue occurred, but—more importantly—why it occurred.
- Monitoring is actually an important action in achieving observability.
- Monitoring is the act of collecting regular data about systems so performance can be viewed and tracked.

## [Telemetry data types](https://newrelic.com/platform/telemetry-data-101)

- Events - a discrete action happening at a moment in time
- Metrics - numeric measurements (average, total, minimum, maximum)
- Logs - lines of text a system produces when certain code blocks get executed
- Traces - chains of events (or transactions) between different components in a microservices ecosystem

## Application deployment infrastructure

- [Nginx](https://www.freecodecamp.org/news/the-nginx-handbook/)
- Docker & Kubernetes
- [CDN](https://www.cloudflare.com/learning/cdn/what-is-a-cdn/)
- Database cluster
- Data centers & cloud instances
- Upstream and downstream services deployment

## Web app performance optimization

- Network tab request waterfall
- Optimize the render and parse blocking assets
  - preload the "above the fold" images, fonts, etc
  - defer non-critical Javascript and CSS

## first load times

- resource hints (pre-load, pre-fetch, etc)
- script attributes (defer, async)
- asset minification (minify css, js bundles)
- bundlesize budgeting
- optimizing images (use WebP format, lazy-load)
- optimize long running tasks in your JS (memoize, use web worker)
- optimize resource delivery (CDN)
- optimize third-party JS ([party-town](https://partytown.builder.io/))

## Second and further load times

- [HTTP caching](https://developer.mozilla.org/en-US/docs/Web/HTTP/Caching)
- The server can instruct proxies and clients about what to cache and for how long
- Two types of client caching
  - private: cache tied to a specific client — typically a browser cache. used to store a personalized response for that user.
  - public/shared: cache is located between the client and the server in places like proxy or reverse-proxy. used to store responses that can be shared among users.

## [Accessibility on the web](https://web.dev/learn/accessibility/)

- Ensure that everyone, including people with disabilities, can still interact with your website in a meaningful and equal way
- The World Health Organization (WHO) estimates that over 15% of the world's population or 1.3 billion people self-identify as having a disability
- Types of disabilities includes visual impariments, mobility impairments, hearing impariments, coginitive impariments, seizure and vestibular disorders

## Missed opportunity in potential revenue

- According to the American Institutes for Research (AIR), the total after-tax disposable income for working-age Americans with disabilities is about $490 billion annually
- People with disabilities are also part of a larger network of family members, friends, communities, and institutions. This larger network often looks for and supports businesses that create accessible digital products
- With that factored in the disability market touches 53% of all consumers

## Legal

- In countries such as Canada, the United Kingdom, Japan, Australia, and the European Union, stricter digital accessibility laws exist for both public and private companies
- In fact, of the top 500 e-commerce sites, 412 have been served with a lawsuit within the past four years. Often, the first lawsuit is for the company's website and the second for their mobile app

## How to develop accessible web apps

- Write semantic HTML - use HTML elements to structure your content based on each element's meaning, not its appearance.

## Non semantic HTML

```
  <div>
  <span>My awesome website</span>
  <div>
    <a>Home</a>
    <a>About</a>
    <a>Products</a>
    <a>Contact</a>
  </div>
  </div>
  <div>
  <div>
    <div>About</div>
  </div>
  <div>
    <div>Vision</div>
    <div>Make awesome products</div>
    <div>Use best in class tech</div>
  </div>
  <div>
    <div>Clients</h2>
    <div>Company one</div>
    <div>Company two</div>
  </div>
  </div>
  <div>
    <span>Copyright 2023</span>
  </div>
```
## semantic HTML

```
  <header>
  <h1>My awesome website</h1>
  <nav>
    <a>Home</a>
    <a>About</a>
    <a>Products</a>
    <a>Contact</a>
  </nav>
  </header>
  <main>
  <header>
    <h1>About</h1>
  </header>
  <section>
    <h2>Vision</h2>
    <p>Make awesome products</p>
    <p>Use best in class tech</p>
  </section>
  <section>
    <h2>Clients</h2>
    <p>Company one</p>
    <p>Company two</p>
  </section>
  </main>
  <footer>
  <p>Copyright 2023</p>
  </footer>
```

## ARIA

- Accessible Rich Internet Applications
- A set of attributes you can add to HTML elements to increase their accessibility. These attributes communicate role, state, and property to assistive technologies via accessibility APIs found in modern browsers
- [WAI-ARIA authoring practices](https://www.w3.org/WAI/ARIA/apg/patterns/)

## [Internationalization](https://www.w3.org/International/questions/qa-i18n)

- Internationalization is the process of structuring your code and user interface to support localization
- Localization is the process of adapting an application for a particular language or region. It includes translating text content, as well as bi-directionality, adapting date formatting, number formatting, collation and sorting, text search, and more

## Non-technical capabilities

## PR reviews
- code quality
- using established patterns
- readability over fancy code
- DRY but not at the cost of over abstraction
- test the code!!!
- leave comments as a construtive feedback with proper justification for changes where required

## Be the goto person

- There is always a person whom you go to when you are stuck with something for a long time and you know that that person will definitely resolve the issue
- Become a excellent debugger and problem solver, its just about not giving up

## Take initiative and do POC

- If you see a problem in the product or process of engineering that you are working on which can be solved techincally then take up the initiative to solve it
- Come up with a proof of concept and demonstrate it to your product and project managers or anyone in the leadership

## Become a product engineer

- Focus on user experience first and then the technical challenges not the other way round
- Sometimes we are so lost in the techical challenges that we resist the new requirements which actaully makes the product better and more useable by the consumers

## Become a demo expert

- Very important, if you want to be noticed in a larger audience including the leadership
- Know the usecase of the requriements that are developed
- Prepare a demo script and review it with you product and project manager
- Speak slow and confidently

## Become the manager of your career

- discuss about your career progression with the manager at the start of the yearly cycle not the end
- schedule quarterly check-ins with your manager to get his/her feedback and inform him/her about your challenges
