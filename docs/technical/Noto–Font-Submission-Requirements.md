---
layout: default
title: "Submissions"
parent: "Technical"
nav_order: 210
---
# Noto Font Submission Requirements

{:toc}

### Objective of This Document

This document gathers all the requirements and steps that are necessary to submit a font that _could_ become part of a Noto family of fonts.

### Process

1. Prepare your script proposal. If you're proposing to add or replace new codepoints to an existing font or a new script, you need to make a proposal.

2. Submit it to noto-proposals-external@googlegroups.com (needed: review process)

3. The review process team might approve or reject the proposal or require additional information.

4. Any approved scripts need to meet the requirements listed in the New Font Delivery Requirements and Additions to an existing Font Delivery Requirements sections below.

### Gates

1. Noto font design proposal review.

2. If applicable, Noto font weight and width design proposal review.

3. Noto font technical review after the first version of the font is produced.

### New Font Delivery Requirements

The font and the sources need to meet the following properties:

1. The proposed font has to address the needs of Android or web users.

2. The fonts need to be visually harmonized with both Roboto and Noto Sans (for sans versions) or Noto Serif fonts (for serif versions). If there’s only a single font, then a low stroke modulation and low contrast font is preferred so it can better match with Roboto Sans and Noto Sans.

3. The license is SIL OFL.

4. Delivery of a .glyphs source file is required. The source will be published as open source at https://github.com/googlefonts/noto-source/tree/master/src under the current license (SIL Open Font License, version 1.1). Contributions made by corporations are covered by a different agreement than the one above. Please see CONTRIBUTING for more information.

5. Be of high quality.

6. Any and all codepoints in the font need to already exist in the [Unicode Standard](http://www.unicode.org/versions/latest/). The current standard needs to be fully supported.

7. If there are multiple weights or widths, they need to be interpolatable to make variable fonts.

8. Widths, weights, and naming conventions need to be compatible with the rest of the Noto Family.

### Additions to an existing Font Delivery Requirements (when a script already exists)

The Existing and New Font Delivery Requirements apply when a script already exists:

1. If a serif version of the font already exists and a sans version of the font is added, the glyphs in the sans version need to be “aesthetically compatible” to the existing glyphs in the serif version (or a strong justification is required why they are not). The same is true when a serif font is submitted and a sans version already exists.

2. If a sans or serif version of a font exists and a new serif or sans font is produced, then any existing OTF functionality in the existing font ought to be reproduced for the new font.

3. The number of widths or weights supported by the new font needs to be equal or greater to the number of corresponding widths or weights. (At least the existing widths and weights need to be supported.)

4. If a new codepoint is added to an existing font, then a glyph for this new codepoint needs to be “aesthetically compatible” with the already existing glyphs. The addition of a new glyph is required for both sans and serif styles of the font (if applicable).

### Document vs. UI Fonts

When developing various menus, context (right-click) menus, dialog boxes, and other visible text for scripts/languages where ascenders and descenders exceed the UI specs, you might need to develop a more compact version called “UI fonts.” Google Fonts might need to design a UI version which modifies some “natural” glyph shapes to avoid truncation in the Android UI framework.

For example, as of December 2018, the Noto family has these UI fonts: ArabicUI, BengaliUI, DevanagariUI, KannadaUI, KhmerUI, LaoUI, MalayalamUI, MyanmarUI, SinhalaUI, TamilUI, ThaiUI, and NotoSans that supports Latin, Greek, and Cyrillic scripts. NotoSansDisplay is a less “compact” version.

However, there are many scripts where all the fully shaped glyphs required for “modern usage” (as opposed to characters only used for ancient/archaic/special purposes) can meet the following Noto metric requirements without reducing the quality of the fonts. They can be “deemed UI” and do not need a separate UI font. Noto Sans Armenian, Cherokee, Emoji, Ethiopic, Georgian, Gujarati, Gurmukhi, Hebrew, Oriya, Telugu, and Thaana are considered as “deemed UI” fonts.

If a script is unlikely to be used for a UI language (there is no need to use it to localize apps, software or web pages), then you might only need a document font.

CSS3 has a generic “system-ui” family and Noto UI fonts nicely correspond to that generic family. Many web pages and apps are not designed to be flexible in terms of non-Latin TALL script.

### Noto Font Metrics Requirements

Units per Em: 1000

| Table             | Metric         | Noto UI Fonts                  | Noto Document Fonts       |
|-------------------|----------------|--------------------------------|---------------------------|
| head              | ymax           | ≤ 1069                         | ≤ A                       |
| head              | ymin           | ≥ -293                         | ≥ -B                      |
| hhea              | Ascender       | = 1069                         | = A                       |
| hhea              | Descender      | = -293                         | = -B                      |
| hhea              | LineGap        | = 0                            | = 0                       |
| OS/2              | usWinAscent    | = 1069                         | = A                       |
| OS/2              | usWinDescent   | = 293                          | = B                       |
| OS/2              | sTypoAscender  | = 1069                         | = A                       |
| OS/2              | sTypoDescender | = -293                         | = -B                      |
| OS/2              | sTypoLineGap   | = 0                            | = 0                       |
| Fully shaped text |                | should fit within (1069, -293) | should fit within (A, -B) |

Note: The (A, B) metric of document fonts don't need to fit within the constraints specified for UI fonts (1069, -293) [Roboto Regular’s metrics translated for 1000em] or (1056, -271) [matching Open Sans Regular’s metrics]. For document fonts, there is no fixed metric. However, A and B should be reasonable and not be overly large in comparison to other fonts. When proposing a new document font, specify the approximate values.

- For UI fonts: Request an exception if the fully shaped text does not fit within (1069, -293).

- Fully shaped text has different meanings in the UI and document fonts. In the UI font, it refers to the shaped text in languages expected to appear in UIs. For example, Sanskrit text in a UI is very unlikely, but Marathi text in a UI is very likely. In a document font, it refers to all sensible character combinations in all languages that the font supports that are likely to occur in a document.

### References

- [Typophile](https://typophile.com/node/13081)
- [Microsoft’s hhea table spec](https://www.microsoft.com/typography/otspec/hhea.htm)
- [Microsoft’s OS/2 table spec](https://docs.microsoft.com/en-us/typography/opentype/spec/os2)
- [Microsoft’s head table spec](https://docs.microsoft.com/en-us/typography/opentype/spec/head)
