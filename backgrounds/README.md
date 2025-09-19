# Background Pages for Skill Maps

This folder contains background **pages** (markdown content) for skill maps. These provide additional context, information, or educational content that can be linked from skill maps.

## Important Note

⚠️ **This directory is for background PAGES, not background IMAGES**

- **Background images** (PNG, JPG, GIF) should go in `/img/backgrounds/`
- **Background pages** (markdown content) go in this `/backgrounds/` directory

## Structure

Background pages can be organized by topic or theme:
- Add markdown files for background content
- Include any assets or styling information
- Follow the same patterns as other content in the repository

## Usage

Reference background pages in your skill map definitions using relative paths:
```
* backgroundUrl: /backgrounds/[page-name].md
```

For background images, use:
```
* backgroundurl: /img/backgrounds/my-image.png
* bannerurl: /img/backgrounds/my-banner.png
```

## Examples

- Educational context pages (like `space-explorer.md`)
- Themed backgrounds for different skill paths  
- Visual styling guides
- Additional resources and information

## See Also

- For background **images**, see: `/img/backgrounds/README.md`
- For skill map documentation, see: `README.md` in the root directory