---
title: Support
---

# Support

## Getting started

1. Click the ChatReact icon in your browser toolbar and choose **Connect Twitch**.
2. Open **Settings** from the same menu to write your message. Use the placeholders `{tab.title}`, `{tab.url}`, `{tab.domain}`, and `{channel}`. The preview shows exactly what will be sent.
3. Go to any page and press the ChatReact shortcut. The message appears in your chat and is pinned.

The shortcut only works while your browser window is focused.

## The toolbar badge

| Badge | Meaning |
|---|---|
| ✓ | The message was sent and pinned. |
| ! | Something went wrong. Hover over the icon to see why. |
| AUTH | Your Twitch login needs renewing. Open the ChatReact menu and click **Reconnect**. |
| OFF | ChatReact is switched off. Right-click the icon and tick **Enabled**. |

## Common problems

**The shortcut does nothing.**
- Check that the badge doesn't say OFF.
- Open the shortcut page (in Chrome: `chrome://extensions/shortcuts`) and make sure ChatReact has one. If another extension already uses the default, ChatReact's shortcut is left empty and you need to choose a different one.
- Shortcuts must include Ctrl or Alt.

**"Connect Twitch first."** Open the ChatReact menu and connect your account.

**"Message too long even after shortening."** Twitch allows up to 500 characters. ChatReact first removes tracking parameters from the link, then shortens the page title. If the message is still too long, the link alone or the fixed text in your template is too long. Shorten the template text.

**"Sent, but pinning failed."** The message is in your chat but couldn't be pinned. ChatReact retries for up to 15 seconds and never posts the message twice. You can pin it by hand from Twitch chat.

**"Twitch dropped the message."** Twitch blocked the message, for example because of your channel's AutoMod or blocked-terms settings. Hover over the icon to see the reason Twitch gave.

**The message showed up in other channels.** Your channel is in a Twitch Shared Chat session, and Twitch shows messages in every channel in the session.

## Disconnecting

Click **Disconnect** in the ChatReact menu. ChatReact deletes your Twitch token and asks Twitch to revoke it. To be thorough, you can also remove ChatReact under **Connections** in your Twitch settings.

## Contact

Found a bug or have a question? Open an issue at [github.com/DesertIce/chatreact-docs/issues](https://github.com/DesertIce/chatreact-docs/issues). Please say which browser you use and what the badge showed. Never include your Twitch password or tokens.
