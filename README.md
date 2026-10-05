# WhatsApp Turbo

A Windows desktop beta app that wraps the real WhatsApp Web and adds the power features
WhatsApp never gave you — as buttons in the UI, not chat commands.

> Unofficial community software. Not affiliated with, endorsed by, or connected to
> WhatsApp or Meta in any way.

**Current access:** Windows beta with self-service Google sign-in / sign-up. Your first Google sign-in automatically creates an enabled Turbo account; existing users sign in with the same Google account. WhatsApp linking is a separate step. Administrators can suspend access, sign out devices and require a minimum app version. Online clients check access every five minutes; cached access lasts at most24 hours after successful verification while offline.

## What it does

- **Send later** — right-click WhatsApp's own Send button (or any chat) to schedule a
  message; it sends at the time you picked, with status shown right in the chat.
- **Follow-ups** — send now, get a reminder if nobody replies within N minutes/hours/days.
- **Chat snooze** — mark a chat for later until a set time, "until tomorrow
  09:00", or until they reply.
- **Multiple WhatsApp accounts** side by side (personal + work), each with its own
  message popups and sounds.
- **Turbo notifications** — per-account Windows toasts with the account name and thread,
  even when the app is in the tray.
- **Bulk chat actions** — select many chats and mark read / snooze / follow up at once.
- **Thread summary / Ask this chat** (optional) — summarize a long thread or draft a
  follow-up using your own OpenAI-compatible API key. Selected chat content and the key
  are sent to the AI provider you configure.

## Download

1. Download the current Windows Setup from [Releases](../../releases).
2. Download **WhatsApp-Turbo-Setup-x.y.z.exe** (recommended — installs like any Windows
   app, no admin rights needed) or **WhatsApp-Turbo-Portable-x.y.z.exe** (single file,
   no installation).
3. Run it, sign in or sign up with Google, then scan the QR code with
   your phone (WhatsApp → Linked devices). Existing linked sessions and local data are
   retained when upgrading with Setup. Portable upgrades are manual.

**Requirements:** Windows 10/11 64-bit.

**SmartScreen:** the app is unsigned, so Windows may show "Windows protected your PC".
Click *More info → Run anyway*. Building trust (code signing) may come later.

## Privacy

- Scheduled messages, notes, settings, logs and your WhatsApp linked-device session are
  stored locally. Turbo's access service stores your Google identity/email, device identifier
  and name, app version, session/access state and administrator actions. Chat content and
  private notes are not sent to that access service.
- The AI features are optional and use **your own** API key, stored locally and sent only
  to the AI provider you configure.
- Your WhatsApp session is a normal "linked device" session, like WhatsApp Desktop.

## Safety defaults (please read)

- Scheduled messages are sent automatically at their time. You can turn automation off
  per account in the account flyout.
- The app enforces send pacing (minimum gaps, hourly/daily caps) and a warm-up period
  after linking a device, because aggressive automated sending can get WhatsApp accounts
  flagged or banned.
- **Use with care:** automating WhatsApp may violate WhatsApp's Terms of Service. You
  are responsible for how you use it. This software is provided as-is, with no warranty.

## License

[MIT](LICENSE) — free to use, modify and share.
