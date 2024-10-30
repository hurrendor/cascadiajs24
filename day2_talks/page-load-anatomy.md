---
id: spzek7vctrdv03oxsidd6a3
title: Page Load Anatomy
desc: 'The need to scale for high traffic and accommodate low end devices for great user experiences requires modern approaches. ANATOMY OF A MODERN PAGE LOAD is a look at the means by which we are prioritizing performance and the new APIs available'
updated: 1718990971962
created: 1718990908697
---
# Anatomy of a Modern Page Load
## Henri Helvetica
[YouTube Recording](https://www.youtube.com/watch?v=aMYQVXQV9J4&list=PLLiioAbFTbKPi9SkDhtppEGDPI31GGZyj&index=20&pp=iAQB)

## Speaker Information
x - (@henrihelvetica)[https://twitter.com/henrihelvetica]
Instagram - @henrihelvetica
LinkedIn - @henrihelvetica
Mastadon - @henrihelvetica 
(Cascadia Talk Information)[https://cascadiajs.com/2024/talks/anatomy-of-a-modern-page-load]

## 2024 Page Load
TTFB - Time to First Byte
RUM - Real User Monitoring
LCP - Largest Contentful Paint
CLS - Cumalitive Layout Shift
TBT - Total Blocking Time
INP - Interactive Next Paint

- Use CDNs for HTML
Get the information out there as fast as possible.

## Early Hints - HTTP 103 Code
Server think-time allows a browser to preconnect to sites or start preloading resources before the server has prepared and sent that final response.
Supported by major browsers but requires some server configuration.

### LCP Breakdown
Good < 2500ms, Poor > 5000ms
- 70% of LCP is images
- Load critical resources first.
- Preloading (ex: `<link rel="preload">`) or `fetchpriority="high"`
- Optimizing the image does not reduce the network delay issues. 

### Accelerating the Page
Reviewing the waterfall, identify long-running tasks that can block up the main browser thread and disable user interaction. Reducing these reduces rage-clicks.
Breaking up long tasks can help reduce the time.

### Prefetch / Prerender
Preload the resources
Use prerendering attributes to define the eagerness level (`moderate`, `immediate`, `conservative`)

### RUM vs Lab
Real user data will always be different than lab-derived data

### Tips
1. Test
2. Reduce latency - how fast can things get on the page or loaded?
3. Prioritize critical resources / break up tasks
4. Look at your data
