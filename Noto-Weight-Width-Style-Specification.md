
# Noto Weight & Width naming & numbering and Style naming specification


[TOC]



## Weights {#weights}

**LGC-mainstem-centric:** Weight values applied to Masters and Instances will be grounded in actual font distances: the normal width of the lowercase mainstem of the LGC  “normal” width fonts. In the case of Condensed, Expanded, or other width variants, we want to have the weight value of any given width match the numeric value of the _normal width_ which the master or instance is intended to accompany. 

Thus, if a given Bold master or instance has a value of 190 (equivalent to the dominant lowercase mainstem), and the corresponding Bold Condensed master or instance has a dominant lowercase mainstem weight of 162 (in order to optically blend with the Bold), we will want to set both the Bold and Bold Condensed masters to 190. By doing so, we ensure we have orthogonal interpolation spaces which are easily blended. 



![alt_text](images/PUB-Noto0.png "image_tooltip")
Bold with weight value of 190, dominant lc mainstem of 190




![alt_text](images/PUB-Noto1.png "image_tooltip")
Bold Condensed with weight value of 190, dominant lc mainstem of 162 {#bold-condensed-with-weight-value-of-190-dominant-lc-mainstem-of-162}


## Widths {#widths}

We are not producing a huge range of masters for different widths in the way we are with weights. Widths are generally specified as differences from the Regular or Normal width design, thus we have a degree of condensed or expanded. Our proposal is to number all normal width masters as 100, and the narrow masters as 70. A Semi Condensed instance would be 89, a true Condensed would be 79, with the master at 70 designated as Extra Condensed. If expanded widths are someday required, they might be somewhere between 120 and 130. A given width identifier in one script master would be designed to correspond to any other script with the same width value.


## Family, Style & Full Names {#family-style-&-full-names}

There are known limitation in string lengths. For example, on Windows, the Family name is used in menus and cannot exceed 31 characters in length. Similarly, Postscript names are limited to 63 characters according to the Open Font Format specification, although there is discussion throughout the industry as to whether or not this is a real restriction in practice. Style names have typically been kept as short as possible as well, despite the lack of concrete guidance on limitations in specific implementations.

For this specification we define family name and the complete style names without abbreviation. The software used for generating font files, will create name table specific names and handle abbreviation where necessary.

With this information as background, here is a set of naming guidelines.


#### Family Name {#family-name}

	Noto (“Sans”/”Sans UI”/”Serif”) <Script-name><variant><UI>


#### Style Name {#style-name}



1.  The stylename is the combined font-stretch (width), font-weight and font-style name, without spaces in the width and weight names, but spaces in between the parts.
1.  The weight is optionally preceded by the width (if not a normal width), but Regular is replaced by the width name.
1.  For Italics all style names end with “Italic”,  optionally preceded by width and weight, but Regular is not used in combination with Italic.



#### Weight Style Names {#weight-style-names}

	Thin 		usWeightClass: 100
	ExtraLight 	usWeightClass: 200
	Light 		usWeightClass: 300
	Regular 	usWeightClass: 400
	Medium 		usWeightClass: 500
	SemiBold 	usWeightClass: 600
	Bold 		usWeightClass: 700
	ExtraBold 	usWeightClass: 800
	Black 		usWeightClass: 900


#### Stretch Style Names {#stretch-style-names}

	ExtraCondensed 	usWidthClass: 2
	Condensed	usWidthClass: 3
	SemiCondensed	usWidthClass: 4
	(Normal)	usWidthClass: 5

	


#### Example Full names: {#example-full-names}

Noto Sans UI Thin
Noto Sans UI Bold Italic
Noto Sans UI Condensed ExtraBold Italic
Noto Serif Italic
Noto Sans Myanmar Thin
Noto Serif Myanmar SemiCondensed Light
Noto Serif Myanmar Condensed ExtraBold Italic


## Shipping Instances {#shipping-instances}

Instances need to be defined in the GlyphsApp sources that express the total number of variations in weight and width that can be accommodated by a given design.  Some scripts will not have width variants. Some scripts will not be able to be made as bold as the boldest LGC master. The designer should specify those cases, and include only those instances that render well.

Assuming that the masters of a non-Latin script are drawn and numbered to complement their corresponding LGC counterparts, the Instance interpolation values should also match those of their corresponding LGC counterparts. Below is a table of  weight and width values for each family.


##### Noto Sans interpolation values: {#noto-sans-interpolation-values}


<table>
  <tr>
   <td>
   </td>
   <td>Thin
   </td>
   <td>Extra Light
   </td>
   <td>Light
   </td>
   <td>Regular
   </td>
   <td>Medium
   </td>
   <td>Semi Bold
   </td>
   <td>Bold
   </td>
   <td>Extra Bold
   </td>
   <td>Black
   </td>
  </tr>
  <tr>
   <td>Normal
   </td>
   <td>26, 100
   </td>
   <td>39, 100
   </td>
   <td>58, 100
   </td>
   <td>90, 100
   </td>
   <td>108, 100
   </td>
   <td>128, 100
   </td>
   <td>151, 100
   </td>
   <td>169, 100
   </td>
   <td>190, 100
   </td>
  </tr>
  <tr>
   <td>Semi Cond.
   </td>
   <td>26, 89
   </td>
   <td>39, 89
   </td>
   <td>58, 89
   </td>
   <td>90, 89
   </td>
   <td>108, 89
   </td>
   <td>128, 89
   </td>
   <td>151, 89
   </td>
   <td>169, 89
   </td>
   <td>190, 89
   </td>
  </tr>
  <tr>
   <td>Cond.
   </td>
   <td>26, 79
   </td>
   <td>39, 79
   </td>
   <td>58, 79
   </td>
   <td>90, 79
   </td>
   <td>108, 79
   </td>
   <td>128, 79
   </td>
   <td>151, 79
   </td>
   <td>169, 79
   </td>
   <td>190, 79
   </td>
  </tr>
  <tr>
   <td>Extra Cond.
   </td>
   <td>26, 70
   </td>
   <td>39, 70
   </td>
   <td>58, 70
   </td>
   <td>90, 70
   </td>
   <td>108, 70
   </td>
   <td>128, 70
   </td>
   <td>151, 70
   </td>
   <td>169, 70
   </td>
   <td>190, 70
   </td>
  </tr>
</table>



##### Noto Serif  interpolation values: {#noto-serif-interpolation-values}


<table>
  <tr>
   <td>
   </td>
   <td>Thin
   </td>
   <td>Extra Light
   </td>
   <td>Light
   </td>
   <td>Regular
   </td>
   <td>Medium
   </td>
   <td>Semi Bold
   </td>
   <td>Bold
   </td>
   <td>Extra Bold
   </td>
   <td>Black
   </td>
  </tr>
  <tr>
   <td>Normal
   </td>
   <td>28, 100
   </td>
   <td>42,100
   </td>
   <td>64, 100
   </td>
   <td>94, 100
   </td>
   <td>110, 100
   </td>
   <td>130, 100
   </td>
   <td>152, 100
   </td>
   <td>175, 100
   </td>
   <td>194, 100
   </td>
  </tr>
  <tr>
   <td>Semi Cond.
   </td>
   <td>28, 89
   </td>
   <td>42,89
   </td>
   <td>64, 89
   </td>
   <td>94, 89
   </td>
   <td>110, 89
   </td>
   <td>130, 89
   </td>
   <td>152, 89
   </td>
   <td>175, 89
   </td>
   <td>194, 89
   </td>
  </tr>
  <tr>
   <td>Cond.
   </td>
   <td>28, 79
   </td>
   <td>42,79
   </td>
   <td>64, 79
   </td>
   <td>94, 79
   </td>
   <td>110, 79
   </td>
   <td>130, 79
   </td>
   <td>152, 79
   </td>
   <td>175, 79
   </td>
   <td>194, 79
   </td>
  </tr>
  <tr>
   <td>Extra Cond.
   </td>
   <td>28, 70
   </td>
   <td>42,70
   </td>
   <td>64, 70
   </td>
   <td>94, 70
   </td>
   <td>110, 70
   </td>
   <td>130, 70
   </td>
   <td>152, 70
   </td>
   <td>175, 70
   </td>
   <td>194, 70
   </td>
  </tr>
</table>



#### Document and UI Font instances {#document-and-ui-font-instances}

For UI instances weight and width values will be copied from their corresponding Document font values. If a UI font is shifted to fit into the UI ascender and descender the shift is stored as custom parameter: a filter defining a YOffset transformation. Both UI and document instances may have a “Keep Glyphs” custom parameters defining a Glyph subset. The “Reencode Glyphs” custom parameter may be used to change the default cmap encoding (added 2017).

_Note:_ _Whatever scheme of naming is used, there are going to be differences between Noto Sans and Roboto and Noto Sans CJK.  We could  make the “200” the same weight as Noto Sans CJK Thin with the same name, but not the same with Roboto Thin at the same time. The Roboto Black 900 is matching Noto Sans Extra Bold 800. We can match Roboto Medium in name, class and weight. But Roboto Medium is halfway Regular and Bold: that means you cannot have a Medium and a Semi-Bold, because the weight of the Medium is almost the weight that the Semi Bold should have._

_If the Noto Sans non-Latins UI fonts are linked to Roboto, it may not matter what they are named and what their widthClass is, when these properties are inherited from Roboto anyway. So that is the scenario our proposal assumes. But we can also define instances for the UI fonts that match Roboto in weight, name and classification. That would be a scheme where document and UI fonts have different instances in the glyphs deliverables._

_If the document fonts have 8 weights, then document and UI fonts can have the same instances._

_If the document fonts have 9 weight instances, to cover all of CSS/usWeightClass, and the UI fonts have an instance that matches Roboto Medium, then document and UI fonts will have different instances._

_The proposal is a means to find out what option is preferred._


#### OS/2 x-Height setting {#os-2-x-height-setting}

We will use 536 for all Noto Sans, Sans UI, Serif, Serif Display, etc,. The intention here is to ensure that these fonts will not be scaled to match relative heights, since we have designed these families to work together. We would like to set this as an explicit instance custom parameter, so that the master values can actually match the outline’s x-height, since that is needed for proper placement of anchors on lowercase glyphs. We will wait to request this functionality from Georg, until we get confirmation from Google that our approach will their needs.


#### Panose {#panose}

The chart below a chart showing the construction of the Noto values. See [Noto Panose Details](#noto-panose-details) for more.


<table>
  <tr>
   <td>Family type
   </td>
   <td>2 <em>Latin Text</em>
   </td>
   <td>for all
   </td>
  </tr>
  <tr>
   <td>Serif Type
   </td>
   <td>11 <em>Sans Serif</em>, 2 <em>Cove Serif</em>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Weight
   </td>
   <td><em>According to stem weight</em>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Proportion*
   </td>
   <td colspan="2" >2 normal and semi-cond., 6 Cond. and Extra-Cond., 9 for Monospaced
   </td>
  </tr>
  <tr>
   <td>Contrast
   </td>
   <td>4 Sans, 6 Serif, 8 Serif Display
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Stroke
   </td>
   <td>5 <em>Gradual/Vertical</em>
   </td>
   <td>for all
   </td>
  </tr>
  <tr>
   <td>Arm
   </td>
   <td>4 Sans, 5 Serif
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Form
   </td>
   <td>2 Roman, 9 Italic
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Midline
   </td>
   <td>2 <em>Standard Trimmed</em>
   </td>
   <td>for all
   </td>
  </tr>
  <tr>
   <td>xHeight
   </td>
   <td>4 <em>Constant/Large</em>
   </td>
   <td>for all
   </td>
  </tr>
</table>


_\*The proportion value is a mix of stylistic properties and character width. So it does not have a direct link to the width interpolation._


#### Style Linking {#style-linking}

Bold _is Bold of_ Regular

Semi Condensed Bold _is Bold of _Semi Condensed

Condensed Bold _is Bold of_ Condensed

Extra Condensed Bold _is Bold o_f Extra Condensed

Bold Italic _is Bold and Italic of_ Regular

Semi Condensed Bold Italic _is Bold and Italic of _Semi Condensed

Condensed Bold Italic _is Bold and Italic of_ Condensed

Extra Condensed Bold Italic _is Bold and Italic of_ Extra Condensed

Other Italics are Italic of the equivalent roman instances


#### Monotype Feature Files naming {#monotype-feature-files-naming}

We will name the files with the family name, followed by the numbers of weight and width interpolation values of the master, followed by the table tag. For GSUB files that apply to all weights, the interpolation values will be omitted. Where a GSUB source file is tied to specific masters, then for intermediate instances the nearest GSUB is to be used. GPOS values tables will typically apply to a single master, and named as such. The GPOS tables for intermediate instances will need to be interpolated from existing masters.

For Example:



*   Noto Sans Sinhala GDEF.txt
*   Noto Sans Sinhala GSUB.txt
*   Noto Sans Sinhala 58-100 GPOS.txt
*   Noto Sans Devanagari 90-100 GSUB.txt


#### Glyphs {#glyphs}

The glyph order is defined by a custom parameter at the font level.

Composite component glyphs that are never rendered on their own not are not set to export. To distinguish between component glyphs that can be used as component glyph in TrueType (and might optionally be exported anyway) and those that cannot, the latter will have a name starting with underscore.

Without the custom parameter “don’t use production names” is True, the source glyph names are expected to be renamed where needed. With the parameter, the “nice names” of the Glyphs source file are used with the layout table source files too and should be valid glyph names with regards to length and used characters.


### 

The following table is not part of the specification:


### Comparison of interpolation values  {#comparison-of-interpolation-values}

_The table puts side by side the interpolation weights of the above proposal, with estimated values of Roboto and Noto Sans CJK. It is interesting to see how these values compare if we were to attempt to support the 9 weights as defined in the CSS font-weight property. We are stuck with a regular at 90. So we cannot have as many weight below the regular as calculated by the formula’s of Pablo Impallari and Luc de Groot. But two intermediate light weights fit in easily. For practical use having 4 weights above the regular is sufficient. But having 3 below is important in order to have a lighter light that is useable: the extremely thin master isn’t very usable apart from it’s UI function._


<table>
  <tr>
   <td>The master weights
   </td>
   <td><strong>Updated proposal Noto Sans LCG</strong>
   </td>
   <td>Noto Sans CJK
   </td>
   <td>Roboto
   </td>
   <td>CSS font-weightin 9 equal steps
   </td>
   <td>CSS font-weight in 9 non-linear steps: Impallari method
   </td>
   <td>CSS font-weight in 9 non-linear steps: Luc(as) method
   </td>
   <td>Jelle’s 9 alternative trial and error and educated guess steps
   </td>
  </tr>
  <tr>
   <td>26
   </td>
   <td><strong>26</strong>
   </td>
   <td>
   </td>
   <td>26
   </td>
   <td>26
   </td>
   <td>26
   </td>
   <td>26
   </td>
   <td>26
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>35
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>35
   </td>
   <td>33
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td><strong>39 (new)</strong>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>40
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>47
   </td>
   <td>49
   </td>
   <td>43
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td><strong>58</strong>
   </td>
   <td>58
   </td>
   <td>59
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>55
   </td>
   <td>60
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>67
   </td>
   <td>67
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>70
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>80
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>90
   </td>
   <td><strong>90</strong>
   </td>
   <td>91
   </td>
   <td>92
   </td>
   <td>88
   </td>
   <td>89
   </td>
   <td>90
   </td>
   <td>90
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>106
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>108
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td><strong>118</strong>
   </td>
   <td>114
   </td>
   <td>120
   </td>
   <td>
   </td>
   <td>114
   </td>
   <td>116
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>124
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>129
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td><strong>141</strong>
   </td>
   <td>146
   </td>
   <td>145
   </td>
   <td>
   </td>
   <td>141
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>151
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>149
   </td>
   <td>
   </td>
   <td>148
   </td>
   <td>151
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td><strong>165</strong>
   </td>
   <td>
   </td>
   <td>167
   </td>
   <td>170
   </td>
   <td>167
   </td>
   <td>
   </td>
   <td>169
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>177
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>190
   </td>
   <td><strong>190</strong>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>190
   </td>
   <td>190
   </td>
   <td>190
   </td>
   <td>190
   </td>
  </tr>
</table>





## Noto Panose Details {#noto-panose-details}


<table>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>normal width
   </td>
   <td>semi condensed
   </td>
   <td>condensed
   </td>
   <td>extra Condensed
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>2 old style
   </td>
   <td>2 old style
   </td>
   <td>6 condensed
   </td>
   <td>6 condensed
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>interpl.
   </td>
   <td>100
   </td>
   <td>89
   </td>
   <td>79
   </td>
   <td>70
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>Sans
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>summary
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>26
   </td>
   <td>2 11 2 2 4 5 4 2 2 4
   </td>
   <td>2 11 2 2 4 5 4 2 2 4
   </td>
   <td>2 11 2 6 4 5 4 2 2 4
   </td>
   <td>2 11 2 6 4 5 4 2 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>39
   </td>
   <td>2 11 3 2 4 5 4 2 2 4
   </td>
   <td>2 11 3 2 4 5 4 2 2 4
   </td>
   <td>2 11 3 6 4 5 4 2 2 4
   </td>
   <td>2 11 3 6 4 5 4 2 2 4
   </td>
  </tr>
  <tr>
   <td>Family type
   </td>
   <td>2 Latin Text
   </td>
   <td>for all
   </td>
   <td>
   </td>
   <td>58
   </td>
   <td>2 11 4 2 4 5 4 2 2 4
   </td>
   <td>2 11 4 2 4 5 4 2 2 4
   </td>
   <td>2 11 4 6 4 5 4 2 2 4
   </td>
   <td>2 11 4 6 4 5 4 2 2 4
   </td>
  </tr>
  <tr>
   <td>Serif Type
   </td>
   <td>11 Sans Serif, 2 Cove Serif
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>90
   </td>
   <td>2 11 5 2 4 5 4 2 2 4
   </td>
   <td>2 11 5 2 4 5 4 2 2 4
   </td>
   <td>2 11 5 6 4 5 4 2 2 4
   </td>
   <td>2 11 5 6 4 5 4 2 2 4
   </td>
  </tr>
  <tr>
   <td>Weight
   </td>
   <td><em>According to stem weight</em>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>106
   </td>
   <td>2 11 6 2 4 5 4 2 2 4
   </td>
   <td>2 11 6 2 4 5 4 2 2 4
   </td>
   <td>2 11 6 6 4 5 4 2 2 4
   </td>
   <td>2 11 6 6 4 5 4 2 2 4
   </td>
  </tr>
  <tr>
   <td>Proportion
   </td>
   <td colspan="2" >2 normal and semi-cond., 6 Cond and Extra-Cond, 9 for Monospaced
   </td>
   <td>
   </td>
   <td>119
   </td>
   <td>2 11 6 2 4 5 4 2 2 4
   </td>
   <td>2 11 6 2 4 5 4 2 2 4
   </td>
   <td>2 11 6 6 4 5 4 2 2 4
   </td>
   <td>2 11 6 6 4 5 4 2 2 4
   </td>
  </tr>
  <tr>
   <td>Contrast
   </td>
   <td>4 Sans, 6 Serif, 8 Serif Display
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>124
   </td>
   <td>2 11 7 2 4 5 4 2 2 4
   </td>
   <td>2 11 7 2 4 5 4 2 2 4
   </td>
   <td>2 11 7 6 4 5 4 2 2 4
   </td>
   <td>2 11 7 6 4 5 4 2 2 4
   </td>
  </tr>
  <tr>
   <td>Stroke
   </td>
   <td>5 Gradual/Vertical
   </td>
   <td>for all
   </td>
   <td>
   </td>
   <td>141
   </td>
   <td>2 11 8 2 4 5 4 2 2 4
   </td>
   <td>2 11 8 2 4 5 4 2 2 4
   </td>
   <td>2 11 8 6 4 5 4 2 2 4
   </td>
   <td>2 11 8 6 4 5 4 2 2 4
   </td>
  </tr>
  <tr>
   <td>Arm
   </td>
   <td>4 Sans, 5 Serif
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>151
   </td>
   <td>2 11 8 2 4 5 4 2 2 4
   </td>
   <td>2 11 8 2 4 5 4 2 2 4
   </td>
   <td>2 11 8 6 4 5 4 2 2 4
   </td>
   <td>2 11 8 6 4 5 4 2 2 4
   </td>
  </tr>
  <tr>
   <td>Form
   </td>
   <td>2 Roman, 9 Italic
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>165
   </td>
   <td>2 11 9 2 4 5 4 2 2 4
   </td>
   <td>2 11 9 2 4 5 4 2 2 4
   </td>
   <td>2 11 9 6 4 5 4 2 2 4
   </td>
   <td>2 11 9 6 4 5 4 2 2 4
   </td>
  </tr>
  <tr>
   <td>Midline
   </td>
   <td>2 Standard Trimmed
   </td>
   <td>for all
   </td>
   <td>
   </td>
   <td>190
   </td>
   <td>2 11 10 2 4 5 4 2 2 4
   </td>
   <td>2 11 10 2 4 5 4 2 2 4
   </td>
   <td>2 11 10 6 4 5 4 2 2 4
   </td>
   <td>2 11 10 6 4 5 4 2 2 4
   </td>
  </tr>
  <tr>
   <td>xHeight
   </td>
   <td>4 Constant/Large
   </td>
   <td>for all
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>Sans Italic
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>26
   </td>
   <td>2 11 9 2 4 5 4 9 2 4
   </td>
   <td>2 11 9 2 4 5 4 9 2 4
   </td>
   <td>2 11 2 6 4 5 4 9 2 4
   </td>
   <td>2 11 2 6 4 5 4 9 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>39
   </td>
   <td>2 11 3 2 4 5 4 9 2 4
   </td>
   <td>2 11 3 2 4 5 4 9 2 4
   </td>
   <td>2 11 3 6 4 5 4 9 2 4
   </td>
   <td>2 11 3 6 4 5 4 9 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>58
   </td>
   <td>2 11 4 2 4 5 4 9 2 4
   </td>
   <td>2 11 4 2 4 5 4 9 2 4
   </td>
   <td>2 11 4 6 4 5 4 9 2 4
   </td>
   <td>2 11 4 6 4 5 4 9 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>90
   </td>
   <td>2 11 5 2 4 5 4 9 2 4
   </td>
   <td>2 11 5 2 4 5 4 9 2 4
   </td>
   <td>2 11 5 6 4 5 4 9 2 4
   </td>
   <td>2 11 5 6 4 5 4 9 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>106
   </td>
   <td>2 11 6 2 4 5 4 9 2 4
   </td>
   <td>2 11 6 2 4 5 4 9 2 4
   </td>
   <td>2 11 6 6 4 5 4 9 2 4
   </td>
   <td>2 11 6 6 4 5 4 9 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>119
   </td>
   <td>2 11 6 2 4 5 4 9 2 4
   </td>
   <td>2 11 6 2 4 5 4 9 2 4
   </td>
   <td>2 11 6 6 4 5 4 9 2 4
   </td>
   <td>2 11 6 6 4 5 4 9 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>124
   </td>
   <td>2 11 7 2 4 5 4 9 2 4
   </td>
   <td>2 11 7 2 4 5 4 9 2 4
   </td>
   <td>2 11 7 6 4 5 4 9 2 4
   </td>
   <td>2 11 7 6 4 5 4 9 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>141
   </td>
   <td>2 11 8 2 4 5 4 9 2 4
   </td>
   <td>2 11 8 2 4 5 4 9 2 4
   </td>
   <td>2 11 8 6 4 5 4 9 2 4
   </td>
   <td>2 11 8 6 4 5 4 9 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>151
   </td>
   <td>2 11 8 2 4 5 4 9 2 4
   </td>
   <td>2 11 8 2 4 5 4 9 2 4
   </td>
   <td>2 11 8 6 4 5 4 9 2 4
   </td>
   <td>2 11 8 6 4 5 4 9 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>165
   </td>
   <td>2 11 9 2 4 5 4 9 2 4
   </td>
   <td>2 11 9 2 4 5 4 9 2 4
   </td>
   <td>2 11 9 6 4 5 4 9 2 4
   </td>
   <td>2 11 9 6 4 5 4 9 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>190
   </td>
   <td>2 11 10 2 4 5 4 9 2 4
   </td>
   <td>2 11 10 2 4 5 4 9 2 4
   </td>
   <td>2 11 10 6 4 5 4 9 2 4
   </td>
   <td>2 11 10 6 4 5 4 9 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>Serif
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>28
   </td>
   <td>2 2 2 2 6 5 5 2 2 4
   </td>
   <td>2 2 2 2 6 5 5 2 2 4
   </td>
   <td>2 2 2 6 6 5 5 2 2 4
   </td>
   <td>2 2 2 6 6 5 5 2 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>42
   </td>
   <td>2 2 3 2 6 5 5 2 2 4
   </td>
   <td>2 2 3 2 6 5 5 2 2 4
   </td>
   <td>2 2 3 6 6 5 5 2 2 4
   </td>
   <td>2 2 3 6 6 5 5 2 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>64
   </td>
   <td>2 2 4 2 6 5 5 2 2 4
   </td>
   <td>2 2 4 2 6 5 5 2 2 4
   </td>
   <td>2 2 4 6 6 5 5 2 2 4
   </td>
   <td>2 2 4 6 6 5 5 2 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>94
   </td>
   <td>2 2 5 2 6 5 5 2 2 4
   </td>
   <td>2 2 5 2 6 5 5 2 2 4
   </td>
   <td>2 2 5 6 6 5 5 2 2 4
   </td>
   <td>2 2 5 6 6 5 5 2 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>2 2 6 2 6 5 5 2 2 4
   </td>
   <td>2 2 6 2 6 5 5 2 2 4
   </td>
   <td>2 2 6 6 6 5 5 2 2 4
   </td>
   <td>2 2 6 6 6 5 5 2 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>2 2 6 2 6 5 5 2 2 4
   </td>
   <td>2 2 6 2 6 5 5 2 2 4
   </td>
   <td>2 2 6 6 6 5 5 2 2 4
   </td>
   <td>2 2 6 6 6 5 5 2 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>125
   </td>
   <td>2 2 7 2 6 5 5 2 2 4
   </td>
   <td>2 2 7 2 6 5 5 2 2 4
   </td>
   <td>2 2 7 6 6 5 5 2 2 4
   </td>
   <td>2 2 7 6 6 5 5 2 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>2 2 8 2 6 5 5 2 2 4
   </td>
   <td>2 2 8 2 6 5 5 2 2 4
   </td>
   <td>2 2 8 6 6 5 5 2 2 4
   </td>
   <td>2 2 8 6 6 5 5 2 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>152
   </td>
   <td>2 2 8 2 6 5 5 2 2 4
   </td>
   <td>2 2 8 2 6 5 5 2 2 4
   </td>
   <td>2 2 8 6 6 5 5 2 2 4
   </td>
   <td>2 2 8 6 6 5 5 2 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>175
   </td>
   <td>2 2 9 2 6 5 5 2 2 4
   </td>
   <td>2 2 9 2 6 5 5 2 2 4
   </td>
   <td>2 2 9 6 6 5 5 2 2 4
   </td>
   <td>2 2 9 6 6 5 5 2 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>194
   </td>
   <td>2 2 10 2 6 5 5 2 2 4
   </td>
   <td>2 2 10 2 6 5 5 2 2 4
   </td>
   <td>2 2 10 6 6 5 5 2 2 4
   </td>
   <td>2 2 10 6 6 5 5 2 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>Serif Italic
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>28
   </td>
   <td>2 2 2 2 6 5 5 9 2 4
   </td>
   <td>2 2 2 2 6 5 5 9 2 4
   </td>
   <td>2 2 2 6 6 5 5 9 2 4
   </td>
   <td>2 2 2 6 6 5 5 9 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>42
   </td>
   <td>2 2 3 2 6 5 5 9 2 4
   </td>
   <td>2 2 3 2 6 5 5 9 2 4
   </td>
   <td>2 2 3 6 6 5 5 9 2 4
   </td>
   <td>2 2 3 6 6 5 5 9 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>64
   </td>
   <td>2 2 4 2 6 5 5 9 2 4
   </td>
   <td>2 2 4 2 6 5 5 9 2 4
   </td>
   <td>2 2 4 6 6 5 5 9 2 4
   </td>
   <td>2 2 4 6 6 5 5 9 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>94
   </td>
   <td>2 2 5 2 6 5 5 9 2 4
   </td>
   <td>2 2 5 2 6 5 5 9 2 4
   </td>
   <td>2 2 5 6 6 5 5 9 2 4
   </td>
   <td>2 2 5 6 6 5 5 9 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>2 2 6 2 6 5 5 9 2 4
   </td>
   <td>2 2 6 2 6 5 5 9 2 4
   </td>
   <td>2 2 6 6 6 5 5 9 2 4
   </td>
   <td>2 2 6 6 6 5 5 9 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>2 2 6 2 6 5 5 9 2 4
   </td>
   <td>2 2 6 2 6 5 5 9 2 4
   </td>
   <td>2 2 6 6 6 5 5 9 2 4
   </td>
   <td>2 2 6 6 6 5 5 9 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>125
   </td>
   <td>2 2 7 2 6 5 5 9 2 4
   </td>
   <td>2 2 7 2 6 5 5 9 2 4
   </td>
   <td>2 2 7 6 6 5 5 9 2 4
   </td>
   <td>2 2 7 6 6 5 5 9 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>2 2 8 2 6 5 5 9 2 4
   </td>
   <td>2 2 8 2 6 5 5 9 2 4
   </td>
   <td>2 2 8 6 6 5 5 9 2 4
   </td>
   <td>2 2 8 6 6 5 5 9 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>152
   </td>
   <td>2 2 8 2 6 5 5 9 2 4
   </td>
   <td>2 2 8 2 6 5 5 9 2 4
   </td>
   <td>2 2 8 6 6 5 5 9 2 4
   </td>
   <td>2 2 8 6 6 5 5 9 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>175
   </td>
   <td>2 2 9 2 6 5 5 9 2 4
   </td>
   <td>2 2 9 2 6 5 5 9 2 4
   </td>
   <td>2 2 9 6 6 5 5 9 2 4
   </td>
   <td>2 2 9 6 6 5 5 9 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>194
   </td>
   <td>2 2 10 2 6 5 5 9 2 4
   </td>
   <td>2 2 10 2 6 5 5 9 2 4
   </td>
   <td>2 2 10 6 6 5 5 9 2 4
   </td>
   <td>2 2 10 6 6 5 5 9 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>Display Serif
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>28
   </td>
   <td>2 2 2 2 8 5 5 2 2 4
   </td>
   <td>2 2 2 2 8 5 5 2 2 4
   </td>
   <td>2 2 2 6 8 5 5 2 2 4
   </td>
   <td>2 2 2 6 8 5 5 2 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>42
   </td>
   <td>2 2 3 2 8 5 5 2 2 4
   </td>
   <td>2 2 3 2 8 5 5 2 2 4
   </td>
   <td>2 2 3 6 8 5 5 2 2 4
   </td>
   <td>2 2 3 6 8 5 5 2 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>64
   </td>
   <td>2 2 4 2 8 5 5 2 2 4
   </td>
   <td>2 2 4 2 8 5 5 2 2 4
   </td>
   <td>2 2 4 6 8 5 5 2 2 4
   </td>
   <td>2 2 4 6 8 5 5 2 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>94
   </td>
   <td>2 2 5 2 8 5 5 2 2 4
   </td>
   <td>2 2 5 2 8 5 5 2 2 4
   </td>
   <td>2 2 5 6 8 5 5 2 2 4
   </td>
   <td>2 2 5 6 8 5 5 2 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>2 2 6 2 8 5 5 2 2 4
   </td>
   <td>2 2 6 2 8 5 5 2 2 4
   </td>
   <td>2 2 6 6 8 5 5 2 2 4
   </td>
   <td>2 2 6 6 8 5 5 2 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>2 2 6 2 8 5 5 2 2 4
   </td>
   <td>2 2 6 2 8 5 5 2 2 4
   </td>
   <td>2 2 6 6 8 5 5 2 2 4
   </td>
   <td>2 2 6 6 8 5 5 2 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>125
   </td>
   <td>2 2 7 2 8 5 5 2 2 4
   </td>
   <td>2 2 7 2 8 5 5 2 2 4
   </td>
   <td>2 2 7 6 8 5 5 2 2 4
   </td>
   <td>2 2 7 6 8 5 5 2 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>2 2 8 2 8 5 5 2 2 4
   </td>
   <td>2 2 8 2 8 5 5 2 2 4
   </td>
   <td>2 2 8 6 8 5 5 2 2 4
   </td>
   <td>2 2 8 6 8 5 5 2 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>152
   </td>
   <td>2 2 8 2 8 5 5 2 2 4
   </td>
   <td>2 2 8 2 8 5 5 2 2 4
   </td>
   <td>2 2 8 6 8 5 5 2 2 4
   </td>
   <td>2 2 8 6 8 5 5 2 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>175
   </td>
   <td>2 2 9 2 8 5 5 2 2 4
   </td>
   <td>2 2 9 2 8 5 5 2 2 4
   </td>
   <td>2 2 9 6 8 5 5 2 2 4
   </td>
   <td>2 2 9 6 8 5 5 2 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>194
   </td>
   <td>2 2 10 2 8 5 5 2 2 4
   </td>
   <td>2 2 10 2 8 5 5 2 2 4
   </td>
   <td>2 2 10 6 8 5 5 2 2 4
   </td>
   <td>2 2 10 6 8 5 5 2 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>Display Serif Italic
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>28
   </td>
   <td>2 2 2 2 8 5 5 9 2 4
   </td>
   <td>2 2 2 2 8 5 5 9 2 4
   </td>
   <td>2 2 2 6 8 5 5 9 2 4
   </td>
   <td>2 2 2 6 8 5 5 9 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>42
   </td>
   <td>2 2 3 2 8 5 5 9 2 4
   </td>
   <td>2 2 3 2 8 5 5 9 2 4
   </td>
   <td>2 2 3 6 8 5 5 9 2 4
   </td>
   <td>2 2 3 6 8 5 5 9 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>64
   </td>
   <td>2 2 4 2 8 5 5 9 2 4
   </td>
   <td>2 2 4 2 8 5 5 9 2 4
   </td>
   <td>2 2 4 6 8 5 5 9 2 4
   </td>
   <td>2 2 4 6 8 5 5 9 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>94
   </td>
   <td>2 2 5 2 8 5 5 9 2 4
   </td>
   <td>2 2 5 2 8 5 5 9 2 4
   </td>
   <td>2 2 5 6 8 5 5 9 2 4
   </td>
   <td>2 2 5 6 8 5 5 9 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>2 2 6 2 8 5 5 9 2 4
   </td>
   <td>2 2 6 2 8 5 5 9 2 4
   </td>
   <td>2 2 6 6 8 5 5 9 2 4
   </td>
   <td>2 2 6 6 8 5 5 9 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>2 2 6 2 8 5 5 9 2 4
   </td>
   <td>2 2 6 2 8 5 5 9 2 4
   </td>
   <td>2 2 6 6 8 5 5 9 2 4
   </td>
   <td>2 2 6 6 8 5 5 9 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>125
   </td>
   <td>2 2 7 2 8 5 5 9 2 4
   </td>
   <td>2 2 7 2 8 5 5 9 2 4
   </td>
   <td>2 2 7 6 8 5 5 9 2 4
   </td>
   <td>2 2 7 6 8 5 5 9 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>2 2 8 2 8 5 5 9 2 4
   </td>
   <td>2 2 8 2 8 5 5 9 2 4
   </td>
   <td>2 2 8 6 8 5 5 9 2 4
   </td>
   <td>2 2 8 6 8 5 5 9 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>152
   </td>
   <td>2 2 8 2 8 5 5 9 2 4
   </td>
   <td>2 2 8 2 8 5 5 9 2 4
   </td>
   <td>2 2 8 6 8 5 5 9 2 4
   </td>
   <td>2 2 8 6 8 5 5 9 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>175
   </td>
   <td>2 2 9 2 8 5 5 9 2 4
   </td>
   <td>2 2 9 2 8 5 5 9 2 4
   </td>
   <td>2 2 9 6 8 5 5 9 2 4
   </td>
   <td>2 2 9 6 8 5 5 9 2 4
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>194
   </td>
   <td>2 2 10 2 8 5 5 9 2 4
   </td>
   <td>2 2 10 2 8 5 5 9 2 4
   </td>
   <td>2 2 10 6 8 5 5 9 2 4
   </td>
   <td>2 2 10 6 8 5 5 9 2 4
   </td>
  </tr>
</table>


