---
id: m0u4j1cr4dskyo987zzqdax
title: Gifs Forever
desc: 'Everyone loves animated GIFs, right? Not if you have finite bandwidth, a shaky network connection or motion sensitivity! But fear not… modern browsers make it easier than ever to level up our GIF game!'
updated: 1718900245992
created: 1718900199601
---

# GIFS Are Forever, Let's Make Them Better
## Tyler Sticka
(Recorded Talk)[TBA]


### Speaker Information
x - (@tylersticka)[https://twitter.com/tylersticka]
LinkedIn - @tylersticka
@tylersticka@social.lol
Website - [cloudfour.com](https://cloudfour.com/) 
(Cascadia Talk Information)[https://cascadiajs.com/2024/talks/gifs-are-forever-lets-make-them-better]


## Improving the GIF Experience
Existing GIF attributes
Animated, Silent, Looping, inline, autoplay
### Adding items to the checklist of needs
#### Text alternatives
    - Provide `alt` text descriptions for images used!
    - Write alt text like you're talking to a friend 

#### Higher Quality, Smaller Size
Use modern file types like WebP, AVIF to provide higher quality while reducing the size of the file.

##### Other options (libraries): 
sharp, libvips, gif2webp, FFmpeg, lmageMagick 

##### Services:
- Cloudinary (Biased Link)[cloudfour.com/make]


### Motion preferences
Default to a static image asset to provide non-animated versions for user preferences

### Playback control
Give users individualized control by providing the 
`<video control>` attribute. Changing GIF to video file types is comparable in size.    
Attributes like `<video control autoplay loop muted playinline>`
#### Alt Text on Playback
- Use the HTML <figure>and <figcaption> elements
- Use an aria-label combined with the controls attribute
- Use aria-labelledby={elementID} and a combined div or other HTML element container to capture the alt text

#### Motion preferences
Use Web Components to
- check the media query using `window.matchMedia`
(Example Code in a Gist)[gist.github.com/tylersticka]


## Resources
[web.dev Article - Lazy Loading Video](https://web.dev/articles/lazy-loading-video)