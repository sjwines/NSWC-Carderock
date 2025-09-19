# Background Images for Skill Maps

This directory contains background images that can be used for skill map backgrounds and banners.

## Usage

Background images are referenced in skill map definitions using the `backgroundurl` and `bannerurl` properties:

```markdown
# my-skillmap
* name: My Amazing Skill Map
* description: Learn awesome programming skills!
* backgroundurl: /img/backgrounds/my-background.png
* bannerurl: /img/backgrounds/my-banner.png
```

## Image Requirements

### Background Images (`backgroundurl`)
- **Purpose**: Full background image displayed behind the entire skill map
- **Recommended size**: 1920x1080px or similar widescreen ratio
- **Format**: PNG, JPG, or GIF
- **Style**: Should be subtle/low contrast to not interfere with skill map nodes

### Banner Images (`bannerurl`)
- **Purpose**: Displayed in the sidebar panel when no specific activity is selected
- **Recommended size**: 400x200px or similar 2:1 ratio
- **Format**: PNG, JPG, or GIF
- **Style**: Can be more detailed since it's displayed in a dedicated panel

## Organization

Organize images by theme or skill map:

```
backgrounds/
├── space/
│   ├── space-background.png
│   └── space-banner.png
├── platformer/
│   ├── platformer-background.jpg
│   └── platformer-banner.png
└── general/
    ├── coding-background.png
    └── makecode-banner.png
```

## Examples

### Simple skill map with background
```markdown
# beginner-coding
* name: Beginner Coding Adventure
* backgroundurl: /img/backgrounds/general/coding-background.png
```

### Full skill map with background and banner
```markdown
# space-explorer
* name: Space Explorer Journey
* description: Build amazing space games!
* backgroundurl: /img/backgrounds/space/space-background.png
* bannerurl: /img/backgrounds/space/space-banner.png
* primarycolor: #2EA9B0
* secondarycolor: #F392BD
```

## Tips

1. **Keep file sizes reasonable** - Optimize images for web use (under 500KB recommended)
2. **Use descriptive names** - Include the skill map theme in the filename
3. **Test accessibility** - Ensure text/nodes remain readable over your background
4. **Consider themes** - Match your background to the skill map content theme