# salium
Salium is a collection of [OriginOS](https://github.com/Mistium/Origin-OS) themes and wallpapers that can be accessed through the respective OSL program.

# How to Contribute
If you're looking to update or modify the Salium OSL program, you're in the wrong place. The source code can either be accessed directly in OriginOS or through the [Rotur Apps repository](https://github.com/RoturTW/apps).

## Creating Themes
All themes are handled through `themes.json`. To create a new theme, duplicate one of the pre-existing theme objects and replace the following information:
```js
{
    "name": "My Theme", // The name to be associated with your theme (try to keep this under 16 characters)
    "author": "Alice", // Your name
    "tags": "red, blue, light", // A list of tags; see the section below.
    "primary": "#fff", // user.theme.primary
    "secondary": "#fff", // user.theme.secondary
    "tertiary": "#fff", // user.theme.tertiary
    "text": "#f00", // user.theme.text
    "background": "#fff", // user.theme.background
    "accent": "#0f0" // user.theme.accent
}
```
Your theme can have as few or as many tags as you'd like. If your theme revolves around one or more specific colors, consider including those colors as a tag. Please don't use the "default" tag, that is reserved only for themes built into OriginOS. **All themes must contain a "light" or "dark" tag.**

## Creating Wallpapers
Wallpapers are created similarly to themes, however the wallpaper image is stored in a seperate file. Your wallpaper must be a .PNG or .JPG file, and must have a somewhat descriptive name (basically, no `IMAGE_5067.jpg`'s or anything like that). Your wallpaper must be of reasonable quality and aspect ratio.

Once you've uploaded your wallpaper image to the `./wallpapers` directory, navigate to `wallpapers.json` and duplicate one of the pre-existing wallpaper objects and replace the following information:
```js
{
    "name": "My Wallpaper", // The name to be associated with your wallpaper (try to keep this under 16 characters)
    "author": "Alice", // Your name
    "tags": "scenery, green, calm", // A list of tags; see the section below.
    "src": "https://raw.githubusercontent.com/antiviiris/salium/main/wallpapers/wallpaper.jpg" // The URL of the raw GitHub content for your image.
}
```
Your wallpaper can have as few or as many tags as you'd like. If your wallpaper revolves around one or more specific colors, consider including those colors as a tag. Please don't use the "default" tag, that is reserved only for wallpapers built into OriginOS.

## Disclaimer
Most wallpapers hosted on Salium have been gathered from the wider internet from sites such as [WallpaperCave](https://wallpapercave.com/). Salium and its contributors do not own these images. If your wallpaper is hosted on here and you'd like it removed, please open an issue citing your original work.
