---
layout: default
title: "Submissions"
parent: "Technical"
nav_order: 210
---
# Noto Font Submission Requirements

{:toc}

### Objective

Thank you for considering contributing to Noto. Noto is Google’s library of fonts which covers the whole of the Unicode range - every encoded script, living and historical. If you have not already done so, please familiarize yourself with the [Noto Project Overview](https://fonts.google.com/noto).

As Noto is part of the Google Fonts library, contributions must be compliant with our expectations set out in the [Google Fonts guide](https://googlefonts.github.io/gf-guide/). Please read that carefully. This document is a summary of the most important aspects of that guide, together with some information which is specific to Noto.

### New Font Delivery Requirements

1. Noto is a libre and open source font programme of nearly 200 typeface projects, each hosted at github.com/notofonts. The development of each script is carried out in a separate GitHub repository under the notofonts organization. New projects start by using the [Noto repository template](https://github.com/notofonts/noto-project-template). To start a new script, go there and press the green button to “use this template”. Google has commissioned Simon Cozens throughout 2023 to provide technical support in getting the repository and your development environment set up.

2. *When working on a commission from Google for a Noto font, you are expected to check in and push your work incrementally - at least daily, if not after each substantive change - rather than as one final deliverable.*

3. Checking in your font regularly allows you to make use of the Continuous Integration system which builds and tests your font for you. *All Google Fonts projects must be built using a reproducible, libre toolchain. We do not onboard binaries exported from font editors.* In other words, you are expected to deliver the *design sources from which final fonts can be built by the Continuous Integration process*. These should be in Glyphs or UFO format. Additional compilation steps are possible, but must be integrated into an automated build process. If you think that such steps are necessary, we expect you to notify us as soon as possible.

4. We expect you to be proofing and testing from the CI builds of the font, downloadable from the “Actions” tab in GitHub, from the earliest check-ins. If your font requires additional support for building, raise this with Google at the first opportunity.

5. Similarly, the GitHub-created artifacts include a Fontbakery font checker report, which will help you to ensure that your font meets Google Fonts QA standards. Fonts are expected to pass all checks in the Fontbakery Google Fonts profile before delivery.

6. New projects are commissioned to cover a particular Unicode range. Unless there are strong reasons to include glyphs from outside this range, the only glyphs from outside the range expected in the font are space and nbspace (whose advance widths must be equal).

7. As a minimum requirement, the fonts must implement the Unicode Standard and the material in the Unicode proposal for a particular script. Fulfilling user needs (for example, with the choice of conjuncts provided) is a secondary requirement.

8. We expect you to conduct a review of your font with members of the appropriate language community/communities (for living scripts) or with linguistic experts, and for you to revise the font appropriately in response to their comments.

9. You are allowed to credit yourself or your company as the Manufacturer of the font, and you are expected to add your name to the CONTRIBUTORS document. However, remember that Noto is a collaborative project; see the “[Libre Font Culture](https://googlefonts.github.io/gf-guide/culture.html)” chapter of the GF Guide for the implications of this.

10. Because of the need to maintain these fonts, and the possibility of other contributors in the future, it is very important that decisions you make are well documented. Along with font sources in the sources directory of the repository, you are also expected to populate the documentation directory with either copies of, or links to, any material used to inform the decisions made in creating the font. For example:
  * As a bare minimum, the Unicode standard chapter and the final Unicode proposal for the script.
  * Any other Unicode proposals or discussion documents.
  * Any photographs or other typographic references.
  * Descriptions of design decisions you made. (See [Noto Sans Nushu process documentation](https://notofonts.github.io/noto-sans-nushu/noto-sans-nushu-process/) for an example.)
  * Any text strings you use for testing and proofing.

11. You are expected to provide a range of short sample texts for the script, encoded in Unicode. (See [Latin example here](https://github.com/googlefonts/lang/blob/d885b2e8d70601c87d05b2808590a95b1cfc48d9/Lib/gflanguages/data/languages/en_Latn.textproto#L163-L176).)

12. The fonts need to be visually harmonized with both Roboto and Noto Sans (for sans versions) or Noto Serif fonts (for serif versions). If there’s only a single font, then a low stroke modulation and low contrast font is preferred so it can better match with Roboto Sans and Noto Sans.

13. If there are multiple weights or widths, they need to be interpolatable to make variable fonts.

14. Widths, weights, and naming conventions need to be compatible with the rest of the Noto Family.

### Additions to an existing Font Delivery Requirements (when a script already exists)

The Existing and New Font Delivery Requirements apply when a script already exists:

1. Updates to a Noto font are expected to be received as a pull request, or series of pull requests, to that font’s repository. Fork the appropriate repository on github by using the “Fork” button on the top right, make your changes, and then create a pull request.

2. These pull requests should be accompanied by high-level descriptions of the changes they make.

3. As for “new scripts” above, you are expected to commit your changes to the repository incrementally. You are also expected to engage with the project’s issue tracker. (See [Maintaining your font repo](https://googlefonts.github.io/gf-guide/maintaining.html) in the GF Guide.)

4. Changes which fix an issue should also be accompanied by a regression test case in `qa/shaping_files/issues.json`; see [Zanabazar Square](https://github.com/notofonts/zanabazar-square/blob/main/qa/shaping_tests/issues.json) for an example.

5. If a serif version of the font already exists and a sans version of the font is added, the glyphs in the sans version need to be “aesthetically compatible” to the existing glyphs in the serif version. If they are not "aesthetically compatible," please provide a strong justification. The same is true when a serif font is submitted and a sans version already exists.

6. If a sans or serif version of a font exists and a new serif or sans font is produced, then any existing OTF functionality in the existing font ought to be reproduced for the new font; the glyphset and shaping rules should be the same.

7. The number of widths or weights supported by the new font needs to be equal or greater to the number of corresponding widths or weights. (At least the existing widths and weights need to be supported.)

8. If a new codepoint is added to an existing font, then a glyph for this new codepoint needs to be “aesthetically compatible” with the already existing glyphs. The addition of a new glyph is required for both sans and serif styles of the font (if applicable).
