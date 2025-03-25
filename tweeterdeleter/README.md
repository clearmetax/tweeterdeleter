# tweeterdeleter

A powerful userscript that helps you manage your X/Twitter account by providing tools to delete tweets, direct messages, favorites, and manage follows - all for free.

## Features

- **Delete Tweets**: Remove all your tweets using your Twitter data export
- **Delete Direct Messages**: Remove DMs using your Twitter data export
- **Remove Favorites/Likes**: Unlike tweets using your Twitter data export
- **Export Bookmarks**: Save your bookmarks before deleting them
- **Unfollow Everyone**: Mass unfollow feature to clean up your following list
- **Rate Limit Handling**: Automatically handles Twitter's rate limits
- **Progress Tracking**: Visual progress bar and status updates
- **Skip Option**: Ability to skip older tweets during deletion

## Installation

1. Install a userscript manager for your browser:
   - [Tampermonkey](https://www.tampermonkey.net/) (recommended)
   - [Greasemonkey](https://addons.mozilla.org/en-US/firefox/addon/greasemonkey/)
   - [Violentmonkey](https://violentmonkey.github.io/)

2. Install tweeterdeleter:
   - Visit [Greasy Fork](https://update.greasyfork.org/scripts/476062/tweeterdeleter.user.js)
   - Click "Install"
   - Your userscript manager will prompt you to confirm the installation

## Usage

### Deleting Tweets

1. Request your Twitter data export from Twitter settings
2. Once you receive the export, extract the `tweet-headers.js` file
3. Visit your Twitter profile
4. Click the tweeterdeleter interface at the top of the page
5. Upload your `tweet-headers.js` file
6. Wait for the deletion process to complete

### Deleting Direct Messages

1. Use the `direct-message-headers.js` or `direct-message-group-headers.js` from your Twitter data export
2. Follow the same steps as tweet deletion

### Removing Favorites

1. Use the `like.js` file from your Twitter data export
2. Follow the same steps as tweet deletion
3. Note: This only works for the most recent few thousand likes

### Exporting Bookmarks

1. Click "Advanced Options" in the tweeterdeleter interface
2. Click "Export Bookmarks"
3. Wait for the export to complete
4. Download the JSON file when prompted

### Unfollowing Everyone

1. Click "Advanced Options" in the tweeterdeleter interface
2. Click "Unfollow everyone"
3. Wait for the process to complete

## Advanced Options

- **Skip Count**: Enter a number to skip older tweets during deletion
- **Slow Delete**: Alternative deletion method that doesn't require data export (slower and less reliable)

## Rate Limits

- Tweets: 10,000 - 20,000 per hour
- Direct Messages: ~800 per 15 minutes
- Favorites: 500 per 15 minutes
- Unfollows: Rate limited by Twitter's API

## Troubleshooting

- If the interface doesn't appear, refresh the page
- If deletion stops, check the console for error messages
- For rate limit errors, the script will automatically wait and resume
- If you encounter issues, try the "Slow delete" option in Advanced Options

## Support

For issues or feature requests, please visit the [GitHub issues page](https://github.com/clearmetax/tweeterdeleter/issues).

## License

This project is licensed under the NoHarm draft license.

## Credits

Created by @clearmetax, with contributions from:
- dbort
- pReya
- Micolithe
- STrRedWolf

## Version

Current version: 0.9.3 