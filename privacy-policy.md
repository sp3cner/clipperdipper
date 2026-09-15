# Privacy Policy for ClipperDipper

**Effective date:** 15 September 2026

ClipperDipper ("the app") is a desktop application that runs entirely on your own
computer. There is no ClipperDipper server, no account to create with us, and no
analytics or telemetry of any kind.

This policy explains exactly what happens to your data.

## What we collect

**Nothing.** The developer of ClipperDipper operates no servers and receives no
data from the app. We cannot see your videos, your transcripts, your TikTok
account, or the fact that you are using the app at all.

## What stays on your computer

All of the following are written to disk on your own machine and never leave it
unless you explicitly choose to publish a video:

- Source videos you provide or download
- Audio extracted from those videos for transcription
- Transcripts, including word-level timings
- Rendered clips and summary videos
- Cached data used to avoid repeating work

Speech-to-text runs locally using the Whisper model. Audio is **not** sent to any
transcription service. Text-to-speech for narrated summaries also runs locally.

## What is sent to third parties, and when

The app contacts outside services only in these situations.

**1. Anthropic (Claude API) — when you generate clips or summaries**

The **text of your transcript** is sent to Anthropic's API so the model can
identify interesting moments or write a summary script. Video and audio are never
sent — only text. This happens only when you start a clipping or summarizing job.
Anthropic's handling of that data is governed by their own privacy policy at
https://www.anthropic.com/legal/privacy

You supply your own Anthropic API key. It is read from a local configuration file
and is never transmitted anywhere except to Anthropic.

**2. Video platforms — when you download a source video**

If you paste a link, the app requests that video from the platform hosting it
(for example YouTube, Twitch, or Kick), exactly as a browser would.

**3. TikTok, YouTube, or Instagram — when you publish**

When you select a clip and choose to publish it, the app uploads that video file,
its title, and its description to the platform you selected, using credentials you
authorized. Nothing is uploaded automatically. Every upload requires you to select
a specific clip and confirm the action.

## Credentials and tokens

When you connect a TikTok, YouTube, or Instagram account, the platform returns an
access token. That token is stored **in your operating system's keychain**
(the macOS Keychain), or, where a keychain is unavailable, in a file readable only
by your user account.

Tokens are used solely to upload videos you have selected and to display which
account is connected. They are never transmitted to the developer or to any party
other than the platform that issued them.

## What we do with your TikTok data

If you connect a TikTok account, the app requests two permissions:

- `user.info.basic` — used only to show your display name in the interface, so you
  can confirm which account you are about to post to.
- `video.upload` — used only to send a clip you selected to your own TikTok inbox
  as a draft.

The app does not read your videos, your followers, your analytics, or any other
account data. It does not post publicly on your behalf; uploaded clips arrive as
drafts that you review and publish yourself in the TikTok app.

## Deleting your data

Because nothing is stored remotely, deleting your data means deleting local files:

- Remove the app's `output/`, `downloads/`, and `.cache/` directories
- Disconnect any connected account in the app, which deletes its stored token
- Revoke the app's access in the platform's own settings (for TikTok: Settings →
  Security and permissions → Manage app permissions)

## Children

ClipperDipper is not directed at children and is not intended for use by anyone
under 13.

## Changes

If this policy changes, the effective date above will be updated.

## Contact

Questions about this policy: **[YOUR EMAIL ADDRESS]**
