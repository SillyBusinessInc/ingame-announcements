# ingame-announcements
This repo is used to host our in-game announcements that do not need a steam announcement, but we still want to showcase in game.

## To get an announcement in-game:
Edit announcement.json and opy/paste the below object into the newsitems list.
Preferably add to the top, as there is no sorting. So read from top to bottom.

```json
      {
        "title": "Sideloaded 1",
        "url": "https://google.com",
        "author": "sillybusinessstudios",
        "contents": "[img]{EXTERNAL_IMG_HOST}discordBanner.png[/img]",
      }
```
- Edit title, not used ingame but makes it easier to keep track of the announcements.
- Edit url, this is the link the user goes to when clicking the announcement in-game.
- Edit contents, this is largely ignored as we only look for the first \[img] tag.

## How to get the right image link
1) place image in the `/images/`-folder.
2) go to that image in browser, and rightclick > "open image in new tab"
3) url of image is now in your url bar, you take everything after `https://raw.githubusercontent.com/SillyBusinessInc/ingame-announcements/refs/heads/main/images/`
4) paste this url in the contents: `[img]{EXTERNAL_IMG_HOST}<COPIED LINK HERE>[/img]`
