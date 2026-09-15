# ClipperDipper

<img src="logo.png" alt="ClipperDipper" width="120">

**Turn long videos into short captioned clips.**

ClipperDipper is a desktop application for creators. It takes a long video you
already own — a recorded livestream, a podcast, an upload — finds the moments that
work as standalone clips, and renders them as vertical videos with captions burned
in, ready to post.

## What it does

**Finds the good parts.** The video is transcribed on your own machine, then
analyzed to identify segments that stand on their own: a clear hook, a complete
idea, a payoff before the clip ends. Each suggestion comes with a score and the
reason it was chosen, so you decide what actually ships.

**Cuts and captions automatically.** Clips are rendered at 1080x1920 for vertical
feeds, or in landscape and square formats. Captions are generated from word-level
timings and burned in, with the spoken word highlighted as it is said. When a wide
source is cropped to a vertical frame, the crop follows the speaker rather than
blindly centering.

**Summarizes long videos.** A separate mode writes a voiceover script for a long
video, narrates it with a local text-to-speech voice, and lays it over the footage
each line refers to.

**Publishes when you tell it to.** Connect a TikTok, YouTube, or Instagram account
and upload a finished clip directly. Nothing is ever posted automatically — you
pick a clip and confirm it.

## How it works

Everything heavy runs locally. Speech-to-text and voice synthesis happen on your
own computer, and source videos and rendered clips never leave it. The only text
sent anywhere is the transcript, which goes to Anthropic's API so a model can
judge which moments are worth clipping.

Accounts are connected through each platform's standard authorization flow. Access
tokens are stored in your operating system's keychain.

## Platform

macOS desktop application. Runs as a local app with a browser-based interface and a
command line, both on your own machine.

## Legal

- [Terms of Service](terms-of-service)
- [Privacy Policy](privacy-policy)

ClipperDipper is not affiliated with, endorsed by, or sponsored by TikTok,
ByteDance, YouTube, Google, Instagram, or Meta.
