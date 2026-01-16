# fm-dx-webserver-popup-plugin

Popup plugin for FM-DX Webserver that shows a one-time notice modal on the frontend.

## What it does
- Injects a modal popup on page load with configurable text.
- Uses the FM-DX Webserver theme variables for colors.
- Dismisses on button click or overlay click.

## Files
- `popup.js` - plugin manifest used by the server to register the frontend script.
- `popup/frontend.js` - frontend code that injects styles and renders the popup.

## Configuration
Edit the message in `popup/frontend.js`:

```js
var popupTitle = 'Announcement';
var popupText = 'Your message here.';
```

Use `<br>` tags for line breaks if needed.

## Install
1. Copy this plugin folder into your FM-DX Webserver plugins directory.
2. Restart or reload the server so it loads the plugin.

## Development
The popup is purely frontend; backend hooks are not used.

## License
GNU GPL v3. See `LICENSE`.
