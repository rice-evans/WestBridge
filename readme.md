# Roleplay Utility Assistant

A sleek, minimalist, no-color dashboard featuring a rounded GUI layout built exclusively to assist in EMS, Fire, and LEO roleplay scenarios.

## Features
- **Timezone-Adjustable Clock**: Dynamically updates and toggles between Local, UTC, EST, PST, and GMT.
- **Light/Dark Mode**: Minimalist themes without color clutter.
- **Modular Data System**: Powered entirely by a single inline JSON structure, making edits incredibly easy.

## How to add Subpages
Open `index.html`, scroll down to the `<script>` tag, and find the `siteConfig` object. 

To add a new subpage, simply insert a new `"Key": "Value"` pair under your desired department section:

```javascript
LEO: {
    "Equipment": "...",
    "Miranda Rights": "...",
    "Your New Subpage": "Put your text instructions or content guidelines here."
}
## How to add Dividers inside Subpages
To break up a single subpage into clean, structured sections, just type `---` on a line by itself anywhere in your text. 

Example configuration style:
```javascript
"Your Subpage": "This is section one text.\n• Item A\n---\nThis text appears below the divider line.\n• Item B"

## Subheadings & Formatting Layout Rules

1. **Auto-Header Divider**: The application automatically places a master divider line right beneath the tab title (`EMS - Equipment`), you don't need to manually type one at the top.
2. **Adding Section Dividers**: Place three dashes (`---`) on its own line to slice content categories.
3. **Adding Subheadings**: Directly below a custom divider (or anywhere in text), type `### ` followed by your heading title.

Example Syntax:
```javascript
"Subpage Title": "Standard information string goes here.\n---\n### Your Subheading Title\n• Next section details."
