# Discord Web Auto Quest Extension

## What it does

This extension hooks into Discord's quest system and automatically completes the requirements for all active quests sequentially. It works with:

- Video watching quests (WATCH_VIDEO, WATCH_VIDEO_ON_MOBILE)
- Desktop game playing (PLAY_ON_DESKTOP) 
- Desktop streaming (STREAM_ON_DESKTOP)
- Activity playing (PLAY_ACTIVITY)

The extension spoofs your user-agent to make Discord think you're using the desktop app, which is required for some quest types to work properly. Supports sequential quest execution to ensure stability and proper completion.

## Installation

1. Clone or download this repo
2. Open Chrome/Edge and go to `chrome://extensions/`
3. Toggle "Developer mode" on (top right corner)
4. Click "Load unpacked" and select the extension folder
5. You're done!

## How to use

1. Go to `https://discord.com/quest-home` in your browser
2. Accept quests if you haven't already
3. Look for the "Running Quests" button in the bottom right corner with a Symbol icon
4. Click it and check the browser console (F12) for progress updates
5. Expand the panel to see quest details (shows Discord ID and credits)

The extension will automatically detect all your active quests and start completing them one by one. Progress is logged to the console so you can see what's happening for each quest.

