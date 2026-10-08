---
title: Privacy policy
---

# Privacy policy

**Effective date:** 3 October 2026

This policy explains what the ChatReact browser extension ("ChatReact", "the extension") does with your information. ChatReact is published by DesertIce ("we", "us"). It applies to every version of the extension: the [Chrome Web Store version](https://chromewebstore.google.com/detail/chatreact/khpihddljmpknjjbjaoioaololfbkaal) (which also runs in other Chromium-based browsers) and the [Firefox version](https://addons.mozilla.org/en-US/firefox/addon/chatreact/). Both handle your information the same way.

## The short version

- ChatReact has **no servers**. We never receive, see, or store your information.
- It talks to **one service only: Twitch**, and only to do what you ask it to do.
- It reads the **title and address of your current tab only when you press its shortcut**, and only to build the chat message you configured.
- There are **no analytics, ads, or tracking**, and **nothing is sold or shared**.

## What the extension handles, and why

| Information | When | Where it's kept | Where it goes |
|---|---|---|---|
| Twitch access token | When you connect your Twitch account | Browser memory only (session storage). Never written to disk. Cleared when the browser closes. | Twitch only, to authorize sending and pinning your messages |
| Twitch username and user ID | When you connect | Browser memory, alongside the token | Twitch only, to identify your channel |
| Title and address of the active tab | Only when you press the ChatReact shortcut | Not stored. Used once to build the message. | Twitch only, as the chat message you configured |
| Your settings (message template, link-cleaning choice, pin duration, on/off switch) | When you save them | Your browser's local extension storage | Nowhere. They stay on your device. |
| A "connected" flag (yes or no) | When you connect or disconnect | Your browser's local extension storage | Nowhere. It records whether you chose to stay connected. |

ChatReact does not read page contents, browsing history, keystrokes, other tabs, or anything else.

### Your Twitch connection

ChatReact uses Twitch's standard sign-in page, and your Twitch password is never shared with the extension. It asks Twitch for two permissions:

- **Send chat messages as you** (`user:write:chat`)
- **Manage chat messages in your channel** (`moderator:manage:chat_messages`), which is needed to pin messages

The resulting access token is kept in memory and is never written to disk. ChatReact checks the token with Twitch about once an hour, as Twitch requires, and quietly gets a new one before it expires.

When you click **Disconnect**, ChatReact deletes the token, asks Twitch to revoke it, and stops renewing it. You can also remove ChatReact's access at any time in your Twitch settings under **Connections**.

### Messages you send

The messages ChatReact posts go into your Twitch chat. Like any chat message, they are visible to your viewers and are handled by Twitch under [Twitch's Privacy Notice](https://legal.twitch.com/legal/privacy-notice/). If your channel is in a Twitch **Shared Chat** session, Twitch shows the message in every channel in that session.

The page title and address you share depend on what tab you are on when you press the shortcut, so check before you press it.

## Third parties

ChatReact only communicates with Twitch (`id.twitch.tv` and `api.twitch.tv`). It does not use analytics services, advertising networks, crash reporters, or any other third-party service. We do not sell, rent, or transfer your information to anyone.

## Browser permissions

| Permission | Why ChatReact needs it |
|---|---|
| `activeTab` | To read the current tab's title and address, only when you press the shortcut |
| `identity` | To open Twitch's sign-in page and receive the token |
| `storage` | To keep your settings locally and your token in memory |
| `alarms` | To check the Twitch connection about once an hour |
| `contextMenus` | For the **Enabled** switch when you right-click the toolbar icon |

## Browser store requirements

**Chrome Web Store.** ChatReact's use of information complies with the [Chrome Web Store User Data Policy](https://developer.chrome.com/docs/webstore/program-policies/user-data-faq), including the [Limited Use](https://developer.chrome.com/docs/webstore/program-policies/limited-use) requirements. We use the information above only to provide ChatReact's single purpose: posting and pinning messages in your own Twitch chat. We do not use it for advertising or to determine creditworthiness, and no human reads it.

**Firefox Add-ons.** As Mozilla's add-on policies require, the Firefox version declares the data it transmits in its manifest: authentication information (your Twitch token), browsing activity (the active tab's address), and website content (the active tab's title). All three go only to Twitch, only as described above.

## Keeping and deleting your information

- The Twitch token and your Twitch username and ID stay in memory until you disconnect or close the browser, whichever comes first.
- Tab titles and addresses are not kept after the message is sent.
- Settings stay in your browser until you remove the extension or clear its data. Uninstalling ChatReact deletes all of it.

Because we never receive your information, there is nothing for us to delete on our side. Messages already posted in Twitch chat are controlled by Twitch and your channel's moderation tools.

## Children

ChatReact is meant for Twitch streamers and follows Twitch's own age requirements. It is not directed at children under 13, and we do not knowingly handle children's information.

## Changes to this policy

If ChatReact starts handling information differently, we'll update this page and the effective date before the change is released. Significant changes will also be noted in the extension's release notes.

## Contact

Questions about this policy: open an issue at [github.com/DesertIce/chatreact-docs/issues](https://github.com/DesertIce/chatreact-docs/issues).
