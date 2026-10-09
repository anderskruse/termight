---
layout: page
title: Privacy policy
permalink: /privacy/
---

Effective 6 October 2026

Termight is an iPhone app developed by Anders Kruse, Denmark. This policy describes what happens to your data when you use it.

Contact: [termight.app@gmail.com](mailto:termight.app@gmail.com)

## Summary

The developer of Termight does not collect, store or sell your personal data. The app has no analytics, no advertising and no tracking. It connects your phone to your own GitHub account and your own codespaces, and what you do there stays between you, GitHub and the services you choose to use.

## What stays on your phone

- **GitHub access tokens.** They are stored in the iOS Keychain, for this device only.
- **Settings.** Appearance, your default agent, saved terminal commands, and the address and model name of a custom endpoint if you set one.
- **Agent sessions.** The list of your sessions and their transcripts are saved in the app's own storage so you can reopen them.
- **Sign-in cookies.** When you sign in to an AI provider inside the app, that provider's cookies are kept in the app's browser storage.

None of this is sent to the developer. Your settings, sessions and sign-in cookies are included in the backups you make of your own phone. The GitHub tokens are not: they stay on the device they were saved on, and on a new or restored phone you sign in again.

## What leaves your phone, and where it goes

**GitHub.** The app talks directly to GitHub to sign you in, list your repositories and codespaces, and start, stop and create codespaces. Your terminal input and output, the files you open and edit, and your agent conversations travel between your phone and your codespace over an encrypted connection through GitHub's Codespaces infrastructure, which GitHub and Microsoft operate. GitHub's handling of your data is described in the [GitHub Privacy Statement](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement).

**The sign-in helper.** When you choose "Sign in with GitHub", GitHub gives the app a one-time code. The app sends that code to a small service run by the developer on Cloudflare, which adds the app's credentials and passes the request on to GitHub. GitHub's answer, your access token, is passed straight back to your phone. The service handles the code and the token only for the moment the request takes. It does not log them or store them. Cloudflare, as the hosting provider, processes the request and with it your IP address, as any web host does.

If you sign in with a personal access token instead, the token goes only to GitHub.

**API keys for AI providers.** If you enter an API key, the app encrypts the key on your phone and saves it as a GitHub Codespaces secret in your own GitHub account. The key is not kept on your phone and is never sent to the developer.

**Signing in with a Claude subscription.** If you sign in to Claude from the app, the token Claude issues is stored in your codespace, so that the codespace is signed in: in a file in your home directory there (`~/.codescape/claude-oauth-token`) and in your shell startup files, which load it. It stays there until you remove it under Settings → Providers → Claude Subscription, or until the codespace is rebuilt or deleted. If you choose to remember it for new codespaces, it is also saved as a GitHub Codespaces secret in your own GitHub account. The token is not kept on your phone and is never sent to the developer.

**AI providers.** When you run a coding agent, the agent runs inside your codespace. Your prompts, and the files and command output the agent reads, are sent from your codespace to the AI provider you chose (for example Anthropic, OpenAI, OpenRouter or a custom endpoint), under your own account or API key with that provider. The provider's own privacy policy applies. Agents may also keep their own history inside your codespace.

**Apple.** If you have agreed on your device to share analytics with app developers, Apple may give the developer anonymous crash and usage statistics. You control this in Settings → Privacy & Security → Analytics & Improvements.

## Sharing

The developer has no personal data from the app to share and shares none.

## Removing your data

- **Sign out** in Settings. This deletes the GitHub tokens from your phone. Do this before deleting the app, because iOS can keep Keychain items after an app is removed.
- **Revoke the app's access** at [github.com/settings/applications](https://github.com/settings/applications). After that the app can no longer reach your GitHub account.
- **Delete saved API keys** on GitHub under Settings → Codespaces → Secrets, or from the app's Settings.
- **Remove a Claude sign-in from a codespace** under Settings → Providers → Claude Subscription in the app. This deletes the token stored in that codespace. It does not cancel the token itself.
- **Delete the app** to remove its settings, session lists and transcripts from your phone.
- **Delete your codespaces** on GitHub to remove what is stored in them.

## Your rights

If you write to the contact address, your email is kept only as long as needed to answer you. You can ask to see, correct or delete it at any time. Under the EU General Data Protection Regulation you also have the right to complain to a data protection authority; in Denmark that is Datatilsynet.

## Children

Termight is a tool for software developers and is not directed at children. GitHub requires its users to be at least 13 years old.

## Changes

If this policy changes, the new version will be published on this page with a new date.
