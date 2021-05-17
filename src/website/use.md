# Use Noto fonts

## How are Noto fonts organized?

Noto is a collection of high-quality fonts with multiple weights and widths in sans, serif, mono and other styles. The Noto fonts are made for the world. They offer a modular, flexible typographic system for designers, writers, publishers, advertisers, software makers, students, and scholars everywhere.

The Noto fonts are licensed under the Open Font License. You can use them freely in your products and projects — print or digital, commercial or otherwise. However, you can’t sell the fonts on their own. (This isn’t legal advice, please consider consulting a lawyer and see the [full license](https://github.com/googlefonts/noto-fonts/blob/main/LICENSE) for all details.)

### Noto scripts

The Noto font collection includes 205 families that consist of nearly 2,300 fonts. Noto fonts are designed and engineered for typographically correct and aesthetically pleasing global communication in more than 1,000 languages and over 150 scripts (writing systems). Noto supports more than 77,000 characters — nearly all non-CJK characters included in the Unicode Standard version 13, and beyond.

The world’s scripts are diverse: they go left-to-right or right-to-left or top-to-bottom. Noto is modular to ensure harmonious design across scripts while retaining the authentic flavors that make each script special. The characters for the European scripts (Latin, Cyrillic, Greek) are in one font. Other scripts like Arabic, Chinese, Devanagari, Hebrew, Ogham or emoji have their own dedicated fonts, specifically engineered to provide the best experience.

### Noto styles

Noto provides a rich palette of styles (designs). Each supported script has at least one font in a basic style, usually called **Noto Sans \[script\] Regular**. This is a clean, unornamented design best suitable for online reading.

The **Noto Sans** fonts are best suitable for short texts, product information, online reading, advertising or branding. For most scripts, the glyphs in Noto Sans have strokes of uniform thickness. Some Noto Sans fonts have letters made with modulated strokes that change their thickness — this is done if the user community of that script prefers this as the default style.

For many scripts, the Noto collection also includes a **Noto Serif** design. This design has modulated strokes and visible stroke endings, and is often preferred for book and newspaper typography.

Noto fonts for many scripts include variation in **weight**: there are fonts from Thin or Extra Light (thinnest) to Black (boldest). Some scripts also have variation in **width**: there additional fonts that are narrower than the basic style (Extra Condensed is the narrowest).

For Arabic, Indic, and Southeast Asian scripts, the additional **Noto Sans UI** fonts are optimized for apps and websites where user interface elements have limited vertical space.

### Noto families

The Noto fonts are modular. The **main** Noto Sans and Noto Serif families (without any suffixes) have letters for languages that use the Latin, Cyrillic, and Greek alphabets. If you have text any language that uses these scripts (like English, German, Polish, Russian, Greek), use these fonts. They also contain many characters used across scripts, like punctuation, European digits, currency symbols, or diacrtitical marks. The fonts also contain the phonetic alphabet (IPA), and characters used in linguistic research.

The main Noto Sans and Noto Serif families include **italic** fonts intended for emphasis. They also have a corresponding **Display** family intended for larger optical sizes (like headlines and titles).

If you have text in another language, find the Noto font that supports that language, and use it together with the corresponding main font.

If you have text in multiple languages that use different scripts, either the app or the person who typesets the text needs to switch between the different fonts accordingly. For example, Noto Sans Armenian only has Armenian-script letters. But Armenian text also contains digits, punctuation, it may also contain terms written in Latin or Cyrillic scripts, so you also need the main Noto Sans fonts.

Some apps can switch fonts automatically. For example in CSS, you can specify multiple font families in a “stack”, and the browser will use the next font if the previous font does not support the necessary characters. In other apps like Microsoft Word or Adobe InDesign you can define a separate “character style” for each script.

Use Noto Sans Symbols for boxed and circled letters, astronomical, chemical, and alchemical symbols, and Noto Sans Symbols2 for Braille letters, dingbats, arrows, and chess symbols.

If you want fonts for continuous reading, like blog posts, articles or essays, you may choose Noto Serif. If a script or a language doesn’t have a Noto Serif design, use the corresponding Noto Sans font.

### Static vs. variable OpenType fonts

Noto fonts are published in the OpenType (ISO Open Font) format and use the Unicode Standard encoding.

Noto fonts that have multiple styles are available as variable and static OpenType fonts. **Static** fonts are traditional OpenType fonts, where every weight and width exists in a single font file. Those fonts work in all apps and all operating systems. Noto fonts that only have one style are available only as static fonts.

In a **variable** font, all weights and widths are included in one font file. The file is smaller than the corresponding set of static fonts. In some apps, you can choose intermediate weights and widths for easier use of Noto fonts with other fonts. But variable fonts only work in new apps and systems.

When you unpack (unzip) the downloaded.zip archive for a Noto family, check if there is a sub-folder called *static* inside the unpacked folder.

- If there is no *static* sub-folder, then the unpacked folder contains static OpenType fonts (.ttf or.otf).

- If there is a *static* sub-folder, then the unpacked folder contains variable OpenType fonts, and the static sub-folder contains the static fonts.

If you’re not sure that your app or system supports variable fonts, install the **static** Noto fonts.

- Read more about [variable fonts](https://design.google/library/variable-fonts-are-here-to-stay/) on Google Design

- Read more about [variable web fonts](https://web.dev/variable-fonts/) on web.dev

## Use Noto fonts on computers and devices

### Download the Noto fonts you need

To use Noto fonts on your computer (a notebook or desktop), you should download the font families you’re interested in and install them.

1. Click the *Fonts* tab to go to the Noto font selector, which shows samples of all fonts from the Noto font collection.

2. In the search box, type the name of the style (like *Serif*) or script (like *Devanagari*) or language (like *Russian*) or region (like *India*), or click the region or language dropdown to filter the collection.

3. Use the font size dropdown or slider to make the samples smaller or bigger. Use the rightmost buttons to see the samples as tiles or as a list.

4. Click a sample to go to the specimen page for the selected font family.

5. Click *Download Family* to download the selected Noto font family as a.zip archive.

6. Continue the above steps for each Noto family that interests you.

### Install on Windows 10

1. In *File Explorer*, go to the folder where you downloaded the fonts.

2. Right-click the downloaded.zip archive, choose *Open with › Windows Explorer*.

3. On top of the *File Explorer* window, click *Extract › Extract all*, and click *Extract*.

4. Go to the unpacked folder, and the static folder inside it if it exists.

5. Select all fonts.

6. Right-click and choose *Install*.

7. Repeat for each downloaded Noto.zip archive.

### Install on Windows XP, 7, Vista, 8

1. In *File Explorer*, go to the folder where you downloaded the fonts.

2. Click the *Start* button and choose *Control Panel*.

3. Click *Fonts* to open the system Fonts folder. If you don’t see the *Fonts* icon, first choose *Appearance*.

4. In *Windows Explorer*, right-click the downloaded.zip archive, choose *Open* or *Open with › Windows Explorer*.

5. If the *static* sub-folder exists, double-click to enter it.

6. Select all fonts and drag them to the system Fonts folder.

7. Repeat for each downloaded Noto.zip archive.

### Install on macOS or Mac OS X

1. Launch the *Font Book* app: in *Finder*, choose your *Applications* folder, locate *Font Book* and double-click it. You can also press Command+Space, type *font book* and press Enter.

2. Also in *Finder*, go to the folder where you downloaded the.zip archive.

3. Double-click the.zip to unpack the archive.

4. Double-click the unpacked folder to enter the folder. If the *static* sub-folder exists, double-click to enter it.

5. Select all of the font files and drag them to the *Font* column (the second column) of the *Font Book* app.

### Install on Linux with Gnome desktop

1. Open the *Files* app.

2. Click the menu icon (☰) in the top-right area of the *Files* window.

3. Turn on *Show Hidden Files*, click the menu icon again, turn on *Show Sidebar*.

4. In the sidebar, click *Downloads* or go to the folder where you saved the the downloaded.zip archive.

5. Right-click the.zip archive, choose *Extract here*.

6. Double-click to enter the unpacked folder. If the *static* sub-folder exists, enter it.

7. Click the top *Files* menu and choose *New Window*.

8. Click *Home* in the sidebar.

9. Double-click the *.local* folder to enter it, then *share*, then *fonts*.

10. In the first window, select the unpacked fonts and drag them into the *fonts* folder in the second window.

Some Linux apps will recognize newly installed fonts as soon as font-cache is updated. Some apps require a restart.

## Use Noto fonts on the web

To use the Noto fonts on your website, select the Noto fonts for the writing systems that your website text will be using. Add the code that Google Fonts creates to your HTML, and specify the Noto font families in your CSS.

When readers visit your website, their browsers will automatically download the selected Noto **web fonts** from the Google Fonts servers, and your website text will be shown in those fonts. Google Fonts will automatically deliver the fonts in the best format suitable for the reader’s browser.

### Select the fonts

1. Click the *Fonts* tab to go to the Noto font selector, which shows samples of all fonts from the Noto font collection.

2. In the search box, type the name of the style (like *Serif*) or script (like *Devanagari*) or language (like *Russian*) or region (like *India*), or click the region or language dropdown to filter the collection.

3. Use the font size dropdown or slider to make the samples smaller or bigger. Use the rightmost buttons to see the samples as tiles or as a list.

4. Click a sample to go to the specimen page for the selected font family.

5. In the *Styles* section, click *Select this style* next to each style that you want to use.

6. Continue the above steps for each Noto family that interests you.

### Get the Google Fonts code

1. Click the top-right *View your selected families* button to open the *Selected families* sidebar. Click the close button (×) to close the sidebar.

2. In the *Review* section, click the selected family to expand its section. There, you can select more styles from the same family or remove them.

3. In the *Use on the web* section, select the code below the \<link\> indicator and copy it.

4. Paste the copied code into the \<head\> section of your website’s HTML.

5. In your website’s CSS, use the font family names specified in the *CSS rules to specify families* section.

### Web font recommendations

If your website uses many web fonts, it will load (open) slower. Avoid adding too many styles from each Noto family. Most websites don’t need more than three weights for a given family.

The Noto collection has separate fonts for different scripts, so you should only select fonts for the languages that your website actually uses. If your website multiple language versions, you may want to create separate Google Fonts codes for each language version of your website.

In the CSS `font-family` property, you can specify multiple font families separated by commas. When the first font does not contain characters necessary to render the text, the browser uses font **fallback**: it tries the second font, then third and so on. When none of the fonts support a particular character, the browser uses the default system font.

If your website is in a non-European language (for example Hindi) and you’re using a sanserif design, select the appropriate style (like Regular) from the script-specific family (like Noto Sans Devanagari), and the corresponding style from the Noto Sans family. The Noto Sans family has punctuation signs, digits and other characters that your text may use. Also select Noto Sans Symbols2 if your website text uses arrows or dingbats.

If you’re using a serif design, select the script-specifc serif font like Noto Serif Devanagari, and also Noto Serif.

In the `font-family` property, put the font family for your most important script/language at the very beginning. However, for Chinese, Japanese or Korean, it’s recommended that you put Noto Sans before Noto Sans CJK, and put Noto Serif before Noto Serif CJK.

### Web font use examples

To use the Noto fonts on the entire website, your CSS should set the `font-family` property for the `body` element.

For example, the CSS portion for a website in Hindi and Tamil could look like this:

```
body {
  font-family: 'Noto Sans Devanagari', 'Noto Sans Tamil', 'Noto Sans', 'Noto Sans Symbols2', sans-serif;
}
```

For a Japanese website, the `font-family` property would be:

```
font-family: 'Noto Sans', 'Noto Sans CJK JP', sans-serif;
```

For buttons and other UI elements of an Arabic website:

```
font-family: 'Noto Sans Arabic UI', 'Noto Sans UI', sans-serif;
```

For a website targeting Armenian and Georgian users who prefer serif style:

```
font-family: 'Noto Serif Armenian', 'Noto Serif Georgian', 'Noto Serif', serif;
```

- Read more about the [Google Fonts web font API](https://design.google/library/hot-type-always-fresh/) on Google Design

- Learn how to [optimize web font loading](https://web.dev/optimize-webfont-loading/) and [reduce web font size](https://web.dev/reduce-webfont-size/) on web.dev

- Read the Google Fonts web font [API documentation](https://developers.google.com/fonts/docs/css2)

## Bundle Noto fonts with your native app

The Noto fonts are licensed under the Open Font License. You can bundle the fonts with an app that you create, and you can sell the app if you want, but there are additional license requirements. (This isn’t legal advice, please consider consulting a lawyer and see the [full license](https://github.com/googlefonts/noto-fonts/blob/main/LICENSE) for all details.)

### Android

Add the font files to your app and define them as font resources using XML. Alternatively, use the Downloadable Fonts mechanism to request fonts from a provider application.

- Read more about Android [Font resources](https://developer.android.com/guide/topics/resources/font-resource) and [Downloadable Fonts](https://developer.android.com/guide/topics/ui/look-and-feel/downloadable-fonts)

### iOS

Add the font file that contains your font to your app bundle, then use your font the same way you use any of the iOS-provided custom fonts.

- Read more about [adding custom fonts](https://developer.apple.com/documentation/uikit/text_display_and_fonts/adding_a_custom_font_to_your_app) to an iOS app

## Frequently Asked Questions (FAQ)

### How do I report a problem?

Visit our [Contribute](./contribute.md) page. Please be sure to give as much detail as possible. If it’s a technical issue, list the app and operating system being used as well as versions. Images and diagrams are very helpful.

### What is the current Unicode support of Noto?

As of April 2021, Noto supports the most commonly used Chinese, Japanese and Korean (CJK) characters defined in Unicode Standard version 13, nearly all of non-CJK Unicode characters, and over half of the entire Unicode character set.

|             | **Noto** | **Unicode** | **% of Unicode** |
|-------------|----------|-------------|------------------|
| Non-CJK     | 46,794   | 49,256      | 95.0%            |
| BMP CJK     | 26,712   | 26,782      | 99.7%            |
| All CJK     | 30,867   | 94,442      | 32.7%            |
| All Unicode | 77,661   | 143,698     | 54.0%            |

### Is there a single Noto font that supports all Unicode?

There is no one “Noto font”. One OpenType font can only hold 65,535 glyphs, and one Unicode character often needs more than one glyph, so Noto supports many more characters that can fit into one font. There are also additional technical limitations that makes creating a single global font impossible.

Noto is a global font collection. The designs are harmonious across scripts, but retain the authentic flavors that make each script special. If you want global font support, you will need some knowledge of how to put the pieces in this collection together into a solution that works for you.

### How do I use Noto fonts with other fonts?

If you already use a sans font you like (like Roboto, Lato, Montserrat, Source Sans and many others), and if your document or website needs to support other scripts, you can use Noto Sans as a “fallback.”

If you use another serif font such as Merriweather, Playfair, PT Serif, Crimson Text or Source Serif, for example for your main text, you can complement the global reading experience with the Noto Serif font series.

If you use Noto fonts together with other fonts, choose the Noto style, weight and width that best matches your primary font. You may need to adjust the font size for each script for a more harmonious experience.

### Why is text in Arabic, Devanagari or other scripts displayed wrong?

Many scripts need several glyphs to represent the same character in different positions within a word. A Noto font for a given script includes all the required glyphs, as well as advanced typographic **features**, which define **shaping** rules. The shaping rules enable complex text layout: accurate, orthographically correct rendering of that script.

Browsers and most word processing apps have full support for shaping and complex text layout. But many apps, especially older versions of graphic design apps, don’t support shaping for all scripts.

If you use Noto for a language you don’t know, you may want to compare what the text looks like in Google Chrome and what you see in the app. If the text in your app looks largely different, for example the letters are disjoined or are in the reversed order, check if your app has a text setting or preference to activate correct rendering.

Different products use different words for these settings, like “complex script support” or “world-ready composer”, and these are optional because they can be slower. You may also consider using a different app to typeset the text.

- Read more about [complex text layout](https://en.wikipedia.org/wiki/Complex_text_layout) on Wikipedia.

### What are the Noto UI fonts for?

Many scripts form lines of text where all characters have roughly the same height, with only some letters extending below the baseline. User interface elements (menus, buttons, text boxes) in apps and on websites are often designed with a particular script in mind (often Latin).

However, letters in Arabic, Indic, and Southeast Asian scripts often connect both vertically and horizontally, so text for continuous reading needs a more generous line height. For those scripts, Noto includes an additional family with the **“UI”** suffix. These fonts are more compact vertically and have the same line height as the basic Noto Sans fonts.

| **Languages or scripts** | **Noto fonts to use** |
|---|---|
| Latin, Cyrillic, or Greek scripts | “Noto Sans” for user interfaces and for documents |
| Bengali, Devanagari, Gujarati, Gurmukhi, Kannada, Khmer, Lao, Malayalam, Myanmar, Oriya, Sinhala, Tamil, Telugu, Thai | “Noto Sans” with the script and “UI” suffixes for user interfaces with limited vertical space, fonts without the “UI” suffix for documents |
| Arabic | “Noto Sans Arabic UI” or “Noto Naskh Arabic UI” for user interfaces with limited vertical space, fonts without the UI suffix for documents |
| Armenian, Cherokee, Ethiopic, Georgian, Hebrew, and other scripts | Noto Sans with the script suffix for user interfaces and for documents |

### Which Noto fonts should I use for the Adlam script?

Noto has two Noto Sans fonts for the Adlam script that is used to write the Fulani language of Central and West Africa:

- Noto Sans Adlam, an unmodulated design with joining (cursive) letters, suitable for most texts.

- Noto Sans Adlam Unjoined, an unmodulated design with unjoined (block) letters, suitable for headlines and for educational content.

### Which Noto fonts should I use for the Arabic script?

Noto has six font families for the Arabic script:

- Noto Sans Arabic, an unmodulated design, suitable for all uses.

- Noto Sans Arabic UI, a variant of the Sans design for user interfaces with limited vertical space.

- Noto Kufi Arabic, a simplified unmodulated design in the Kufi (or Kufic) style of Arabic lettering. Noto Kufi Arabic is more simplified than Noto Sans Arabic, and is suitable for headlines and short texts for example in packaging or advertising.

- Noto Naskh Arabic, a modulated font in the Naskh style of Arabic calligraphy, which is suitable for longer texts. Noto Naskh Arabic can be used together with Noto Serif fonts for other scripts.

- Noto Naskh Arabic UI, a variant of the Naskh design for user interfaces with limited vertical space.

- Noto Nastaliq Urdu, a modulated cursive font in the Nastaliq style of Persian calligraphy, predominantly used for the Urdu language. The Nastaliq style was developed in Iran in the 15th century, and is used for the Persian, Urdu and Turkic languages that use the Arabic script.

### Which Noto fonts should I use for Chinese, Japanese or Korean?

The Noto collection includes two font families Chinese, Japanese and Korean languages: Noto Sans CJK, an unmodulated design, and Noto Serif CJK, a modulated design. Each of these families has 7 weights, and Noto Sans CJK is also available as a variable font. These fonts are available in language variants:

- Noto Sans CJK HK for the Traditional Chinese language variant used in Hong Kong.

- Noto Sans CJK JP and Noto Serif CJK JP for the Japanese language.

- Noto Sans CJK KR and Noto Serif CJK KR for the Korean language.

- Noto Sans CJK SC and Noto Serif CJK SC for the Simplified Chinese language variant used in the People’s Republic of China.

- Noto Sans CJK TC and Noto Serif CJK TC for the Traditional Chinese language variant used in Taiwan.

The Noto Sans CJK fonts contain all Han ideographs included in the Basic Multilingual Plane (BMP) of the Unicode Standard plus over 2,000 non-BMP Han ideographs.

### Which Noto fonts should I use for the Hebrew script?

Noto has three font families for the Hebrew script:

- Noto Sans Hebrew, an unmodulated design with a “square” skeleton and no stroke modulation, suitable for all uses.

- Noto Serif Hebrew, a modulated design with a “square” skeleton, suitable for longer texts.

- Noto Rashi Hebrew, a modulated design with a semi-cursive skeleton based on 15th-century Sephardic writing. It can be used for emphasis, complementing Noto Serif Hebrew. This type of design was used by early Hebrew typographers to set rabbinic commentary in the Talmud and Tanakh, while the primary text was set in a “square” Serif typeface.

### Which fonts should I use for the emoji characters?

Unicode includes over 3,500 emoji characters. Each operating system uses a different font format to represent the color emoji. The Google Fonts team recommends that you use the emoji fonts that are bundled with your app or system.

The Noto collection includes two fonts that contain emoji characters:

- Noto Emoji, a monochrome (non-color) font in TrueType-flavored OpenType format. It only contains about 25% of all encoded emoji but has scalable monochrome glyphs. It is intended for limited use in print publications, on monochrome displays, and in other scenarios where multiple colors cannot be reproduced.

- Noto Color Emoji, a multi-color font in the OpenType CBDT format. The font supports all emoji in Unicode 13 and beyond, but only works in Android, in Google Chrome and in apps that support the CBDT format. There is also a version of this font that works on Windows 10.

If you want to use the Noto emoji fonts, [download them](https://github.com/googlefonts/noto-emoji/tree/main/fonts) from Github.

### Why do some Noto Sans fonts have modulated strokes?

The Noto Sans fonts mostly have uniform strokes without pronounced endings. However, the Noto Sans fonts for some scripts do have stroke modulation if the user community of a particular script prefers it.

Traditionally, European scripts were of “serif” style. The “sans” style was introduced in the 19th century, and was originally not considered serious. Hence the term “grotesque” or “grotesk”, which is now a normal category of sans fonts. Today, typography on screens mostly uses sans designs but books or newspapers are still typeset with serif designs.

Not all writing systems have the same history. Users of some scripts prefer to always have stroke modulation. To ensure authenticity and to provide a pleasing reading experience for those communities, the Noto Sans fonts for that script have stroke modulation.

### Which Noto monospace fonts should I use?

Noto has several monospace fonts:

- Noto Sans Mono, a monospace font for languages written in Latin, Cyrillic and Greek scripts, in multiple weights.

- Noto Sans Mono CJK HK, a monospace font for the Traditional Chinese language variant used in Hong Kong, in two weights.

- Noto Sans Mono CJK JP, a monospace font for the Japanese language, in two weights.

- Noto Sans Mono CJK KR, a monospace font for the Korean language, in two weights.

- Noto Sans Mono CJK SC, a monospace font for the Simplified Chinese language variant used in the People’s Republic of China, in two weights.

- Noto Sans Mono CJK TC, a monospace font for the Traditional Chinese language variant used in Taiwan, in two weights.

For most use cases such as programming code, use Noto Sans Mono.

### When will language or script X be supported by Noto?

The Google Fonts team intends to support all scripts encoded by Unicode. This takes time. The team prioritizes the addition depending on the complexity of the script, on product and project needs, on the availability of script experts and designers, on the number and responsiveness of language reviewers, and on other factors.

### When will Noto support Klingon, Elvish etc.?

The [Script Encoding Initiative](https://linguistics.berkeley.edu/sei/scripts-not-encoded.html) lists scripts that are not yet included in the Unicode Standard. Once Klingon, Elvish etc. is included in Unicode, the Google Fonts team will consider adding it to Noto. [Contact](https://corp.unicode.org/reporting.html) the Unicode Consortium to encourage them to support your favourite script or language.

### Is Noto based on existing fonts?

The Latin characters in Noto Sans are based on earlier fonts designed by the same person, Steve Matteson, for Google: Droid Sans and Open Sans. The Latin characters in Noto Serif are based on Droid Serif. However, the the Noto fonts are undergoing regular reviews and revisions, and have more styles than the older fonts.

Noto Sans CJK is the same design as Adobe Han Sans, and the Latin characters are based on Adobe’s Source Sans Pro. Noto Serif CJK is the same design as Adobe Han Serif, and the Latin characters are based on Adobe’s Source Serif Pro.

The Noto fonts for many other scripts are original designs, while some are adapted from earlier existing designs. The Noto fonts for some scripts may be similar to existing fonts, often because the same designers created them, or because the fonts were modeled on the same calligraphic or typographic references.
