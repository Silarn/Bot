# Wave Bot
Fork from PlaceDE Bot. Thanks guys!  
The bot for The Wave! This bot automatically fetches [plans](https://github.com/Silarn/pixel) every few minutes to prevent bots from colliding with each other.

## Installation instructions

Check that new pixels can be placed and this is not on cooldown

1. Install the browser extension [Tampermonkey](https://www.tampermonkey.net/) or [Violentmonkey (Firefox)](https://addons.mozilla.org/en-US/firefox/addon/violentmonkey/).
2. Install the browser extension [CORS Unblock](https://chrome.google.com/webstore/detail/cors-unblock/lfhmikememgdcahcdlaciloancbhjino/related?hl=en) or [for Firefox](https://addons.mozilla.org/en-US/firefox/addon/cors-unblock/)
3. Click on this link: [https://github.com/Silarn/Bot/raw/main/placewavebot.user.js](https://github.com/Silarn/Bot/raw/main/placewavebot.user.js). If all goes well, Tampermonkey will offer to install a user script. Click **Install**.
4. In your **r/place** tab, make sure to toggle on the CORS Unblock extension -> ![cors.png](cors.png)
5. Reload the **r/place** tab. If all went well, you should see "Ask for access token..." at the top right of the screen. The bot is now active and will use these notifications at the top right for ongoing information.

## Bot weaknesses

- The bot doesn't update the cooldown message, so it looks like there's still a pixel to place. However, the bot has already placed the pixel and is now waiting for the cooldown.
- The bot doesn't take into account an existing cooldown and therefore assumes that you can place a pixel immediately when you open **r/place**. In the worst case, 5 minutes are lost
