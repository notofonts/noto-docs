# Contribute to Noto fonts

## How you can help with Noto

You can help with the Noto development in several ways:

- **Test** the fonts in various documents, especially with rare but sensible letter combinations in the script that you know natively. If you find unwanted letter clashes, wrong forms, or any other kind of problem or defect with any Noto font, [open an issue](#open-an-issue-to-report-a-problem).

- You may **extend** or **customize** Noto fonts for your own project, website or app. You don’t need to ask our permission, but you need to follow the terms of the [Open Font License (OFL)](https://scripts.sil.org/OFL). Learn more about the terms in the [OFL FAQ](https://scripts.sil.org/ofl-faq_web).

- If you’d like Google Fonts to **incorporate** your extensions or changes into an official Noto font, or if you’d like to contribute a design for a script for which a Noto font does not exist yet, read how to [propose changes](#propose-changes).

## Before you open an issue or propose changes

### How are Noto fonts developed?

Noto fonts for each script are developed in a collaborative approach. Google Fonts provides the direction, planning, and final aesthetic decisions. The team works with font foundries and designers to create requirements for each script and language. This results in design proposals that are vetted by expert reviewers and, when available, by native readers of the script.

Type designers and font developers create the fonts in several cycles, along with a review at each step. The duration of the process depends on the complexity of the script and on availability of the reviewers and other resources. Finally, a technical review of the fonts is made. Google Fonts then publishes the font sources and uses an open source tool chain to build the fonts in various formats.

The Noto project is an ambitious undertaking: 2,300 fonts in over 200 font families to support more than 150 scripts. The Fonts team aims to make each Noto font aesthetically pleasing and typographically correct. But, just like with any software project, there will be issues that need to be addressed over time.

### On what basis does Noto include glyphs?

The Noto project provides default glyphs for scripts as defined in the Unicode Standard. Noto fonts have glyph designs that are suitable for the widest audience.

Noto currently has at least one font style for all basic characters of the Unicode Standard version 12, released in 2019. For Chinese, Japanese and Korean (CJK) languages, Noto has characters included in the Basic Multilingual Plane (BMP) of the Unicode Standard. More than 25 scripts have both Sans and Serif families and many have multiple weights and widths.

If some languages or writing conventions prefer an alternate shape, Noto fonts may provide the shape as a localized form (the OpenType locl feature) or stylistic alternate (salt, ssXX). Ligatures that are widely accepted are includes as standard ligatures (liga feature). Noto fonts may also provide discretionary ligatures (dlig) for more specialized use.

The Noto team reserves the right to make the specific choices. If you are unhappy with a particular choice, you may create and distribute a modified variant of the the font according to the Open Font License.

### Is it the font, is it the app?

For many scripts, Noto fonts use advanced typographic features that include “shaping” rules that allow accurate, orthographically correct rendering of text.

Browsers and word processing apps typically support shaping for all scripts. But many apps, especially older versions of graphic design apps, don’t support shaping for all scripts. A given version of the app and system supports a particular version of the Unicode Standard. Some apps only support an older version of Unicode and cannot correctly render text in scripts that were recently added to the Unicode Standard.

When you notice a problem with a Noto font in a particular app or system, first check if the same problem occurs with another vendor’s font for the same script. If this is so, then likely it’s not a Noto problem but the problem of the app or system. Check the most recent version of the app or system to see if the problem persists. Ideally, test with several different apps and systems. Compare the current version of the Noto font with an older version of the same font.

## Open an issue to report a problem

### Before you open an issue

The Google Fonts team uses GitHub to develop Noto. GitHub is a popular platform used for collaborative software development by thousands of open-source projects. If you haven’t used GitHub before, [sign up](https://github.com/join) to create an account.

Google Fonts uses several GitHub repositories to store Noto project files. The issue tracker in each repository is like a forum where you can report a problem (defect, bug). The Fonts team will respond to the issue, and you can monitor the discussion and comment. When the problem is resolved, one of the Team members will close the issue.

If you think that there is a problem with a Noto font itself, open an issue in the suitable repository.

Give the issue a brief but clear title. Please use English and be polite.

Describe the problem in detail. Paste the relevant text where the problem occurs. Attach screenshots and images that illustrate the problem, and annotate them. Include the name and version of the app and operating system where the problem is visible.

Since Noto is available in many places, when you report a problem with a particular font, tell us where the font came from, and the font version. You can attach a ZIP with the font file to the issue.

### How to open an issue

- To report a problem with any Noto font except CJK and emoji, [open an issue](https://github.com/googlefonts/noto-fonts/issues) in the [noto-fonts](https://github.com/googlefonts/noto-fonts/) repository.

- To report a problem with Noto Sans CJK or Noto Serif CJK (SC, TC, JP, KR, HK), [open an issue](https://github.com/googlefonts/noto-cjk/issues) in the [noto-cjk](https://github.com/googlefonts/noto-cjk/) repository.

- To report a problem with Noto Color Emoji or Noto Emoji, or with the tools used to build these fonts, [open an issue](https://github.com/googlefonts/noto-emoji/issues) in the [noto-emoji](https://github.com/googlefonts/noto-emoji/) repository.

- To report a problem with the tools used to build the non-emoji Noto fonts, [open an issue](https://github.com/googlefonts/nototools/issues) in the [nototools](https://github.com/googlefonts/nototools/) repository.

## Propose changes

You may extend or customize Noto fonts for your own project, website or app, and you may publish the customized fonts in accordance with the [Open Font License](https://github.com/googlefonts/noto-fonts/blob/main/LICENSE).

You may also propose to Google Fonts that your changes are incorporated into the official Noto release. You can propose a new design for an existing Unicode character (codepoint), or for a new character. You can propose designs for additional weights or widths for an existing script, or even a new design for a Unicode script that Noto does not yet cover.

The most up-to-date source files for all Noto fonts are in the [noto-source](https://github.com/googlefonts/noto-source) repository in the.glyphs format. The final font files are in the [noto-fonts](https://github.com/googlefonts/noto-fonts) repository in the OpenType format. Before proposing changes, check the newest files. Perhaps you’re trying to fix something that’s already been addressed?

The proposed additions need to match the existing designs, be of high quality, and be delivered in the same source format as the existing fonts. If you’re proposing design for new codepoints, those need to already exist in the Unicode Standard. Google Fonts does not accept proposals for scripts that are not part of Unicode.

If there are multiple weights or widths, those need to be variable. The widths, weights, and naming conventions need to be compatible with the rest of the Noto family.

Before you submit your proposal, sign a Google Open Source [Contributor License Agreement](https://cla.developers.google.com/clas) (CLA). Then, submit your proposal to noto-proposals-external@googlegroups.com. For detailed guidelines regarding the proposal, please see the [Noto Contributing Guide](https://github.com/notofonts/noto-docs/blob/main/CONTRIBUTING.md)

As with any maintained open-source project, Google Fonts may accept the proposal, reject it or require additional information.

## Send other feedback

If you’d like to share feedback that is not a problem report, or you’d like to ask about the fonts, visit the [noto-font group](https://groups.google.com/g/noto-font/) or send an email to _noto-font@googlegroups.com_

