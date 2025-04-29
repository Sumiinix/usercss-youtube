# Resize YouTube grid (resize-youtube-grid.user.css)

I created this UserCSS to adjust the number of videos displayed in YouTube's grid layout.  
 Instead of specifying the number of videos per row, this style adjusts the width of the thumbnails.  
 Since the number of videos per row is not fixed, thumbnails will not become squished even if you reduce the browser window's width.

After initially creating this, I found myself wanting to modify other visual aspects as well, so I added a few more tweaks.  
 If you don't need some of the additional features, please feel free to disable them in the style settings.

Example on my Full HD display:
![ex1.jpg](https://github.com/Igusy/style-youtube-grid/blob/5aab8a96888b7e43f15de1c58d0f92dea4fd86c5/screenshots/ex1.jpg)

Example on my 4K display:
![ex2.jpg](https://github.com/Igusy/style-youtube-grid/blob/5aab8a96888b7e43f15de1c58d0f92dea4fd86c5/screenshots/ex2.jpg)

## Installation
To apply this style, please use the Stylus extension.  
I have not tested it with other extensions.

You can install it from this link:  
[Install resize-youtube-grid.user.css](https://github.com/Igusy/style-youtube-grid/raw/main/resize-youtube-grid.user.css)

## Clone this repository
``` shell
git clone https://github.com/Igusy/style-youtube-grid.git
```

## Limitations
YouTube frequently conducts A/B testing, which may cause this style to stop working.  
I have personally encountered cases where the style worked on one account but not on another.

Additionally, since YouTube's layout changes often, some settings might already be outdated.  
Recently, I started using alternative frontends to avoid YouTube's excessive algorithm influence, so I use the official YouTube site less frequently now.  
As a result, it has become difficult for me to maintain this style.  
Feel free to copy, modify, and share this style with anyone who might find it helpful.

## Known Issues
When adjusting thumbnail width, ghost cards (placeholders) that appear during grid loading are hidden.  
This is because I couldn't make the ghost cards display properly under the modified layout.

The thumbnail width dynamically changes depending on your browser window size, ranging between the values set in "Content Size (px) → Width" and "Content Size (px) → Max Width" in the style settings.  
Due to variations in the number of videos per row (e.g., fewer videos because of ad blockers), the last row might have fewer thumbnails than others. In such cases, thumbnails on the last row can appear larger — up to the "Max Width" you set.

If you don't fully understand this behavior, try scrolling to the bottom of your YouTube homepage and observe the thumbnail sizes before new videos load.

If you prefer a consistent thumbnail size regardless of browser width, set the same value for both "Width" and "Max Width" in the style settings.
