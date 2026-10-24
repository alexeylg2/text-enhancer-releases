# Text Enhancer — builds

Text Enhancer is a macOS menu bar app: select text in any app, press ⌘T and pick a style to fix mistakes,
rewrite it in a business tone, translate it, or answer a customer from your knowledge base.
It works with LM Studio (local), Claude, OpenAI, DeepSeek and DeepL.

This repository contains ready-to-install builds only; the source code lives elsewhere.

## Download

**[Latest version — Text-Enhancer.zip](https://github.com/alexeylg2/text-enhancer-releases/releases/latest/download/Text-Enhancer.zip)**

Requires macOS 14 Sonoma or later on Apple Silicon or Intel. All versions and changelogs are in
[Releases](https://github.com/alexeylg2/text-enhancer-releases/releases).

## Install

1. Unzip the archive and drag “Text Enhancer.app” to Applications.
2. Open the app. macOS will say it can't verify the developer because the build isn't notarized by Apple.
   Go to System Settings → Privacy & Security and click **Open Anyway**, or run in Terminal:
   ```bash
   xattr -dr com.apple.quarantine "/Applications/Text Enhancer.app"
   ```
3. Turn on Text Enhancer in System Settings → Privacy & Security → Accessibility,
   and enter your API keys in the app's Settings → Models. Keys are stored only in your Mac's Keychain.

## Update

Starting with version 0.5.0 (18), the app checks for new releases at launch and once a day.
When one is available, click **Update to …** in Settings → General or in the menu bar menu:
the app downloads the new version, installs it and relaunches. Your settings, styles, API keys
and Accessibility permission are kept, and there is no Gatekeeper prompt.

Older versions have to be updated once by hand: quit the app (menu bar icon → Quit) and repeat the install steps.
