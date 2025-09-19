# MakeCode Skill Map Sample

This is an example skill map that contains three separate learning paths.You can view the content here:
https://arcade.makecode.com/skillmap#github:microsoft/pxt-skillmap-sample/skillmap.md

Github-hosted skill maps are loaded in the same manner as tutorials, with a URL fragment
formatted as follows:

`#github:[organization name]/[repository name]/[markdown file name]`

## Syntax

The skill map definition can be found in the `skillmap.md` file. Metadata about the skill
map itself can be found under the top-level heading:

- `id`: The string after the heading (eg `# sample`). Cannot contain spaces.
- `name`: The title of your skill map. This will be displayed in the banner on the page.
- `description`: A description of the map contents. This is also shown in the banner.
- `infoUrl` (optional): A URL to a page with additional educator information
- `backgroundurl` (optional): URL to a background image for the entire skill map
- `bannerurl` (optional): URL to a banner image displayed in the sidebar panel

### Learning Paths

A skill map consists of one or more "paths", each path being an ordered sequence of activities.
The first activity in each path is unlocked, and completing an activity unlocks the next one.

A learning path is defined by a level two heading (`##`) has has the following properties:

- `id`: The string after the heading (eg `## interface`). Must be unique within this skill map.
- `name`: The title of the path, displayed above the linked activities.
- `description`: Additional details (not currently displayed).
- `completionUrl`: URL to a certificate, displayed when a user has completed the entire path.

### Activities

Each learning path has multiple activities, defined by level three headings (`###`). Currently,
an "activity" is simply a MakeCode tutorial, and has the following properties:

- `id`: The string after the heading (eg `### space-activity1`). Must be unique within this skill map.
- `name`: The title of the activity. Displayed on the activity card.
- `type`: The type of activity. Must be `tutorial` currently.
- `description`: Details about the activity, displayed on the back of the card.
- `tags`: Descriptive tags displayed on the bottom of the activity card.
- `url`: Link to the tutorial. See the [MakeCode Tutorial Documentation](https://makecode.com/writing-docs/user-tutorials) for details on tutorial authoring and link formatting.
- `imageUrl`: URL for the image displayed on the front of the activity card.

## Background Images and Pages

This repository supports two types of background content for skill maps:

### Background Images
Background images provide visual theming for your skill maps. Place image files (PNG, JPG, GIF) in the `/img/backgrounds/` directory:

```
/img/backgrounds/
├── space/
│   ├── space-background.png
│   └── space-banner.png
├── platformer/
│   └── platformer-bg.jpg
└── general/
    └── coding-background.png
```

Reference them in your skill map using:
```markdown
# my-skillmap
* backgroundurl: /img/backgrounds/space/space-background.png
* bannerurl: /img/backgrounds/space/space-banner.png
```

**Image Guidelines:**
- **Background images**: Should be subtle/low contrast (1920x1080px recommended)
- **Banner images**: Can be more detailed (400x200px recommended)  
- **File size**: Keep under 500KB for good performance
- **Accessibility**: Ensure skill map nodes remain visible over background

### Background Pages
Background pages are markdown files that provide educational context. Place them in the `/backgrounds/` directory:

```
/backgrounds/
├── space-explorer.md
├── beginner-gamedev.md
└── README.md
```

These are separate from background images and are used for additional educational content that can be referenced from skill maps.

### Example Usage
```markdown
# space-explorer
* name: Space Explorer Journey
* description: Build amazing space games!
* backgroundurl: /img/backgrounds/space/nebula-background.png
* bannerurl: /img/backgrounds/space/spacecraft-banner.png
* primarycolor: #2EA9B0
* secondarycolor: #F392BD
```

## Forking

If you fork this repo, be sure to change all URL references to https://github.com/microsoft/pxt-skillmap-sample to your forked repo's URL. Otherwise you won't see your changes.

## Contributing

This project welcomes contributions and suggestions.  Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.

When you submit a pull request, a CLA bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.

## Trademarks

This project may contain trademarks or logos for projects, products, or services. Authorized use of Microsoft
trademarks or logos is subject to and must follow
[Microsoft's Trademark & Brand Guidelines](https://www.microsoft.com/en-us/legal/intellectualproperty/trademarks/usage/general).
Use of Microsoft trademarks or logos in modified versions of this project must not cause confusion or imply Microsoft sponsorship.
Any use of third-party trademarks or logos are subject to those third-party's policies.
