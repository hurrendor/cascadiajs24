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


# Summary 

### Key Themes
- Importance of alternative text (alt text) for accessibility
- Utilizing modern image and animation formats for better performance
- Adapting to user preferences for motion sensitivity
- Enhancing playback controls for better user experience

### Detailed Notes

#### Alternative Text (Alt Text) for Accessibility
- Over half of the top million home pages lack alt text.
- Developers should influence interfaces to include alt text.
- Content creators should describe images as if talking to a friend for clarity.
- Automated tools can help smooth the process of adding alt text.

#### Modern Image and Animation Formats
- Use WebP and AVIF formats for higher quality animations with smaller file sizes.
- WebP has been supported in Chrome for a decade, AVIF offers cutting-edge support.
- These formats offer better image quality, color depth, and are more efficient than older formats.
- Headless tools can be used to generate assets in these formats.
- Cloudinary and similar services can assist in managing and optimizing these assets.

#### Motion Preferences
- Modern operating systems allow users to opt into reduced motion for animations.
- Developers can respect these preferences by providing static alternatives to animated content.
- Use media attributes to dynamically swap between animated and static assets based on user preferences.
- Serve static versions by default and use source elements to provide animations conditionally.

#### Playback Controls
- Individualized playback controls are important due to varying motion sensitivities among users.
- Use video elements with controls and autoplay attributes to enhance user control.
- Implementing playback controls ensures animations are accessible and not overwhelming for users.

#### Best Practices
- Provide alt text and ensure it's associated with the relevant image or video element.
- Use modern formats (WebP, AVIF) for better performance and user experience.
- Respect user motion preferences by offering static alternatives and using media attributes.
- Implement comprehensive playback controls to accommodate different user needs.

#### Progressive Enhancement Techniques
- Use web components to build reusable, customizable elements that enhance user experience.
- Implementing a class to manage media elements dynamically based on user preferences.
- Ensure elements like `aria-label` and `figcaption` are used correctly for accessibility.

#### Conclusion
- GIFs and animations are evolving; modern practices can significantly improve user experience.
- Developers should explore and modernize neglected areas of web development.
- Continuous improvement and user-centered design are crucial for creating accessible, high-performing web content.
