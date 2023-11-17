# CDN_System_Design

## 1. Introduction

A content delivery network (CDN) is a geographically distributed group of servers that work together to provide fast delivery of internet content. Generally, static files such as HTML/CSS/JS, photos, and videos are served from CDN.
A content delivery network (CDN) is a geographically distributed group of servers that work together to provide fast delivery of internet content. Generally, static files such as HTML/CSS/JS, photos, and videos are served from CDN.

![xs](https://github.com/dhruv2x/CDN_System_Design/assets/84621641/32e62abe-e424-44bb-aae7-da87b8f28389)

Hierachy

![hi](https://github.com/dhruv2x/CDN_System_Design/assets/84621641/4842d32b-ff25-4640-9253-2a9b8867cf8a)


## 2. High-Level Design

Working

![sx](https://github.com/dhruv2x/CDN_System_Design/assets/84621641/c5c0f802-9503-4d01-b264-64584f8242e9)


High-Level Design

![ss](https://github.com/dhruv2x/CDN_System_Design/assets/84621641/edaefe63-8a62-4d5b-9548-92deaa9ec920)

- **Origin servers:** These are the servers that store the original content, such as HTML, CSS, JavaScript, images, and videos.
- **Edge servers:** These are servers that are located closer to the users than the origin servers. They store cached copies of the content, which can be delivered to users more quickly.
- **Routing system:** This system directs user requests to the nearest edge server.
- **Distribution system:** This system keeps the cached content on the edge servers up to date.
- **Data control system:** This system monitors and manages the CDN network.
- **Scrubber servers:** These servers protect the CDN network from attacks.

**How it works:**

1. A user requests a web page or other content from a website.
2. The user's DNS server resolves the website's domain name to the IP address of the nearest edge server.
3. The user's browser sends a request to the edge server for the content.
4. The edge server checks its cache for the content. If the content is cached, the edge server delivers it to the user's browser. If the content is not cached, the edge server requests it from the origin server.
5. The origin server delivers the content to the edge server, which then caches it for future requests.
6. The edge server delivers the content to the user's browser.

The benefits of using a CDN include:

- **Reduced latency:** Users receive content from the server that is closest to them, which reduces latency and improves performance.
- **Improved reliability:** If one edge server is unavailable, the routing system can direct requests to another edge server. This improves the reliability of the CDN network.
- **Reduced load on the origin server:** Edge servers cache and deliver content, which reduces the load on the origin server. This improves the scalability of the website or web application.
- **Improved security:** CDN networks can use scrubber servers to protect against attacks such as DDoS attacks.

CDN systems are used by a wide variety of websites and web applications, including streaming video services, social media platforms, and e-commerce websites.
