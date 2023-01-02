---
layout: default
title: "Use Noto"
parent: "Website"
nav_order: 21
---
# Use Noto fonts

## How are Noto fonts organized?

Noto is a collection of high-quality fonts with multiple weights and widths in sans, serif, mono and other styles. Noto fonts are made for the world. They offer a modular, flexible typographic system for designers, writers, publishers, advertisers, software makers, students, and scholars everywhere.

All Noto fonts are licensed under the Open Font License. You can use them freely in your products and projects — print or digital, commercial or otherwise. However, you can’t sell the fonts on their own. (This isn’t legal advice, please consider consulting a lawyer and see the [full license](https://github.com/googlefonts/noto-fonts/blob/main/LICENSE) for all details.)

### Noto scripts

The Noto font collection includes over 180 families that consist of nearly 2,300 fonts. Noto fonts are designed and engineered for typographically correct and aesthetically pleasing global communication in more than 1,000 languages and over 150 scripts (writing systems). Noto supports more than 77,000 characters — nearly all the non-Chinese Japanese and Korean (CJK) characters included in the Unicode Standard version 13, and beyond.

The world’s scripts are diverse: they go left-to-right or right-to-left or top-to-bottom. Each has its heritage. Some writing systems evolved over centuries, and are used today for many languages around the world. Other scripts were created for one language or community. Many were forgotten, yet some are experiencing a revival.

Noto is modular to ensure harmonious design across scripts, while retaining the authentic flavors that make each script special. The characters for the European scripts (Latin, Cyrillic, Greek) are in one font. Other scripts like Arabic, Chinese, Devanagari, Hebrew, Ogham or emoji have their own dedicated fonts, specifically engineered to provide the best experience.

### Noto styles: local and global

Noto provides a rich palette of styles (designs). Each supported script has at least one font in a basic style, usually called **Noto Sans [script] Regular**. This is a clean, unornamented design best suitable for online reading.

The **Noto Sans** fonts offer a clean, global look that brings harmony to text in different languages. They are best suitable for short texts, product information, online reading, advertising or branding. For most scripts, the glyphs in Noto Sans have strokes of uniform thickness. If a script’s user community prefers modulated strokes that change their thickness for their sans font, it will be the default style.

For many scripts, the Noto collection also includes a **Noto Serif** design, which has modulated strokes and visible stroke endings. Each Noto Serif family borrows from the heritage of its writing system, and lends the text a local, culture-specific flavor. It is often preferred for book and newspaper typography.

Noto fonts for many scripts include variation in **weight**: there are fonts from thin or extra light (thinnest) to black (boldest). Some scripts also have variation in **width**: there additional fonts that are narrower than the basic style (extra condensed is the narrowest).

For Arabic, Indic, and Southeast Asian scripts, the additional **Noto Sans UI** fonts are optimized for apps and websites where user interface elements have limited vertical space.

### Noto families

The Noto font collection is modular. The main [Noto Sans](../specimen/Noto+Sans) and [Noto Serif](../specimen/Noto+Serif) families (without any suffixes) have letters for languages that use the Latin, Cyrillic, and Greek alphabets. Use these fonts if you have text in any language that uses these scripts (such as English, German, Polish, Russian, Greek). They also contain many characters used across scripts, like punctuation, European digits, currency symbols, or diacritical marks. The fonts also contain the phonetic alphabet (IPA), and characters used in linguistic research.

The main Noto Sans and Noto Serif families include **italic** fonts intended for emphasis. Both also have corresponding display families intended for larger optical sizes (like headlines and titles).

If you have text in another language, find the Noto font that supports that language, and use it together with the corresponding Sans or Serif main font. If your text uses multiple scripts, either the app or the person who typesets the text needs to switch between the different fonts. For example, [Noto Sans Armenian](../specimen/Noto+Sans+Armenian) only has Armenian-script letters. But Armenian text also contains digits, punctuation, it may also contain terms written in Latin or Cyrillic scripts, so you also need the main Noto Sans fonts.

Some apps can switch fonts automatically. For example in CSS, you can specify multiple font families in a stack, and the browser will use the next font if the previous font does not support the necessary characters. In other apps, like Microsoft Word or Adobe InDesign, you can define a separate character style for each script.

Use [Noto Sans Symbols](../specimen/Noto+Sans+Symbols) for boxed and circled letters, astronomical, chemical, and alchemical symbols, and [Noto Sans Symbols 2](../specimen/Noto+Sans+Symbols+2) for Braille letters, dingbats, arrows, and chess symbols.

If you want fonts for continuous reading, like blog posts, articles or essays, you may choose Noto Serif. If a script or a language doesn’t have a Noto Serif design, use the corresponding Noto Sans font.

### Static vs. variable OpenType fonts

Noto fonts are published in the OpenType (ISO Open Font) format and use the Unicode Standard encoding.

Noto fonts that have multiple styles are available as variable and static OpenType fonts. **Static** fonts are traditional OpenType fonts, where every weight and width exists in a single font file. Those fonts work in all apps and all operating systems. Noto fonts that only have one style are available only as static fonts.

In a **variable** font, all weights and widths are included in one font file. The file is smaller than the corresponding set of static fonts. In some apps, you can choose intermediate weights and widths for easier use of Noto fonts with other fonts. But variable fonts only work in new apps and systems.

When you unpack (unzip) the downloaded `.zip` archive for a Noto family, check if there is a sub-folder called `static` inside the unpacked folder.

- If there is no `static` sub-folder, then the unpacked folder contains static OpenType fonts (`.ttf` or `.otf`).

- If there is a `static` sub-folder, then the unpacked folder contains variable OpenType fonts, and the static sub-folder contains the static fonts.

If you’re not sure that your app or system supports variable fonts, install the **static** Noto fonts.

- Read more about [variable fonts](https://design.google/library/variable-fonts-are-here-to-stay/) on Google Design

- Read more about [variable web fonts](https://web.dev/variable-fonts/) on web.dev

## Use Noto fonts on computers and devices

### Download the Noto fonts you need

To use Noto fonts on your computer, download the font families you’re interested in and install them.

1. Click the <samp>Fonts</samp> tab to go to the Noto [font selector](../), which shows samples of all fonts from the Noto font collection.

2. In the search box, type the name of the style (like <samp>Serif</samp>) or script (like <samp>Devanagari</samp>) or language (like <samp>Russian</samp>) or region (like <samp>India</samp>), or click the region or language dropdown to filter the collection.

3. Use the font size dropdown or slider to make the samples smaller or bigger. Use the rightmost buttons to see the samples as tiles or as lists.

4. Click a sample to go to the specimen page for the selected font family.

5. Click <samp>Download Family</samp> to download the selected Noto font family as a.zip archive.

6. Continue the above steps for each Noto family that interests you.

### Install on Windows 10

1. In <samp>File Explorer</samp>, go to the folder where you downloaded the fonts.

2. Right-click the downloaded `.zip` archive, choose <samp>Open with › Windows Explorer</samp>.

3. On top of the <samp>File Explorer</samp> window, click <samp>Extract › Extract all</samp>, and click <samp>Extract</samp>.

4. Go to the unpacked folder, and the `static` folder (if it exists).

5. Select all fonts.

6. Right-click and choose <samp>Install</samp>.

7. Repeat for each downloaded Noto `.zip` archive.

### Install on Windows XP, 7, Vista, 8

1. In <samp>File Explorer</samp>, go to the folder where you downloaded the fonts.

2. Click the <samp>Start</samp> button and choose <samp>Control Panel</samp>.

3. Click <samp>Fonts</samp> to open the system Fonts folder. If you don’t see the <samp>Fonts</samp> icon, first choose <samp>Appearance</samp>.

4. In <samp>Windows Explorer</samp>, right-click the downloaded `.zip` archive, choose <samp>Open</samp> or <samp>Open with › Windows Explorer</samp>.

5. If the `static` sub-folder exists, double-click to enter it.

6. Select all fonts and drag them to the system Fonts folder.

7. Repeat for each downloaded Noto `.zip` archive.

### Install on macOS or Mac OS X

1. Launch the <samp>Font Book</samp> app: in <samp>Finder</samp>, choose your <samp>Applications</samp> folder, locate <samp>Font Book</samp> and double-click it. You can also press <kbd>Command</kbd>+<kbd>Space</kbd>, type <samp>font book</samp> and press <kbd>Enter</kbd>.

2. Also in <samp>Finder</samp>, go to the folder where you downloaded the `.zip` archive.

3. Double-click the `.zip` to unpack the archive.

4. Double-click the unpacked folder to enter the folder. If the `static` sub-folder exists, double-click to enter it.

5. Select all font files and drag them to the <samp>Font</samp> column (the second column) of the <samp>Font Book</samp> app.

### Install on Linux with Gnome desktop

1. Open the <samp>Files</samp> app.

2. Click the menu icon (<samp>☰</samp>) in the top-right area of the <samp>Files</samp> window.

3. Turn on <samp>Show Hidden Files</samp>, click the menu icon again, turn on <samp>Show Sidebar</samp>.

4. In the sidebar, click <samp>Downloads</samp> or go to the folder where you saved the the downloaded `.zip` archive.

5. Right-click the `.zip` archive, choose <samp>Extract here</samp>.

6. Double-click to enter the unpacked folder. If the `static` sub-folder exists, enter it.

7. Click the top <samp>Files</samp> menu and choose <samp>New Window</samp>.

8. Click <samp>Home</samp> in the sidebar.

9. Double-click the `.local` folder to enter it, then `share`, then `fonts`.

10. In the first window, select the unpacked fonts and drag them into the `fonts` folder in the second window.

Some Linux apps will recognize newly installed fonts as soon as the font cache is updated. Some apps require a restart.

## Use Noto fonts on the web

Select the Noto fonts for the writing systems that your website text will use. Add the code that Google Fonts creates to your HTML, and specify the Noto font families in your CSS.

When readers visit your website, their browsers will automatically download the selected Noto **web fonts** from the Google Fonts servers, and your website text will be shown in those fonts. Google Fonts will automatically deliver the fonts in the best format suitable for the reader’s browser.

### Select the fonts

1. Click the <samp>Fonts</samp> tab to go to the Noto [font selector](../), which shows samples of all fonts from the Noto font collection.

2. In the search box, type the name of the style (such as <samp>Serif</samp>) or script (such as <samp>Devanagari</samp>) or language (such as <samp>Russian</samp>) or region (such as <samp>India</samp>), or click the region or language dropdown to filter the collection.

3. Use the font size dropdown or slider to make the samples smaller or bigger. Use the rightmost buttons to see the samples as tiles or as lists.

4. Click a sample to go to the specimen page for the selected font family.

5. In the <samp>Styles</samp> section, click <samp>Select this style</samp> next to each style that you want to use.

6. Continue the above steps for each Noto family that interests you.

### Get the Google Fonts code

1. Click the top-right <samp>View your selected families</samp> button to open the <samp>Selected families</samp> sidebar. Click the close button (<samp>×</samp>) to close the sidebar.

2. In the <samp>Review</samp> section, click the selected family to expand its section. There, you can select more styles from the same family or remove them.

3. In the <samp>Use on the web</samp> section, select the code below the `<link>` indicator and copy it.

4. Paste the copied code into the `<head>` section of your website’s HTML.

5. In your website’s CSS, use the font family names specified in the <samp>CSS rules to specify families</samp> section.

### Web font recommendations

If your website uses many web fonts, it will load (open) slower. Avoid adding too many styles from each Noto family. Most websites don’t need more than three weights for a given family.

The Noto collection has separate fonts for different scripts, so you should only select fonts for the languages that your website actually uses. If your website uses multiple language versions, consider creating separate Google Fonts codes for each language version.

In the CSS `font-family` property, you can specify a “family stack”: multiple font families separated by commas. When the first font does not contain characters necessary to render the text, the browser uses font **fallback**: it tries the second font, then third and so on. When none of the fonts support a particular character, the browser uses the default system font.

If your website is in a non-European language (for example Hindi) and you’re using a sans serif design, select the appropriate style (such as Regular) from the script-specific family (like [Noto Sans Devanagari](../specimen/Noto+Sans+Devanagari)), and the corresponding style from the main [Noto Sans](../specimen/Noto+Sans) family. The Noto Sans family has punctuation signs, digits and other characters that your text may use. Also select [Noto Sans Symbols 2](../specimen/Noto+Sans+Symbols+2) if your website text uses arrows or dingbats.

If you’re using a serif design, select the script-specifc serif font like [Noto Serif Devanagari](../specimen/Noto+Serif+Devanagari), and the matching font from the main [Noto Serif](../specimen/Noto+Serif) family.

In the `font-family` property, put the font family for your most important script/language at the very beginning. However, for Chinese, Japanese or Korean, it’s recommended that you put `Noto Sans` before `Noto Sans TC` (or `SC`, `JP` etc.), and put `Noto Serif` before `Noto Serif TC`.

### Web font use examples

To use the Noto fonts on the entire website, your CSS should set the `font-family` property for the `body` element.

For example, the CSS portion for a website in Hindi and Tamil could look like this:

```css
body {
  font-family: 'Noto Sans Devanagari', 'Noto Sans Tamil', 'Noto Sans', 'Noto Sans Symbols 2', sans-serif;
}
```

For a Japanese website, the `font-family` property would be:

```css
font-family: 'Noto Sans', 'Noto Sans JP', sans-serif;
```

For buttons and other UI elements of an Arabic website:

```css
font-family: 'Noto Sans Arabic UI', 'Noto Sans', sans-serif;
```

For a website targeting Armenian and Georgian users who prefer serif style:

```css
font-family: 'Noto Serif Armenian', 'Noto Serif Georgian', 'Noto Serif', serif;
```

- Read more about the [Google Fonts web font API](https://design.google/library/hot-type-always-fresh/) on Google Design

- Learn how to [optimize web font loading](https://web.dev/optimize-webfont-loading/) and [reduce web font size](https://web.dev/reduce-webfont-size/) on web.dev

- Read the Google Fonts web font [API documentation](https://developers.google.com/fonts/docs/css2)

## Bundle Noto fonts with your native app

All Noto fonts are licensed under the Open Font License. You can bundle the fonts with an app that you create, and you can sell the app if you want, but there are additional license requirements. (This isn’t legal advice, please consider consulting a lawyer and see the [full license](https://github.com/googlefonts/noto-fonts/blob/main/LICENSE) for all details.)

### Android

Add the font files to your app and define them as font resources using XML. Alternatively, use the Downloadable Fonts mechanism to request fonts from a provider application.

- Read more about Android [Font resources](https://developer.android.com/guide/topics/resources/font-resource) and [Downloadable Fonts](https://developer.android.com/guide/topics/ui/look-and-feel/downloadable-fonts)

### iOS

Add the font file that contains your font to your app bundle, then use your font the same way you use any of the iOS-provided custom fonts.

- Read more about [adding custom fonts](https://developer.apple.com/documentation/uikit/text_display_and_fonts/adding_a_custom_font_to_your_app) to an iOS app

## Frequently Asked Questions (FAQ)

### Can I use Noto fonts commercially?

All Noto fonts are licensed under the Open Font License (OFL). You can use them freely in your products and projects — print or digital, commercial or otherwise. However, you can’t sell the fonts on their own. For more questions and answers regarding the Open Font License, see the [OFL FAQ](https://scripts.sil.org/OFL).

(This isn’t legal advice, please consider consulting a lawyer and see the [full license](https://github.com/googlefonts/noto-fonts/blob/main/LICENSE) for all details.)

### How do I report a problem?

Visit our [Contribute](./contribute.md) page. Please be sure to give as much detail as possible. If it’s a technical issue, list the app and operating system used as well as versions. Images and diagrams are very helpful.

### What is the current Unicode support of Noto?

As of April 2021, Noto supports the most commonly used Chinese, Japanese and Korean (CJK) characters defined in Unicode Standard version 13, nearly all of non-CJK Unicode characters, and over half of the entire Unicode character set.

|             | **Noto** | **Unicode** | **% of Unicode** |
|-------------|----------|-------------|------------------|
| Non-CJK     | 46,794   | 49,256      | 95.0%            |
| BMP CJK     | 26,712   | 26,782      | 99.7%            |
| All CJK     | 30,867   | 94,442      | 32.7%            |
| All Unicode | 77,661   | 143,698     | 54.0%            |

### Is there a single Noto font that supports all Unicode?

There is no single universal Noto font. One OpenType font can only hold 65,535 glyphs, and one Unicode character often needs more than one glyph. The Noto collection supports many more characters that can fit into one font. There are also additional technical limitations that makes creating a single global font impossible.

Noto is a global font collection. The designs are harmonious across scripts, but retain the authentic flavors that make each script special. If you want global font support, you will need some knowledge of how to put the pieces in this collection together into a solution that works for you.

### How do I use Noto fonts with other fonts?

If you already use a sans font (such as Roboto, Lato, Montserrat, Source Sans and many others), and if your document or website needs to support other scripts, you can use Noto Sans as a “fallback.”

If you use another serif font such as Merriweather, Playfair, PT Serif, Crimson Text or Source Serif, for example for your main text, you can complement the global reading experience with the Noto Serif font series.

If you use Noto fonts together with other fonts, choose the Noto style, weight and width that best matches your primary font. You may need to adjust the font size for each script for a more harmonious experience.

### Why is text in Arabic, Devanagari or other scripts displayed incorrectly?

Many scripts need several glyphs to represent the same character in different positions within a word. A Noto font for a given script includes all the required glyphs, as well as advanced typographic features, which define shaping rules. The shaping rules enable complex text layout: accurate, orthographically correct rendering of that script.

Browsers and most word processing apps have full support for shaping and complex text layout. But many apps, especially older versions of graphic design apps, don’t support shaping for all scripts.

If you use Noto for a language you don’t know, compare what the text looks like in Google Chrome and what you see in the app. If the text in your app looks very different, for example if the letters are disjoined or are in the reverse order, check if your app has a text setting or preference to activate correct rendering.

Different products use different words for these settings, like “complex script support” or “world-ready composer” and these are optional because they can be slower. You may also consider using a different app to typeset the text.

- Read more about [complex text layout](https://en.wikipedia.org/wiki/Complex_text_layout) on Wikipedia.

### How do I use Noto UI fonts?

Many scripts form lines of text where all characters have roughly the same height, with only some letters extending below the baseline. User interface elements (menus, buttons, text boxes) in apps and on websites are often designed with a particular script in mind (often Latin).

However, letters in Arabic, Indic, and Southeast Asian scripts often connect both vertically and horizontally. So text for continuous reading in those scripts needs a more generous line height. For those scripts, Noto includes an additional family with the **UI** suffix. These fonts are more compact vertically and have the same line height as the basic Noto Sans fonts.

| **Languages or scripts** | **Noto fonts to use** |
|---|---|
| Latin, Cyrillic, or Greek scripts | [Noto Sans](../specimen/Noto+Sans) for user interfaces and for documents |
| [Bengali](../specimen/Noto+Sans+Bengali+UI/), [Devanagari](../specimen/Noto+Sans+Devanagari+UI/), [Gujarati](../specimen/Noto+Sans+Gujarati+UI/), [Gurmukhi](../specimen/Noto+Sans+Gurmukhi+UI/), [Kannada](../specimen/Noto+Sans+Kannada+UI/), [Khmer](../specimen/Noto+Sans+Khmer+UI/), [Lao](../specimen/Noto+Sans+Lao+UI/), [Malayalam](../specimen/Noto+Sans+Malayalam+UI/), [Myanmar](../specimen/Noto+Sans+Myanmar+UI/), [Oriya](../specimen/Noto+Sans+Oriya+UI/), [Sinhala](../specimen/Noto+Sans+Sinhala+UI/), [Tamil](../specimen/Noto+Sans+Tamil+UI/), [Telugu](../specimen/Noto+Sans+Telugu+UI/), [Thai](../specimen/Noto+Sans+Thai+UI/) | Noto Sans with the script and “UI” suffixes for user interfaces with limited vertical space, fonts without the “UI” suffix for documents |
| Arabic | [Noto Sans Arabic UI](../specimen/Noto+Sans+Arabic+UI/) or [Noto Naskh Arabic UI](../specimen/Noto+Naskh+Arabic+UI/) for user interfaces with limited vertical space, fonts without the UI suffix for documents |
| Armenian, Cherokee, Ethiopic, Georgian, Hebrew, and other scripts | Noto Sans with the script suffix for user interfaces and for documents |

### Which Noto fonts should I use for the Adlam script?

Noto has two Noto Sans fonts for the Adlam script that is used to write the Fulani language of Central and West Africa:

- [Noto Sans Adlam](../specimen/Noto+Sans+Adlam/), an unmodulated design with joining (cursive) letters, suitable for most texts

- [Noto Sans Adlam Unjoined](../specimen/Noto+Sans+Adlam+Unjoined/), an unmodulated design with unjoined (block) letters, suitable for headlines and for educational content

### Which Noto fonts should I use for the Arabic script?

Noto has six font families for the Arabic script:

- [Noto Sans Arabic](../specimen/Noto+Sans+Arabic/), an unmodulated design, suitable for all uses

- [Noto Sans Arabic UI](../specimen/Noto+Sans+Arabic+UI/), a variant of the Sans design for user interfaces with limited vertical space

- [Noto Kufi Arabic](../specimen/Noto+Kufi+Arabic/), a simplified unmodulated design in the Kufi (or Kufic) style of Arabic lettering. Noto Kufi Arabic is more simplified than Noto Sans Arabic, and is suitable for headlines and short texts, such as in packaging or advertising

- [Noto Naskh Arabic](../specimen/Noto+Naskh+Arabic/), a modulated font in the Naskh style of Arabic calligraphy, which is suitable for longer texts. Noto Naskh Arabic can be used together with Noto Serif fonts for other scripts

- [Noto Naskh Arabic UI](../specimen/Noto+Naskh+Arabic+UI/), a variant of the Naskh design for user interfaces with limited vertical space

- [Noto Nastaliq Urdu](../specimen/Noto+Nastaliq+Urdu/), a modulated cursive font in the Nastaliq style of Persian calligraphy, predominantly used for the Urdu language. The Nastaliq style was developed in Iran in the 15th century, and is used for the Persian, Urdu and Turkic languages that use the Arabic script.

### Which Noto fonts should I use for Chinese, Japanese or Korean?

The Noto collection includes two font families for the Chinese, Japanese and Korean languages: Noto Sans CJK, an unmodulated design, and Noto Serif CJK, a modulated design. Each of these families has 7 weights, and Noto Sans CJK is also available as a variable font.

These fonts are available in these language variants:

- [Noto Sans JP](../specimen/Noto+Sans+JP/) and [Noto Serif JP](../specimen/Noto+Serif+JP/) for the Japanese language

- [Noto Sans SC](../specimen/Noto+Sans+SC/) and [Noto Serif SC](../specimen/Noto+Serif+SC/) for the Simplified Chinese language variant used in the mainland People’s Republic of China

- [Noto Sans TC](../specimen/Noto+Sans+TC/) and [Noto Serif TC](../specimen/Noto+Serif+TC/) for the Traditional Chinese language variant used in Taiwan

- [Noto Sans HK](../specimen/Noto+Sans+HK/) for the Traditional Chinese language variant used in Hong Kong

- [Noto Sans KR](../specimen/Noto+Sans+KR/) and [Noto Serif KR](../specimen/Noto+Serif+KR/) for the Korean language

The Noto Sans CJK fonts contain all Han ideographs included in the Basic Multilingual Plane (BMP) of the Unicode Standard plus over 2,000 non-BMP Han ideographs.

### Which Noto fonts should I use for the Hebrew script?

Noto has three font families for Hebrew:

- [Noto Sans Hebrew](../specimen/Noto+Sans+Hebrew/), an unmodulated design with a square skeleton and no stroke modulation, suitable for all uses.

- [Noto Serif Hebrew](../specimen/Noto+Serif+Hebrew/), a modulated design with a square skeleton, suitable for longer texts.

- [Noto Rashi Hebrew](../specimen/Noto+Rashi+Hebrew/), a modulated design with a semi-cursive skeleton based on 15th-century Sephardic writing. It can be used for emphasis, complementing Noto Serif Hebrew. This type of design was used by early Hebrew typographers to set rabbinic commentary in the Talmud and Tanakh, while the primary text was set in a square Serif typeface.

### Which fonts should I use for the emoji characters?

Unicode includes over 3,500 emoji characters. Each operating system uses a different font format to represent color emoji. The Google Fonts team recommends that you use the emoji fonts that are bundled with your app or system.

The Noto collection includes two fonts that contain emoji characters:

- [Noto Emoji](../specimen/Noto+Emoji/), a monochrome (non-color) font in TrueType-flavored OpenType format. It only contains about 25% of all encoded emoji but has scalable monochrome glyphs. It is intended for limited use in print publications, on monochrome displays, and in other scenarios where multiple colors cannot be reproduced.

- [Noto Color Emoji](../specimen/Noto+Color+Emoji), a multi-color font in the OpenType CBDT format. The font supports all emoji in Unicode 13 and beyond, but only works on Android, in Google Chrome, and in apps that support the CBDT format. [Download the font](https://github.com/googlefonts/noto-emoji/tree/main/fonts) from Github.

### Which Noto fonts should I use for the Lao and Thai scripts?

Noto has five font families for the Lao script, and five for the Thai script:

- [Noto Looped Lao](../specimen/Noto+Looped+Lao/) and [Noto Looped Thai](../specimen/Noto+Looped+Thai/) are unmodulated designs in the more traditional style that includes loops, suitable for all uses including longer texts.

- [Noto Looped Lao UI](../specimen/Noto+Looped+Lao+UI/) and [Noto Looped Thai UI](../specimen/Noto+Looped+Thai+UI/) are variants of the looped designs for user interfaces with limited vertical space.

- [Noto Sans Lao](../specimen/Noto+Sans+Lao/) and [Noto Sans Thai](../specimen/Noto+Sans+Thai/) are unmodulated designs in the more modern loopless style, suitable for all uses, particularly headlines, packaging and advertising.

- [Noto Sans Lao UI](../specimen/Noto+Sans+Lao+UI/) and [Noto Sans Thai UI](../specimen/Noto+Sans+Thai+UI/) are variants of the Sans designs for user interfaces with limited vertical space.

- [Noto Serif Lao](../specimen/Noto+Serif+Lao/) and [Noto Serif Thai](../specimen/Noto+Serif+Thai/) are modulated looped designs for longer texts.

### Which Noto fonts should I use for the Nüshu script?

Noto has two font families for the Nüshu script:

- [Noto Sans Nushu](../specimen/Noto+Sans+Nushu/) is an unmodulated design in one weight, with a simplified, modernized skeleton and relatively large counters. It is suitable for shorter texts, especially in smaller font sizes and user interface contexts.

- [Noto Traditional Nushu](../specimen/Noto+Traditional+Nushu/) is an unmodulated design in three weights, with a more calligraphic skeleton and a more compact appearance. It is suitable for longer texts, especially those set in medium font sizes and for headlines.

### Why do some Noto Sans fonts have modulated strokes?

The Noto Sans fonts mostly have uniform strokes without pronounced endings. However, the Noto Sans fonts for some scripts do have stroke modulation if the user community of a particular script prefers it.

Traditionally, European scripts were of serif style. The sans style was introduced in the 19th century, and was originally not considered serious. The terms “grotesque” or “grotesk” are used for a category of sans fonts. Today, typography on screens mostly uses sans designs but books or newspapers are still typeset with serif designs.

Not all writing systems have the same history. Users of some scripts prefer to always have stroke modulation. To ensure authenticity and to provide a pleasing reading experience for those communities, the Noto Sans fonts for that script have stroke modulation.

### Which Noto monospace fonts should I use?

- [Noto Sans Mono](../specimen/Noto+Sans+Mono/), a monospace font for languages written in Latin, Cyrillic, and Greek scripts, in multiple weights

- [Noto Sans Mono CJK HK](../specimen/Noto+Sans+Mono+CJK+HK/), a monospace font for the Traditional Chinese language variant used in Hong Kong, in two weights

- [Noto Sans Mono CJK JP](../specimen/Noto+Sans+Mono+CJK+JP/), a monospace font for the Japanese language, in two weights

- [Noto Sans Mono CJK KR](../specimen/Noto+Sans+Mono+CJK+KR/), a monospace font for the Korean language, in two weights

- [Noto Sans Mono CJK SC](../specimen/Noto+Sans+Mono+CJK+SC/), a monospace font for the Simplified Chinese language variant used in the People’s Republic of China, in two weights

- [Noto Sans Mono CJK TC](../specimen/Noto+Sans+Mono+CJK+TC/), a monospace font for the Traditional Chinese language variant used in Taiwan, in two weights

For most use cases such as programming code, use Noto Sans Mono.

### Where can I download all Noto fonts?

The Google Fonts team recommends that you download the Noto font families that you need from the [Google Fonts Noto](https://fonts.google.com/noto/) website.

However, you can also download **development builds** in several formats. These fonts may contain bugs and may differ slightly from the fonts available on Google Fonts.

- [Download all non-CJK Noto](https://github.com/googlefonts/noto-fonts/archive/refs/heads/main.zip) fonts, or visit the [repository](https://github.com/googlefonts/noto-fonts) on Github.
- [Download all Noto CJK](https://github.com/googlefonts/noto-cjk/archive/refs/heads/main.zip) fonts, or visit the [repository](https://github.com/googlefonts/noto-cjk) on Github. This includes versions in the space-saving [OpenType Collection](https://github.com/googlefonts/noto-cjk/blob/main/README-formats.md) (`.ttc`) format.

### When will language or script X be supported by Noto?

The Google Fonts team intends to support all scripts encoded by Unicode. This takes time. The team prioritizes additions depending on the complexity of the script, on product and project needs, on the availability of script experts and designers, on the number and responsiveness of language reviewers, and on other factors.

### When will Noto support Klingon, Elvish etc.?

The [Script Encoding Initiative](https://linguistics.berkeley.edu/sei/scripts-not-encoded.html) lists scripts that are not yet included in the Unicode Standard. Once Klingon, Elvish etc. are included in Unicode, the Google Fonts team will consider adding them to Noto. [Contact](https://corp.unicode.org/reporting.html) the Unicode Consortium to encourage them to support your favourite script or language.

### Is Noto based on existing fonts?

The Latin characters in Noto Sans are based on Steve Matteson’s designs for Droid Sans and Open Sans. The Latin characters in Noto Serif are based on Droid Serif. Noto fonts completely replace the Droid fonts. Noto fonts are undergoing regular reviews and revisions and have more styles than the older fonts.

Noto Sans CJK is the same design as Adobe Han Sans and the Latin characters are based on Adobe’s Source Sans Pro. Noto Serif CJK is the same design as Adobe Han Serif, and the Latin characters are based on Adobe’s Source Serif Pro.

The Noto fonts for many other scripts are original designs, while some are adapted from earlier existing designs. The Noto fonts for some scripts may be similar to existing fonts, often because the same designers created them, or because the fonts were modeled on the same calligraphic or typographic references.
