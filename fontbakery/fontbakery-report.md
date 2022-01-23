## Fontbakery report

Fontbakery version: 0.8.3

<details>
<summary><b>[12] Rubik-Light.ttf</b></summary>
<details>
<summary>💔 <b>ERROR:</b> Check samples can be rendered.</summary>

* [com.google.fonts/check/metadata/can_render_samples](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/metadata/can_render_samples)
<pre>--- Rationale ---
In order to prevent tofu from being seen on fonts.google.com, this check
verifies that all samples provided on METADATA.pb can be properly rendered by
the font.</pre>

* 💔 **ERROR** Failed with AttributeError: 'NoneType' object has no attribute 'sample_glyphs'

</details>
<details>
<summary>🔥 <b>FAIL:</b> Check license file has good copyright string.</summary>

* [com.google.fonts/check/license/OFL_copyright](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/license/OFL_copyright)
<pre>--- Rationale ---
An OFL.txt file&#x27;s first line should be the font copyright e.g:
&quot;Copyright 2019 The Montserrat Project Authors
(https://github.com/julietaula/montserrat)&quot;</pre>

* 🔥 **FAIL** First line in license file does not match expected format: "copyright 20** the my font project authors (https://github.com/googlefonts/my-font-repository)"

</details>
<details>
<summary>⚠ <b>WARN:</b> Checking OS/2 achVendID.</summary>

* [com.google.fonts/check/vendor_id](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/vendor_id)
<pre>--- Rationale ---
Microsoft keeps a list of font vendors and their respective contact info. This
list is updated regularly and is indexed by a 4-char &quot;Vendor ID&quot; which is stored
in the achVendID field of the OS/2 table.
Registering your ID is not mandatory, but it is a good practice since some
applications may display the type designer / type foundry contact info on some
dialog and also because that info will be visible on Microsoft&#x27;s website:
https://docs.microsoft.com/en-us/typography/vendors/
This check verifies whether or not a given font&#x27;s vendor ID is registered in
that list or if it has some of the default values used by the most common font
editors.
Each new FontBakery release includes a cached copy of that list of vendor IDs.
If you registered recently, you&#x27;re safe to ignore warnings emitted by this
check, since your ID will soon be included in one of our upcoming releases.</pre>

* ⚠ **WARN** OS/2 VendorID value 'NONE' is not yet recognized. If you registered it recently, then it's safe to ignore this warning message. Otherwise, you should set it to your own unique 4 character code, and register it with Microsoft at https://www.microsoft.com/typography/links/vendorlist.aspx
 [code: unknown]

</details>
<details>
<summary>⚠ <b>WARN:</b> Font has old ttfautohint applied?</summary>

* [com.google.fonts/check/old_ttfautohint](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/old_ttfautohint)
<pre>--- Rationale ---
Check if font has been hinted with an outdated version of ttfautohint.</pre>

* ⚠ **WARN** ttfautohint used in font = 1.8.3; latest = 1.8.4; Need to re-run with the newer version! [code: old-ttfa]

</details>
<details>
<summary>⚠ <b>WARN:</b> Glyphs are similiar to Google Fonts version?</summary>

* [com.google.fonts/check/production_glyphs_similarity](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/production_glyphs_similarity)

* ⚠ **WARN** Following glyphs differ greatly from Google Fonts version: [Euro, Hbar, uni05B8, uni20AE, uni20B4, yen]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check if each glyph has the recommended amount of contours.</summary>

* [com.google.fonts/check/contour_count](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/contour_count)
<pre>--- Rationale ---
Visually QAing thousands of glyphs by hand is tiring. Most glyphs can only be
constructured in a handful of ways. This means a glyph&#x27;s contour count will only
differ slightly amongst different fonts, e.g a &#x27;g&#x27; could either be 2 or 3
contours, depending on whether its double story or single story.
However, a quotedbl should have 2 contours, unless the font belongs to a display
family.
This check currently does not cover variable fonts because there&#x27;s plenty of
alternative ways of constructing glyphs with multiple outlines for each feature
in a VarFont. The expected contour count data for this check is currently
optimized for the typical construction of glyphs in static fonts.</pre>

* ⚠ **WARN** This check inspects the glyph outlines and detects the total number of contours in each of them. The expected values are infered from the typical ammounts of contours observed in a large collection of reference font families. The divergences listed below may simply indicate a significantly different design on some of your glyphs. On the other hand, some of these may flag actual bugs in the font such as glyphs mapped to an incorrect codepoint. Please consider reviewing the design and codepoint assignment of these to make sure they are correct.

The following glyphs do not have the recommended number of contours:

Glyph name: uni0493	Contours detected: 2	Expected: 1
Glyph name: ustraitstrokecy	Contours detected: 2	Expected: 1
Glyph name: fi	Contours detected: 1	Expected: 3
Glyph name: fl	Contours detected: 1	Expected: 2
Glyph name: uni0493	Contours detected: 2	Expected: 1 [code: contour-count]

</details>
<details>
<summary>⚠ <b>WARN:</b> Is there kerning info for non-ligated sequences?</summary>

* [com.google.fonts/check/kerning_for_non_ligated_sequences](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/kerning_for_non_ligated_sequences)
<pre>--- Rationale ---
Fonts with ligatures should have kerning on the corresponding non-ligated
sequences for text where ligatures aren&#x27;t used (eg
https://github.com/impallari/Raleway/issues/14).</pre>

* ⚠ **WARN** GPOS table lacks kerning info for the following non-ligated sequences:
	- f + f
	- f + i
	- i + f
	- f + l
	- l + f
	- i + l

   [code: lacks-kern-info]

</details>
<details>
<summary>⚠ <b>WARN:</b> Ensure fonts have ScriptLangTags declared on the 'meta' table.</summary>

* [com.google.fonts/check/meta/script_lang_tags](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/meta/script_lang_tags)
<pre>--- Rationale ---
The OpenType &#x27;meta&#x27; table originated at Apple. Microsoft added it to OT with
just two DataMap records:
- dlng: comma-separated ScriptLangTags that indicate which scripts, or languages
and scripts, with possible variants, the font is designed for
- slng: comma-separated ScriptLangTags that indicate which scripts, or languages
and scripts, with possible variants, the font supports
The slng structure is intended to describe which languages and scripts the font
overall supports. For example, a Traditional Chinese font that also contains
Latin characters, can indicate Hant,Latn, showing that it supports Hant, the
Traditional Chinese variant of the Hani script, and it also supports the Latn
script
The dlng structure is far more interesting. A font may contain various glyphs,
but only a particular subset of the glyphs may be truly &quot;leading&quot; in the design,
while other glyphs may have been included for technical reasons. Such a
Traditional Chinese font could only list Hant there, showing that it’s designed
for Traditional Chinese, but the font would omit Latn, because the developers
don’t think the font is really recommended for purely Latin-script use.
The tags used in the structures can comprise just script, or also language and
script. For example, if a font has Bulgarian Cyrillic alternates in the locl
feature for the cyrl BGR OT languagesystem, it could also indicate in dlng
explicitly that it supports bul-Cyrl. (Note that the scripts and languages in
meta use the ISO language and script codes, not the OpenType ones).
This check ensures that the font has the meta table containing the slng and dlng
structures.
All families in the Google Fonts collection should contain the &#x27;meta&#x27; table.
Windows 10 already uses it when deciding on which fonts to fall back to. The
Google Fonts API and also other environments could use the data for smarter
filtering. Most importantly, those entries should be added to the Noto fonts.
In the font making process, some environments store this data in external files
already. But the meta table provides a convenient way to store this inside the
font file, so some tools may add the data, and unrelated tools may read this
data. This makes the solution much more portable and universal.</pre>

* ⚠ **WARN** This font file does not have a 'meta' table. [code: lacks-meta-table]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check font contains no unreachable glyphs</summary>

* [com.google.fonts/check/unreachable_glyphs](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/universal.html#com.google.fonts/check/unreachable_glyphs)
<pre>--- Rationale ---
Glyphs are either accessible directly through Unicode codepoints or through
substitution rules. Any glyphs not accessible by either of these means are
redundant and serve only to increase the font&#x27;s file size.</pre>

* ⚠ **WARN** The following glyphs could not be reached by codepoint or substitution rules:
 - Euro.BRACKET.125
 - parenright.denominator
 - .null
 - yen.BRACKET.125
 - parenleft.numerator
 - uni030C.alt
 - brevecombcy
 - parenleft.denominator
 - uni20B4.BRACKET.125 
 - parenright.numerator
 [code: unreachable-glyphs]

</details>
<details>
<summary>⚠ <b>WARN:</b> Are there any misaligned on-curve points?</summary>

* [com.google.fonts/check/outline_alignment_miss](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_alignment_miss)
<pre>--- Rationale ---
This check heuristically looks for on-curve points which are close to, but do
not sit on, significant boundary coordinates. For example, a point which has a
Y-coordinate of 1 or -1 might be a misplaced baseline point. As well as the
baseline, here we also check for points near the x-height (but only for lower
case Latin letters), cap-height, ascender and descender Y coordinates.
Not all such misaligned curve points are a mistake, and sometimes the design may
call for points in locations near the boundaries. As this check is liable to
generate significant numbers of false positives, it will pass if there are more
than 100 reported misalignments.</pre>

* ⚠ **WARN** The following glyphs have on-curve points which have potentially incorrect y coordinates:
	* parenleft (U+0028): X=204.0,Y=698.5 (should be at cap-height 700?)
	* parenright (U+0029): X=115.0,Y=698.5 (should be at cap-height 700?)
	* one (U+0031): X=263.0,Y=699.0 (should be at cap-height 700?)
	* braceright (U+007D): X=197.0,Y=699.5 (should be at cap-height 700?)
	* questiondown (U+00BF): X=97.0,Y=-2.0 (should be at baseline 0?)
	* aogonek (U+0105): X=445.0,Y=1.0 (should be at baseline 0?)
	* eogonek (U+0119): X=213.0,Y=-2.0 (should be at baseline 0?)
	* uogonek (U+0173): X=485.0,Y=-2.0 (should be at baseline 0?)
	* uni0409 (U+0409): X=43.0,Y=1.0 (should be at baseline 0?)
	* uni0409 (U+0409): X=43.0,Y=1.0 (should be at baseline 0?) and 10 more. [code: found-misalignments]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do any segments have colinear vectors?</summary>

* [com.google.fonts/check/outline_colinear_vectors](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_colinear_vectors)
<pre>--- Rationale ---
This check looks for consecutive line segments which have the same angle. This
normally happens if an outline point has been added by accident.
This check is not run for variable fonts, as they may legitimately have colinear
vectors.</pre>

* ⚠ **WARN** The following glyphs have colinear vectors:
	* uni05B3 (U+05B3): L<<26.0,-131.0>--<26.0,-134.0>> -> L<<26.0,-134.0>--<26.0,-223.0>>
	* uni05C7 (U+05C7): L<<26.0,-131.0>--<26.0,-134.0>> -> L<<26.0,-134.0>--<26.0,-223.0>>
	* uni05DC (U+05DC): L<<173.0,513.0>--<170.0,513.0>> -> L<<170.0,513.0>--<92.0,514.0>>
	* uni05DC (U+05DC): L<<207.0,513.0>--<173.0,513.0>> -> L<<173.0,513.0>--<170.0,513.0>>
	* uniFB2F (U+FB2F): L<<311.0,-131.0>--<311.0,-134.0>> -> L<<311.0,-134.0>--<311.0,-223.0>>
	* uniFB3C (U+FB3C): L<<173.0,513.0>--<170.0,513.0>> -> L<<170.0,513.0>--<92.0,514.0>> and uniFB3C (U+FB3C): L<<207.0,513.0>--<173.0,513.0>> -> L<<173.0,513.0>--<170.0,513.0>> [code: found-colinear-vectors]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do outlines contain any semi-vertical or semi-horizontal lines?</summary>

* [com.google.fonts/check/outline_semi_vertical](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_semi_vertical)
<pre>--- Rationale ---
This check detects line segments which are nearly, but not quite, exactly
horizontal or vertical. Sometimes such lines are created by design, but often
they are indicative of a design error.
This check is disabled for italic styles, which often contain nearly-upright
lines.</pre>

* ⚠ **WARN** The following glyphs have semi-vertical/semi-horizontal lines:
 * uni0434 (U+0434): L<<133.0,58.0>--<409.0,60.0>> and uni0446 (U+0446): L<<495.0,498.0>--<494.0,58.0>> [code: found-semi-vertical]

</details>
<br>
</details>
<details>
<summary><b>[12] Rubik-SemiBold.ttf</b></summary>
<details>
<summary>💔 <b>ERROR:</b> Check samples can be rendered.</summary>

* [com.google.fonts/check/metadata/can_render_samples](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/metadata/can_render_samples)
<pre>--- Rationale ---
In order to prevent tofu from being seen on fonts.google.com, this check
verifies that all samples provided on METADATA.pb can be properly rendered by
the font.</pre>

* 💔 **ERROR** Failed with AttributeError: 'NoneType' object has no attribute 'sample_glyphs'

</details>
<details>
<summary>🔥 <b>FAIL:</b> Check license file has good copyright string.</summary>

* [com.google.fonts/check/license/OFL_copyright](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/license/OFL_copyright)
<pre>--- Rationale ---
An OFL.txt file&#x27;s first line should be the font copyright e.g:
&quot;Copyright 2019 The Montserrat Project Authors
(https://github.com/julietaula/montserrat)&quot;</pre>

* 🔥 **FAIL** First line in license file does not match expected format: "copyright 20** the my font project authors (https://github.com/googlefonts/my-font-repository)"

</details>
<details>
<summary>⚠ <b>WARN:</b> Checking OS/2 achVendID.</summary>

* [com.google.fonts/check/vendor_id](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/vendor_id)
<pre>--- Rationale ---
Microsoft keeps a list of font vendors and their respective contact info. This
list is updated regularly and is indexed by a 4-char &quot;Vendor ID&quot; which is stored
in the achVendID field of the OS/2 table.
Registering your ID is not mandatory, but it is a good practice since some
applications may display the type designer / type foundry contact info on some
dialog and also because that info will be visible on Microsoft&#x27;s website:
https://docs.microsoft.com/en-us/typography/vendors/
This check verifies whether or not a given font&#x27;s vendor ID is registered in
that list or if it has some of the default values used by the most common font
editors.
Each new FontBakery release includes a cached copy of that list of vendor IDs.
If you registered recently, you&#x27;re safe to ignore warnings emitted by this
check, since your ID will soon be included in one of our upcoming releases.</pre>

* ⚠ **WARN** OS/2 VendorID value 'NONE' is not yet recognized. If you registered it recently, then it's safe to ignore this warning message. Otherwise, you should set it to your own unique 4 character code, and register it with Microsoft at https://www.microsoft.com/typography/links/vendorlist.aspx
 [code: unknown]

</details>
<details>
<summary>⚠ <b>WARN:</b> Font has old ttfautohint applied?</summary>

* [com.google.fonts/check/old_ttfautohint](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/old_ttfautohint)
<pre>--- Rationale ---
Check if font has been hinted with an outdated version of ttfautohint.</pre>

* ⚠ **WARN** ttfautohint used in font = 1.8.3; latest = 1.8.4; Need to re-run with the newer version! [code: old-ttfa]

</details>
<details>
<summary>⚠ <b>WARN:</b> Glyphs are similiar to Google Fonts version?</summary>

* [com.google.fonts/check/production_glyphs_similarity](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/production_glyphs_similarity)

* ⚠ **WARN** Following glyphs differ greatly from Google Fonts version: [Euro, Euro.BRACKET.125, Hbar, Ustraitstrokecy, hbar, uni044E, uni0462, uni0463, uni0473, uni0492, uni0496, uni0497, uni0498, uni049A, uni049B, uni04A2, uni04A3, uni04AA, uni04B6, uni04B7, uni04B8, uni04CB, uni04CC, uni04E8, uni04E9, uni04F6, uni04F7, uni0524, uni0525, uni05B8, uni05D2, uni05E0, uni05E2, uni05EA, uni20AE, uni20B4, uni20B4.BRACKET.125, uni20B9, uniFB2F, uniFB32, uniFB40, uniFB4A, yen, yen.BRACKET.125, zero.tf.zero, zero.zero]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check if each glyph has the recommended amount of contours.</summary>

* [com.google.fonts/check/contour_count](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/contour_count)
<pre>--- Rationale ---
Visually QAing thousands of glyphs by hand is tiring. Most glyphs can only be
constructured in a handful of ways. This means a glyph&#x27;s contour count will only
differ slightly amongst different fonts, e.g a &#x27;g&#x27; could either be 2 or 3
contours, depending on whether its double story or single story.
However, a quotedbl should have 2 contours, unless the font belongs to a display
family.
This check currently does not cover variable fonts because there&#x27;s plenty of
alternative ways of constructing glyphs with multiple outlines for each feature
in a VarFont. The expected contour count data for this check is currently
optimized for the typical construction of glyphs in static fonts.</pre>

* ⚠ **WARN** This check inspects the glyph outlines and detects the total number of contours in each of them. The expected values are infered from the typical ammounts of contours observed in a large collection of reference font families. The divergences listed below may simply indicate a significantly different design on some of your glyphs. On the other hand, some of these may flag actual bugs in the font such as glyphs mapped to an incorrect codepoint. Please consider reviewing the design and codepoint assignment of these to make sure they are correct.

The following glyphs do not have the recommended number of contours:

Glyph name: uni0493	Contours detected: 2	Expected: 1
Glyph name: ustraitstrokecy	Contours detected: 2	Expected: 1
Glyph name: fi	Contours detected: 1	Expected: 3
Glyph name: fl	Contours detected: 1	Expected: 2
Glyph name: uni0493	Contours detected: 2	Expected: 1 [code: contour-count]

</details>
<details>
<summary>⚠ <b>WARN:</b> Is there kerning info for non-ligated sequences?</summary>

* [com.google.fonts/check/kerning_for_non_ligated_sequences](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/kerning_for_non_ligated_sequences)
<pre>--- Rationale ---
Fonts with ligatures should have kerning on the corresponding non-ligated
sequences for text where ligatures aren&#x27;t used (eg
https://github.com/impallari/Raleway/issues/14).</pre>

* ⚠ **WARN** GPOS table lacks kerning info for the following non-ligated sequences:
	- f + f
	- f + i
	- i + f
	- f + l
	- l + f
	- i + l

   [code: lacks-kern-info]

</details>
<details>
<summary>⚠ <b>WARN:</b> Ensure fonts have ScriptLangTags declared on the 'meta' table.</summary>

* [com.google.fonts/check/meta/script_lang_tags](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/meta/script_lang_tags)
<pre>--- Rationale ---
The OpenType &#x27;meta&#x27; table originated at Apple. Microsoft added it to OT with
just two DataMap records:
- dlng: comma-separated ScriptLangTags that indicate which scripts, or languages
and scripts, with possible variants, the font is designed for
- slng: comma-separated ScriptLangTags that indicate which scripts, or languages
and scripts, with possible variants, the font supports
The slng structure is intended to describe which languages and scripts the font
overall supports. For example, a Traditional Chinese font that also contains
Latin characters, can indicate Hant,Latn, showing that it supports Hant, the
Traditional Chinese variant of the Hani script, and it also supports the Latn
script
The dlng structure is far more interesting. A font may contain various glyphs,
but only a particular subset of the glyphs may be truly &quot;leading&quot; in the design,
while other glyphs may have been included for technical reasons. Such a
Traditional Chinese font could only list Hant there, showing that it’s designed
for Traditional Chinese, but the font would omit Latn, because the developers
don’t think the font is really recommended for purely Latin-script use.
The tags used in the structures can comprise just script, or also language and
script. For example, if a font has Bulgarian Cyrillic alternates in the locl
feature for the cyrl BGR OT languagesystem, it could also indicate in dlng
explicitly that it supports bul-Cyrl. (Note that the scripts and languages in
meta use the ISO language and script codes, not the OpenType ones).
This check ensures that the font has the meta table containing the slng and dlng
structures.
All families in the Google Fonts collection should contain the &#x27;meta&#x27; table.
Windows 10 already uses it when deciding on which fonts to fall back to. The
Google Fonts API and also other environments could use the data for smarter
filtering. Most importantly, those entries should be added to the Noto fonts.
In the font making process, some environments store this data in external files
already. But the meta table provides a convenient way to store this inside the
font file, so some tools may add the data, and unrelated tools may read this
data. This makes the solution much more portable and universal.</pre>

* ⚠ **WARN** This font file does not have a 'meta' table. [code: lacks-meta-table]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check font contains no unreachable glyphs</summary>

* [com.google.fonts/check/unreachable_glyphs](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/universal.html#com.google.fonts/check/unreachable_glyphs)
<pre>--- Rationale ---
Glyphs are either accessible directly through Unicode codepoints or through
substitution rules. Any glyphs not accessible by either of these means are
redundant and serve only to increase the font&#x27;s file size.</pre>

* ⚠ **WARN** The following glyphs could not be reached by codepoint or substitution rules:
 - Euro.BRACKET.125
 - parenright.denominator
 - .null
 - yen.BRACKET.125
 - parenleft.numerator
 - uni030C.alt
 - brevecombcy
 - parenleft.denominator
 - uni20B4.BRACKET.125 
 - parenright.numerator
 [code: unreachable-glyphs]

</details>
<details>
<summary>⚠ <b>WARN:</b> Are there any misaligned on-curve points?</summary>

* [com.google.fonts/check/outline_alignment_miss](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_alignment_miss)
<pre>--- Rationale ---
This check heuristically looks for on-curve points which are close to, but do
not sit on, significant boundary coordinates. For example, a point which has a
Y-coordinate of 1 or -1 might be a misplaced baseline point. As well as the
baseline, here we also check for points near the x-height (but only for lower
case Latin letters), cap-height, ascender and descender Y coordinates.
Not all such misaligned curve points are a mistake, and sometimes the design may
call for points in locations near the boundaries. As this check is liable to
generate significant numbers of false positives, it will pass if there are more
than 100 reported misalignments.</pre>

* ⚠ **WARN** The following glyphs have on-curve points which have potentially incorrect y coordinates:
	* cent (U+00A2): X=225.0,Y=-2.0 (should be at baseline 0?)
	* atilde (U+00E3): X=303.5,Y=702.0 (should be at cap-height 700?)
	* atilde (U+00E3): X=353.0,Y=700.5 (should be at cap-height 700?)
	* ntilde (U+00F1): X=334.5,Y=702.0 (should be at cap-height 700?)
	* ntilde (U+00F1): X=384.0,Y=700.5 (should be at cap-height 700?)
	* otilde (U+00F5): X=316.5,Y=702.0 (should be at cap-height 700?)
	* otilde (U+00F5): X=366.0,Y=700.5 (should be at cap-height 700?)
	* eogonek (U+0119): X=207.0,Y=1.0 (should be at baseline 0?)
	* itilde (U+0129): X=153.5,Y=702.0 (should be at cap-height 700?)
	* itilde (U+0129): X=203.0,Y=700.5 (should be at cap-height 700?) and 26 more. [code: found-misalignments]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do any segments have colinear vectors?</summary>

* [com.google.fonts/check/outline_colinear_vectors](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_colinear_vectors)
<pre>--- Rationale ---
This check looks for consecutive line segments which have the same angle. This
normally happens if an outline point has been added by accident.
This check is not run for variable fonts, as they may legitimately have colinear
vectors.</pre>

* ⚠ **WARN** The following glyphs have colinear vectors:
	* uni0524 (U+0524): L<<504.0,25.0>--<504.0,140.0>> -> L<<504.0,140.0>--<504.0,142.0>> [code: found-colinear-vectors]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do outlines contain any semi-vertical or semi-horizontal lines?</summary>

* [com.google.fonts/check/outline_semi_vertical](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_semi_vertical)
<pre>--- Rationale ---
This check detects line segments which are nearly, but not quite, exactly
horizontal or vertical. Sometimes such lines are created by design, but often
they are indicative of a design error.
This check is disabled for italic styles, which often contain nearly-upright
lines.</pre>

* ⚠ **WARN** The following glyphs have semi-vertical/semi-horizontal lines:
 * g (U+0067): L<<561.0,495.0>--<562.0,14.0>>
 * gbreve (U+011F): L<<561.0,495.0>--<562.0,14.0>>
 * gcircumflex (U+011D): L<<561.0,495.0>--<562.0,14.0>>
 * gdotaccent (U+0121): L<<561.0,495.0>--<562.0,14.0>>
 * uni0123 (U+0123): L<<561.0,495.0>--<562.0,14.0>>
 * uni0434 (U+0434): L<<228.0,118.0>--<401.0,119.0>>
 * uni05E9 (U+05E9): L<<194.0,547.0>--<196.0,293.0>>
 * uni05EA (U+05EA): L<<260.0,0.0>--<70.0,1.0>>
 * uniFB2A (U+FB2A): L<<194.0,547.0>--<196.0,293.0>>
 * uniFB2B (U+FB2B): L<<194.0,547.0>--<196.0,293.0>> and 5 more. [code: found-semi-vertical]

</details>
<br>
</details>
<details>
<summary><b>[11] Rubik-Regular.ttf</b></summary>
<details>
<summary>💔 <b>ERROR:</b> Check samples can be rendered.</summary>

* [com.google.fonts/check/metadata/can_render_samples](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/metadata/can_render_samples)
<pre>--- Rationale ---
In order to prevent tofu from being seen on fonts.google.com, this check
verifies that all samples provided on METADATA.pb can be properly rendered by
the font.</pre>

* 💔 **ERROR** Failed with AttributeError: 'NoneType' object has no attribute 'sample_glyphs'

</details>
<details>
<summary>🔥 <b>FAIL:</b> Check license file has good copyright string.</summary>

* [com.google.fonts/check/license/OFL_copyright](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/license/OFL_copyright)
<pre>--- Rationale ---
An OFL.txt file&#x27;s first line should be the font copyright e.g:
&quot;Copyright 2019 The Montserrat Project Authors
(https://github.com/julietaula/montserrat)&quot;</pre>

* 🔥 **FAIL** First line in license file does not match expected format: "copyright 20** the my font project authors (https://github.com/googlefonts/my-font-repository)"

</details>
<details>
<summary>⚠ <b>WARN:</b> Checking OS/2 achVendID.</summary>

* [com.google.fonts/check/vendor_id](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/vendor_id)
<pre>--- Rationale ---
Microsoft keeps a list of font vendors and their respective contact info. This
list is updated regularly and is indexed by a 4-char &quot;Vendor ID&quot; which is stored
in the achVendID field of the OS/2 table.
Registering your ID is not mandatory, but it is a good practice since some
applications may display the type designer / type foundry contact info on some
dialog and also because that info will be visible on Microsoft&#x27;s website:
https://docs.microsoft.com/en-us/typography/vendors/
This check verifies whether or not a given font&#x27;s vendor ID is registered in
that list or if it has some of the default values used by the most common font
editors.
Each new FontBakery release includes a cached copy of that list of vendor IDs.
If you registered recently, you&#x27;re safe to ignore warnings emitted by this
check, since your ID will soon be included in one of our upcoming releases.</pre>

* ⚠ **WARN** OS/2 VendorID value 'NONE' is not yet recognized. If you registered it recently, then it's safe to ignore this warning message. Otherwise, you should set it to your own unique 4 character code, and register it with Microsoft at https://www.microsoft.com/typography/links/vendorlist.aspx
 [code: unknown]

</details>
<details>
<summary>⚠ <b>WARN:</b> Font has old ttfautohint applied?</summary>

* [com.google.fonts/check/old_ttfautohint](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/old_ttfautohint)
<pre>--- Rationale ---
Check if font has been hinted with an outdated version of ttfautohint.</pre>

* ⚠ **WARN** ttfautohint used in font = 1.8.3; latest = 1.8.4; Need to re-run with the newer version! [code: old-ttfa]

</details>
<details>
<summary>⚠ <b>WARN:</b> Glyphs are similiar to Google Fonts version?</summary>

* [com.google.fonts/check/production_glyphs_similarity](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/production_glyphs_similarity)

* ⚠ **WARN** Following glyphs differ greatly from Google Fonts version: [Euro, Euro.BRACKET.125, Hbar, Ustraitstrokecy, uni0462, uni0473, uni0496, uni049A, uni04A2, uni04E8, uni04E9, uni04F6, uni0524, uni05B8, uni20AE, uni20B4, uni20B4.BRACKET.125, uni20B9, yen, yen.BRACKET.125]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check if each glyph has the recommended amount of contours.</summary>

* [com.google.fonts/check/contour_count](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/contour_count)
<pre>--- Rationale ---
Visually QAing thousands of glyphs by hand is tiring. Most glyphs can only be
constructured in a handful of ways. This means a glyph&#x27;s contour count will only
differ slightly amongst different fonts, e.g a &#x27;g&#x27; could either be 2 or 3
contours, depending on whether its double story or single story.
However, a quotedbl should have 2 contours, unless the font belongs to a display
family.
This check currently does not cover variable fonts because there&#x27;s plenty of
alternative ways of constructing glyphs with multiple outlines for each feature
in a VarFont. The expected contour count data for this check is currently
optimized for the typical construction of glyphs in static fonts.</pre>

* ⚠ **WARN** This check inspects the glyph outlines and detects the total number of contours in each of them. The expected values are infered from the typical ammounts of contours observed in a large collection of reference font families. The divergences listed below may simply indicate a significantly different design on some of your glyphs. On the other hand, some of these may flag actual bugs in the font such as glyphs mapped to an incorrect codepoint. Please consider reviewing the design and codepoint assignment of these to make sure they are correct.

The following glyphs do not have the recommended number of contours:

Glyph name: uni0493	Contours detected: 2	Expected: 1
Glyph name: ustraitstrokecy	Contours detected: 2	Expected: 1
Glyph name: fi	Contours detected: 1	Expected: 3
Glyph name: fl	Contours detected: 1	Expected: 2
Glyph name: uni0493	Contours detected: 2	Expected: 1 [code: contour-count]

</details>
<details>
<summary>⚠ <b>WARN:</b> Is there kerning info for non-ligated sequences?</summary>

* [com.google.fonts/check/kerning_for_non_ligated_sequences](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/kerning_for_non_ligated_sequences)
<pre>--- Rationale ---
Fonts with ligatures should have kerning on the corresponding non-ligated
sequences for text where ligatures aren&#x27;t used (eg
https://github.com/impallari/Raleway/issues/14).</pre>

* ⚠ **WARN** GPOS table lacks kerning info for the following non-ligated sequences:
	- f + f
	- f + i
	- i + f
	- f + l
	- l + f
	- i + l

   [code: lacks-kern-info]

</details>
<details>
<summary>⚠ <b>WARN:</b> Ensure fonts have ScriptLangTags declared on the 'meta' table.</summary>

* [com.google.fonts/check/meta/script_lang_tags](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/meta/script_lang_tags)
<pre>--- Rationale ---
The OpenType &#x27;meta&#x27; table originated at Apple. Microsoft added it to OT with
just two DataMap records:
- dlng: comma-separated ScriptLangTags that indicate which scripts, or languages
and scripts, with possible variants, the font is designed for
- slng: comma-separated ScriptLangTags that indicate which scripts, or languages
and scripts, with possible variants, the font supports
The slng structure is intended to describe which languages and scripts the font
overall supports. For example, a Traditional Chinese font that also contains
Latin characters, can indicate Hant,Latn, showing that it supports Hant, the
Traditional Chinese variant of the Hani script, and it also supports the Latn
script
The dlng structure is far more interesting. A font may contain various glyphs,
but only a particular subset of the glyphs may be truly &quot;leading&quot; in the design,
while other glyphs may have been included for technical reasons. Such a
Traditional Chinese font could only list Hant there, showing that it’s designed
for Traditional Chinese, but the font would omit Latn, because the developers
don’t think the font is really recommended for purely Latin-script use.
The tags used in the structures can comprise just script, or also language and
script. For example, if a font has Bulgarian Cyrillic alternates in the locl
feature for the cyrl BGR OT languagesystem, it could also indicate in dlng
explicitly that it supports bul-Cyrl. (Note that the scripts and languages in
meta use the ISO language and script codes, not the OpenType ones).
This check ensures that the font has the meta table containing the slng and dlng
structures.
All families in the Google Fonts collection should contain the &#x27;meta&#x27; table.
Windows 10 already uses it when deciding on which fonts to fall back to. The
Google Fonts API and also other environments could use the data for smarter
filtering. Most importantly, those entries should be added to the Noto fonts.
In the font making process, some environments store this data in external files
already. But the meta table provides a convenient way to store this inside the
font file, so some tools may add the data, and unrelated tools may read this
data. This makes the solution much more portable and universal.</pre>

* ⚠ **WARN** This font file does not have a 'meta' table. [code: lacks-meta-table]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check font contains no unreachable glyphs</summary>

* [com.google.fonts/check/unreachable_glyphs](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/universal.html#com.google.fonts/check/unreachable_glyphs)
<pre>--- Rationale ---
Glyphs are either accessible directly through Unicode codepoints or through
substitution rules. Any glyphs not accessible by either of these means are
redundant and serve only to increase the font&#x27;s file size.</pre>

* ⚠ **WARN** The following glyphs could not be reached by codepoint or substitution rules:
 - Euro.BRACKET.125
 - parenright.denominator
 - .null
 - yen.BRACKET.125
 - parenleft.numerator
 - uni030C.alt
 - brevecombcy
 - parenleft.denominator
 - uni20B4.BRACKET.125 
 - parenright.numerator
 [code: unreachable-glyphs]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do any segments have colinear vectors?</summary>

* [com.google.fonts/check/outline_colinear_vectors](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_colinear_vectors)
<pre>--- Rationale ---
This check looks for consecutive line segments which have the same angle. This
normally happens if an outline point has been added by accident.
This check is not run for variable fonts, as they may legitimately have colinear
vectors.</pre>

* ⚠ **WARN** The following glyphs have colinear vectors:
	* uni0524 (U+0524): L<<529.0,90.0>--<529.0,90.0>> -> L<<529.0,90.0>--<529.0,90.0>>
	* uni05DC (U+05DC): L<<180.0,489.0>--<178.0,489.0>> -> L<<178.0,489.0>--<83.0,490.0>>
	* uni05DC (U+05DC): L<<210.0,489.0>--<180.0,489.0>> -> L<<180.0,489.0>--<178.0,489.0>>
	* uniFB3C (U+FB3C): L<<180.0,489.0>--<178.0,489.0>> -> L<<178.0,489.0>--<83.0,490.0>> and uniFB3C (U+FB3C): L<<210.0,489.0>--<180.0,489.0>> -> L<<180.0,489.0>--<178.0,489.0>> [code: found-colinear-vectors]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do outlines contain any semi-vertical or semi-horizontal lines?</summary>

* [com.google.fonts/check/outline_semi_vertical](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_semi_vertical)
<pre>--- Rationale ---
This check detects line segments which are nearly, but not quite, exactly
horizontal or vertical. Sometimes such lines are created by design, but often
they are indicative of a design error.
This check is disabled for italic styles, which often contain nearly-upright
lines.</pre>

* ⚠ **WARN** The following glyphs have semi-vertical/semi-horizontal lines:
 * uni0434 (U+0434): L<<168.0,80.0>--<406.0,82.0>> and uni0446 (U+0446): L<<517.0,497.0>--<516.0,80.0>> [code: found-semi-vertical]

</details>
<br>
</details>
<details>
<summary><b>[12] Rubik-BoldItalic.ttf</b></summary>
<details>
<summary>💔 <b>ERROR:</b> Check samples can be rendered.</summary>

* [com.google.fonts/check/metadata/can_render_samples](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/metadata/can_render_samples)
<pre>--- Rationale ---
In order to prevent tofu from being seen on fonts.google.com, this check
verifies that all samples provided on METADATA.pb can be properly rendered by
the font.</pre>

* 💔 **ERROR** Failed with AttributeError: 'NoneType' object has no attribute 'sample_glyphs'

</details>
<details>
<summary>🔥 <b>FAIL:</b> Check license file has good copyright string.</summary>

* [com.google.fonts/check/license/OFL_copyright](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/license/OFL_copyright)
<pre>--- Rationale ---
An OFL.txt file&#x27;s first line should be the font copyright e.g:
&quot;Copyright 2019 The Montserrat Project Authors
(https://github.com/julietaula/montserrat)&quot;</pre>

* 🔥 **FAIL** First line in license file does not match expected format: "copyright 20** the my font project authors (https://github.com/googlefonts/my-font-repository)"

</details>
<details>
<summary>⚠ <b>WARN:</b> Checking OS/2 achVendID.</summary>

* [com.google.fonts/check/vendor_id](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/vendor_id)
<pre>--- Rationale ---
Microsoft keeps a list of font vendors and their respective contact info. This
list is updated regularly and is indexed by a 4-char &quot;Vendor ID&quot; which is stored
in the achVendID field of the OS/2 table.
Registering your ID is not mandatory, but it is a good practice since some
applications may display the type designer / type foundry contact info on some
dialog and also because that info will be visible on Microsoft&#x27;s website:
https://docs.microsoft.com/en-us/typography/vendors/
This check verifies whether or not a given font&#x27;s vendor ID is registered in
that list or if it has some of the default values used by the most common font
editors.
Each new FontBakery release includes a cached copy of that list of vendor IDs.
If you registered recently, you&#x27;re safe to ignore warnings emitted by this
check, since your ID will soon be included in one of our upcoming releases.</pre>

* ⚠ **WARN** OS/2 VendorID value 'NONE' is not yet recognized. If you registered it recently, then it's safe to ignore this warning message. Otherwise, you should set it to your own unique 4 character code, and register it with Microsoft at https://www.microsoft.com/typography/links/vendorlist.aspx
 [code: unknown]

</details>
<details>
<summary>⚠ <b>WARN:</b> Font has old ttfautohint applied?</summary>

* [com.google.fonts/check/old_ttfautohint](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/old_ttfautohint)
<pre>--- Rationale ---
Check if font has been hinted with an outdated version of ttfautohint.</pre>

* ⚠ **WARN** ttfautohint used in font = 1.8.3; latest = 1.8.4; Need to re-run with the newer version! [code: old-ttfa]

</details>
<details>
<summary>⚠ <b>WARN:</b> Glyphs are similiar to Google Fonts version?</summary>

* [com.google.fonts/check/production_glyphs_similarity](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/production_glyphs_similarity)

* ⚠ **WARN** Following glyphs differ greatly from Google Fonts version: [Euro, Euro.BRACKET.125, Hbar, Ustraitstrokecy, hbar, uni00B5, uni044E, uni0462, uni0463, uni046B, uni0473, uni0492, uni0493, uni0496, uni0497, uni0498, uni0499, uni049A, uni049B, uni049C, uni04A0, uni04A1, uni04A2, uni04A3, uni04AA, uni04AB, uni04B6, uni04B7, uni04B8, uni04CB, uni04CC, uni04E8, uni04E9, uni04F6, uni04F7, uni0524, uni0525, uni05B8, uni05D2, uni05DC, uni05DE, uni05E0, uni05E2, uni05EA, uni20AE, uni20B4, uni20B4.BRACKET.125, uni20B9, uniFB2F, uniFB32, uniFB3C, uniFB3E, uniFB40, uniFB4A, yen, yen.BRACKET.125, zero.tf.zero, zero.zero]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check if each glyph has the recommended amount of contours.</summary>

* [com.google.fonts/check/contour_count](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/contour_count)
<pre>--- Rationale ---
Visually QAing thousands of glyphs by hand is tiring. Most glyphs can only be
constructured in a handful of ways. This means a glyph&#x27;s contour count will only
differ slightly amongst different fonts, e.g a &#x27;g&#x27; could either be 2 or 3
contours, depending on whether its double story or single story.
However, a quotedbl should have 2 contours, unless the font belongs to a display
family.
This check currently does not cover variable fonts because there&#x27;s plenty of
alternative ways of constructing glyphs with multiple outlines for each feature
in a VarFont. The expected contour count data for this check is currently
optimized for the typical construction of glyphs in static fonts.</pre>

* ⚠ **WARN** This check inspects the glyph outlines and detects the total number of contours in each of them. The expected values are infered from the typical ammounts of contours observed in a large collection of reference font families. The divergences listed below may simply indicate a significantly different design on some of your glyphs. On the other hand, some of these may flag actual bugs in the font such as glyphs mapped to an incorrect codepoint. Please consider reviewing the design and codepoint assignment of these to make sure they are correct.

The following glyphs do not have the recommended number of contours:

Glyph name: ustraitstrokecy	Contours detected: 2	Expected: 1
Glyph name: fi	Contours detected: 1	Expected: 3
Glyph name: fl	Contours detected: 1	Expected: 2 [code: contour-count]

</details>
<details>
<summary>⚠ <b>WARN:</b> Is there kerning info for non-ligated sequences?</summary>

* [com.google.fonts/check/kerning_for_non_ligated_sequences](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/kerning_for_non_ligated_sequences)
<pre>--- Rationale ---
Fonts with ligatures should have kerning on the corresponding non-ligated
sequences for text where ligatures aren&#x27;t used (eg
https://github.com/impallari/Raleway/issues/14).</pre>

* ⚠ **WARN** GPOS table lacks kerning info for the following non-ligated sequences:
	- f + f
	- f + i
	- i + f
	- f + l
	- l + f
	- i + l

   [code: lacks-kern-info]

</details>
<details>
<summary>⚠ <b>WARN:</b> Ensure fonts have ScriptLangTags declared on the 'meta' table.</summary>

* [com.google.fonts/check/meta/script_lang_tags](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/meta/script_lang_tags)
<pre>--- Rationale ---
The OpenType &#x27;meta&#x27; table originated at Apple. Microsoft added it to OT with
just two DataMap records:
- dlng: comma-separated ScriptLangTags that indicate which scripts, or languages
and scripts, with possible variants, the font is designed for
- slng: comma-separated ScriptLangTags that indicate which scripts, or languages
and scripts, with possible variants, the font supports
The slng structure is intended to describe which languages and scripts the font
overall supports. For example, a Traditional Chinese font that also contains
Latin characters, can indicate Hant,Latn, showing that it supports Hant, the
Traditional Chinese variant of the Hani script, and it also supports the Latn
script
The dlng structure is far more interesting. A font may contain various glyphs,
but only a particular subset of the glyphs may be truly &quot;leading&quot; in the design,
while other glyphs may have been included for technical reasons. Such a
Traditional Chinese font could only list Hant there, showing that it’s designed
for Traditional Chinese, but the font would omit Latn, because the developers
don’t think the font is really recommended for purely Latin-script use.
The tags used in the structures can comprise just script, or also language and
script. For example, if a font has Bulgarian Cyrillic alternates in the locl
feature for the cyrl BGR OT languagesystem, it could also indicate in dlng
explicitly that it supports bul-Cyrl. (Note that the scripts and languages in
meta use the ISO language and script codes, not the OpenType ones).
This check ensures that the font has the meta table containing the slng and dlng
structures.
All families in the Google Fonts collection should contain the &#x27;meta&#x27; table.
Windows 10 already uses it when deciding on which fonts to fall back to. The
Google Fonts API and also other environments could use the data for smarter
filtering. Most importantly, those entries should be added to the Noto fonts.
In the font making process, some environments store this data in external files
already. But the meta table provides a convenient way to store this inside the
font file, so some tools may add the data, and unrelated tools may read this
data. This makes the solution much more portable and universal.</pre>

* ⚠ **WARN** This font file does not have a 'meta' table. [code: lacks-meta-table]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check font contains no unreachable glyphs</summary>

* [com.google.fonts/check/unreachable_glyphs](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/universal.html#com.google.fonts/check/unreachable_glyphs)
<pre>--- Rationale ---
Glyphs are either accessible directly through Unicode codepoints or through
substitution rules. Any glyphs not accessible by either of these means are
redundant and serve only to increase the font&#x27;s file size.</pre>

* ⚠ **WARN** The following glyphs could not be reached by codepoint or substitution rules:
 - Euro.BRACKET.125
 - parenright.denominator
 - .null
 - yen.BRACKET.125
 - parenleft.numerator
 - uni030C.alt
 - brevecombcy
 - parenleft.denominator
 - uni20B4.BRACKET.125 
 - parenright.numerator
 [code: unreachable-glyphs]

</details>
<details>
<summary>⚠ <b>WARN:</b> Are there any misaligned on-curve points?</summary>

* [com.google.fonts/check/outline_alignment_miss](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_alignment_miss)
<pre>--- Rationale ---
This check heuristically looks for on-curve points which are close to, but do
not sit on, significant boundary coordinates. For example, a point which has a
Y-coordinate of 1 or -1 might be a misplaced baseline point. As well as the
baseline, here we also check for points near the x-height (but only for lower
case Latin letters), cap-height, ascender and descender Y coordinates.
Not all such misaligned curve points are a mistake, and sometimes the design may
call for points in locations near the boundaries. As this check is liable to
generate significant numbers of false positives, it will pass if there are more
than 100 reported misalignments.</pre>

* ⚠ **WARN** The following glyphs have on-curve points which have potentially incorrect y coordinates:
	* quotedbl (U+0022): X=279.0,Y=702.0 (should be at cap-height 700?)
	* quotedbl (U+0022): X=488.5,Y=702.0 (should be at cap-height 700?)
	* dollar (U+0024): X=477.0,Y=701.0 (should be at cap-height 700?)
	* quotesingle (U+0027): X=279.0,Y=702.0 (should be at cap-height 700?)
	* at (U+0040): X=704.5,Y=0.5 (should be at baseline 0?)
	* macron (U+00AF): X=46.0,Y=698.0 (should be at cap-height 700?)
	* macron (U+00AF): X=370.0,Y=698.0 (should be at cap-height 700?)
	* aring (U+00E5): X=411.5,Y=699.0 (should be at cap-height 700?)
	* aring (U+00E5): X=368.0,Y=699.0 (should be at cap-height 700?)
	* amacron (U+0101): X=228.0,Y=698.0 (should be at cap-height 700?) and 57 more. [code: found-misalignments]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do any segments have colinear vectors?</summary>

* [com.google.fonts/check/outline_colinear_vectors](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_colinear_vectors)
<pre>--- Rationale ---
This check looks for consecutive line segments which have the same angle. This
normally happens if an outline point has been added by accident.
This check is not run for variable fonts, as they may legitimately have colinear
vectors.</pre>

* ⚠ **WARN** The following glyphs have colinear vectors:
	* uni05DC (U+05DC): L<<238.0,434.0>--<237.0,434.0>> -> L<<237.0,434.0>--<105.0,434.0>>
	* uni05DC (U+05DC): L<<261.0,434.0>--<238.0,434.0>> -> L<<238.0,434.0>--<237.0,434.0>>
	* uniFB3C (U+FB3C): L<<238.0,434.0>--<237.0,434.0>> -> L<<237.0,434.0>--<105.0,434.0>> and uniFB3C (U+FB3C): L<<261.0,434.0>--<238.0,434.0>> -> L<<238.0,434.0>--<237.0,434.0>> [code: found-colinear-vectors]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do outlines contain any jaggy segments?</summary>

* [com.google.fonts/check/outline_jaggy_segments](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_jaggy_segments)
<pre>--- Rationale ---
This check heuristically detects outline segments which form a particularly
small angle, indicative of an outline error. This may cause false positives in
cases such as extreme ink traps, so should be regarded as advisory and backed up
by manual inspection.</pre>

* ⚠ **WARN** The following glyphs have jaggy segments:
	* uni0494 (U+0494): B<<252.0,236.0>-<233.0,219.0>-<227.0,188.0>>/L<<227.0,188.0>--<227.0,190.0>> = 10.954062643398332 and uni0494 (U+0494): L<<227.0,188.0>--<227.0,190.0>>/L<<227.0,190.0>--<192.0,25.0>> = 11.976132444203333 [code: found-jaggy-segments]

</details>
<br>
</details>
<details>
<summary><b>[11] Rubik-ExtraBoldItalic.ttf</b></summary>
<details>
<summary>💔 <b>ERROR:</b> Check samples can be rendered.</summary>

* [com.google.fonts/check/metadata/can_render_samples](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/metadata/can_render_samples)
<pre>--- Rationale ---
In order to prevent tofu from being seen on fonts.google.com, this check
verifies that all samples provided on METADATA.pb can be properly rendered by
the font.</pre>

* 💔 **ERROR** Failed with AttributeError: 'NoneType' object has no attribute 'sample_glyphs'

</details>
<details>
<summary>🔥 <b>FAIL:</b> Check license file has good copyright string.</summary>

* [com.google.fonts/check/license/OFL_copyright](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/license/OFL_copyright)
<pre>--- Rationale ---
An OFL.txt file&#x27;s first line should be the font copyright e.g:
&quot;Copyright 2019 The Montserrat Project Authors
(https://github.com/julietaula/montserrat)&quot;</pre>

* 🔥 **FAIL** First line in license file does not match expected format: "copyright 20** the my font project authors (https://github.com/googlefonts/my-font-repository)"

</details>
<details>
<summary>⚠ <b>WARN:</b> Checking OS/2 achVendID.</summary>

* [com.google.fonts/check/vendor_id](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/vendor_id)
<pre>--- Rationale ---
Microsoft keeps a list of font vendors and their respective contact info. This
list is updated regularly and is indexed by a 4-char &quot;Vendor ID&quot; which is stored
in the achVendID field of the OS/2 table.
Registering your ID is not mandatory, but it is a good practice since some
applications may display the type designer / type foundry contact info on some
dialog and also because that info will be visible on Microsoft&#x27;s website:
https://docs.microsoft.com/en-us/typography/vendors/
This check verifies whether or not a given font&#x27;s vendor ID is registered in
that list or if it has some of the default values used by the most common font
editors.
Each new FontBakery release includes a cached copy of that list of vendor IDs.
If you registered recently, you&#x27;re safe to ignore warnings emitted by this
check, since your ID will soon be included in one of our upcoming releases.</pre>

* ⚠ **WARN** OS/2 VendorID value 'NONE' is not yet recognized. If you registered it recently, then it's safe to ignore this warning message. Otherwise, you should set it to your own unique 4 character code, and register it with Microsoft at https://www.microsoft.com/typography/links/vendorlist.aspx
 [code: unknown]

</details>
<details>
<summary>⚠ <b>WARN:</b> Font has old ttfautohint applied?</summary>

* [com.google.fonts/check/old_ttfautohint](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/old_ttfautohint)
<pre>--- Rationale ---
Check if font has been hinted with an outdated version of ttfautohint.</pre>

* ⚠ **WARN** ttfautohint used in font = 1.8.3; latest = 1.8.4; Need to re-run with the newer version! [code: old-ttfa]

</details>
<details>
<summary>⚠ <b>WARN:</b> Glyphs are similiar to Google Fonts version?</summary>

* [com.google.fonts/check/production_glyphs_similarity](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/production_glyphs_similarity)

* ⚠ **WARN** Following glyphs differ greatly from Google Fonts version: [Euro, Hbar, Ustraitstrokecy, hbar, uni00B5, uni043C, uni0443, uni044E, uni045E, uni0462, uni0463, uni046B, uni0473, uni0492, uni0493, uni0496, uni0497, uni0498, uni0499, uni049A, uni049B, uni049C, uni049D, uni04A0, uni04A1, uni04A2, uni04A3, uni04AA, uni04AB, uni04B6, uni04B7, uni04B8, uni04B9, uni04CB, uni04CC, uni04E8, uni04E9, uni04EF, uni04F1, uni04F3, uni04F6, uni04F7, uni0524, uni0525, uni05B8, uni05D2, uni05DC, uni05DE, uni05E0, uni05E2, uni05EA, uni20AE, uni20B4, uni20B4.BRACKET.125, uni20B9, uniFB2F, uniFB32, uniFB3C, uniFB3E, uniFB40, uniFB4A, yen, zero.tf.zero, zero.zero]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check if each glyph has the recommended amount of contours.</summary>

* [com.google.fonts/check/contour_count](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/contour_count)
<pre>--- Rationale ---
Visually QAing thousands of glyphs by hand is tiring. Most glyphs can only be
constructured in a handful of ways. This means a glyph&#x27;s contour count will only
differ slightly amongst different fonts, e.g a &#x27;g&#x27; could either be 2 or 3
contours, depending on whether its double story or single story.
However, a quotedbl should have 2 contours, unless the font belongs to a display
family.
This check currently does not cover variable fonts because there&#x27;s plenty of
alternative ways of constructing glyphs with multiple outlines for each feature
in a VarFont. The expected contour count data for this check is currently
optimized for the typical construction of glyphs in static fonts.</pre>

* ⚠ **WARN** This check inspects the glyph outlines and detects the total number of contours in each of them. The expected values are infered from the typical ammounts of contours observed in a large collection of reference font families. The divergences listed below may simply indicate a significantly different design on some of your glyphs. On the other hand, some of these may flag actual bugs in the font such as glyphs mapped to an incorrect codepoint. Please consider reviewing the design and codepoint assignment of these to make sure they are correct.

The following glyphs do not have the recommended number of contours:

Glyph name: ustraitstrokecy	Contours detected: 2	Expected: 1
Glyph name: fi	Contours detected: 1	Expected: 3
Glyph name: fl	Contours detected: 1	Expected: 2 [code: contour-count]

</details>
<details>
<summary>⚠ <b>WARN:</b> Is there kerning info for non-ligated sequences?</summary>

* [com.google.fonts/check/kerning_for_non_ligated_sequences](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/kerning_for_non_ligated_sequences)
<pre>--- Rationale ---
Fonts with ligatures should have kerning on the corresponding non-ligated
sequences for text where ligatures aren&#x27;t used (eg
https://github.com/impallari/Raleway/issues/14).</pre>

* ⚠ **WARN** GPOS table lacks kerning info for the following non-ligated sequences:
	- f + f
	- f + i
	- i + f
	- f + l
	- l + f
	- i + l

   [code: lacks-kern-info]

</details>
<details>
<summary>⚠ <b>WARN:</b> Ensure fonts have ScriptLangTags declared on the 'meta' table.</summary>

* [com.google.fonts/check/meta/script_lang_tags](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/meta/script_lang_tags)
<pre>--- Rationale ---
The OpenType &#x27;meta&#x27; table originated at Apple. Microsoft added it to OT with
just two DataMap records:
- dlng: comma-separated ScriptLangTags that indicate which scripts, or languages
and scripts, with possible variants, the font is designed for
- slng: comma-separated ScriptLangTags that indicate which scripts, or languages
and scripts, with possible variants, the font supports
The slng structure is intended to describe which languages and scripts the font
overall supports. For example, a Traditional Chinese font that also contains
Latin characters, can indicate Hant,Latn, showing that it supports Hant, the
Traditional Chinese variant of the Hani script, and it also supports the Latn
script
The dlng structure is far more interesting. A font may contain various glyphs,
but only a particular subset of the glyphs may be truly &quot;leading&quot; in the design,
while other glyphs may have been included for technical reasons. Such a
Traditional Chinese font could only list Hant there, showing that it’s designed
for Traditional Chinese, but the font would omit Latn, because the developers
don’t think the font is really recommended for purely Latin-script use.
The tags used in the structures can comprise just script, or also language and
script. For example, if a font has Bulgarian Cyrillic alternates in the locl
feature for the cyrl BGR OT languagesystem, it could also indicate in dlng
explicitly that it supports bul-Cyrl. (Note that the scripts and languages in
meta use the ISO language and script codes, not the OpenType ones).
This check ensures that the font has the meta table containing the slng and dlng
structures.
All families in the Google Fonts collection should contain the &#x27;meta&#x27; table.
Windows 10 already uses it when deciding on which fonts to fall back to. The
Google Fonts API and also other environments could use the data for smarter
filtering. Most importantly, those entries should be added to the Noto fonts.
In the font making process, some environments store this data in external files
already. But the meta table provides a convenient way to store this inside the
font file, so some tools may add the data, and unrelated tools may read this
data. This makes the solution much more portable and universal.</pre>

* ⚠ **WARN** This font file does not have a 'meta' table. [code: lacks-meta-table]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check font contains no unreachable glyphs</summary>

* [com.google.fonts/check/unreachable_glyphs](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/universal.html#com.google.fonts/check/unreachable_glyphs)
<pre>--- Rationale ---
Glyphs are either accessible directly through Unicode codepoints or through
substitution rules. Any glyphs not accessible by either of these means are
redundant and serve only to increase the font&#x27;s file size.</pre>

* ⚠ **WARN** The following glyphs could not be reached by codepoint or substitution rules:
 - Euro.BRACKET.125
 - parenright.denominator
 - .null
 - yen.BRACKET.125
 - parenleft.numerator
 - uni030C.alt
 - brevecombcy
 - parenleft.denominator
 - uni20B4.BRACKET.125 
 - parenright.numerator
 [code: unreachable-glyphs]

</details>
<details>
<summary>⚠ <b>WARN:</b> Are there any misaligned on-curve points?</summary>

* [com.google.fonts/check/outline_alignment_miss](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_alignment_miss)
<pre>--- Rationale ---
This check heuristically looks for on-curve points which are close to, but do
not sit on, significant boundary coordinates. For example, a point which has a
Y-coordinate of 1 or -1 might be a misplaced baseline point. As well as the
baseline, here we also check for points near the x-height (but only for lower
case Latin letters), cap-height, ascender and descender Y coordinates.
Not all such misaligned curve points are a mistake, and sometimes the design may
call for points in locations near the boundaries. As this check is liable to
generate significant numbers of false positives, it will pass if there are more
than 100 reported misalignments.</pre>

* ⚠ **WARN** The following glyphs have on-curve points which have potentially incorrect y coordinates:
	* quotedbl (U+0022): X=296.0,Y=701.0 (should be at cap-height 700?)
	* quotedbl (U+0022): X=528.0,Y=701.0 (should be at cap-height 700?)
	* dollar (U+0024): X=496.0,Y=699.0 (should be at cap-height 700?)
	* ampersand (U+0026): X=359.0,Y=1.5 (should be at baseline 0?)
	* quotesingle (U+0027): X=296.0,Y=701.0 (should be at cap-height 700?)
	* parenleft (U+0028): X=292.0,Y=-1.0 (should be at baseline 0?)
	* parenright (U+0029): X=-16.0,Y=-1.0 (should be at baseline 0?)
	* less (U+003C): X=403.0,Y=-1.0 (should be at baseline 0?)
	* less (U+003C): X=403.0,Y=-1.0 (should be at baseline 0?)
	* greater (U+003E): X=21.0,Y=-2.0 (should be at baseline 0?) and 53 more. [code: found-misalignments]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do outlines contain any jaggy segments?</summary>

* [com.google.fonts/check/outline_jaggy_segments](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_jaggy_segments)
<pre>--- Rationale ---
This check heuristically detects outline segments which form a particularly
small angle, indicative of an outline error. This may cause false positives in
cases such as extreme ink traps, so should be regarded as advisory and backed up
by manual inspection.</pre>

* ⚠ **WARN** The following glyphs have jaggy segments:
	* uni0494 (U+0494): B<<284.5,215.0>-<258.0,203.0>-<250.0,168.0>>/L<<250.0,168.0>--<251.0,171.0>> = 5.559947263309426 and uni0494 (U+0494): L<<250.0,168.0>--<251.0,171.0>>/L<<251.0,171.0>--<220.0,26.0>> = 6.367179864268598 [code: found-jaggy-segments]

</details>
<br>
</details>
<details>
<summary><b>[12] Rubik-BlackItalic.ttf</b></summary>
<details>
<summary>💔 <b>ERROR:</b> Check samples can be rendered.</summary>

* [com.google.fonts/check/metadata/can_render_samples](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/metadata/can_render_samples)
<pre>--- Rationale ---
In order to prevent tofu from being seen on fonts.google.com, this check
verifies that all samples provided on METADATA.pb can be properly rendered by
the font.</pre>

* 💔 **ERROR** Failed with AttributeError: 'NoneType' object has no attribute 'sample_glyphs'

</details>
<details>
<summary>🔥 <b>FAIL:</b> Check license file has good copyright string.</summary>

* [com.google.fonts/check/license/OFL_copyright](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/license/OFL_copyright)
<pre>--- Rationale ---
An OFL.txt file&#x27;s first line should be the font copyright e.g:
&quot;Copyright 2019 The Montserrat Project Authors
(https://github.com/julietaula/montserrat)&quot;</pre>

* 🔥 **FAIL** First line in license file does not match expected format: "copyright 20** the my font project authors (https://github.com/googlefonts/my-font-repository)"

</details>
<details>
<summary>⚠ <b>WARN:</b> Checking OS/2 achVendID.</summary>

* [com.google.fonts/check/vendor_id](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/vendor_id)
<pre>--- Rationale ---
Microsoft keeps a list of font vendors and their respective contact info. This
list is updated regularly and is indexed by a 4-char &quot;Vendor ID&quot; which is stored
in the achVendID field of the OS/2 table.
Registering your ID is not mandatory, but it is a good practice since some
applications may display the type designer / type foundry contact info on some
dialog and also because that info will be visible on Microsoft&#x27;s website:
https://docs.microsoft.com/en-us/typography/vendors/
This check verifies whether or not a given font&#x27;s vendor ID is registered in
that list or if it has some of the default values used by the most common font
editors.
Each new FontBakery release includes a cached copy of that list of vendor IDs.
If you registered recently, you&#x27;re safe to ignore warnings emitted by this
check, since your ID will soon be included in one of our upcoming releases.</pre>

* ⚠ **WARN** OS/2 VendorID value 'NONE' is not yet recognized. If you registered it recently, then it's safe to ignore this warning message. Otherwise, you should set it to your own unique 4 character code, and register it with Microsoft at https://www.microsoft.com/typography/links/vendorlist.aspx
 [code: unknown]

</details>
<details>
<summary>⚠ <b>WARN:</b> Font has old ttfautohint applied?</summary>

* [com.google.fonts/check/old_ttfautohint](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/old_ttfautohint)
<pre>--- Rationale ---
Check if font has been hinted with an outdated version of ttfautohint.</pre>

* ⚠ **WARN** ttfautohint used in font = 1.8.3; latest = 1.8.4; Need to re-run with the newer version! [code: old-ttfa]

</details>
<details>
<summary>⚠ <b>WARN:</b> Glyphs are similiar to Google Fonts version?</summary>

* [com.google.fonts/check/production_glyphs_similarity](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/production_glyphs_similarity)

* ⚠ **WARN** Following glyphs differ greatly from Google Fonts version: [Euro, Euro.BRACKET.125, Hbar, Ustraitstrokecy, hbar, uni00B5, uni040E, uni0423, uni043C, uni0443, uni044E, uni045E, uni0462, uni0463, uni046B, uni0473, uni0492, uni0493, uni0496, uni0497, uni0498, uni0499, uni049A, uni049B, uni049C, uni049D, uni04A0, uni04A1, uni04A2, uni04A3, uni04AA, uni04AB, uni04B6, uni04B7, uni04B8, uni04B9, uni04CB, uni04CC, uni04E8, uni04E9, uni04EE, uni04EF, uni04F0, uni04F1, uni04F2, uni04F3, uni04F6, uni04F7, uni0524, uni0525, uni05B8, uni05D2, uni05DC, uni05DE, uni05E0, uni05E2, uni05EA, uni20AE, uni20B4, uni20B9, uniFB2F, uniFB32, uniFB3C, uniFB3E, uniFB40, uniFB4A, yen, zero.tf.zero, zero.zero]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check if each glyph has the recommended amount of contours.</summary>

* [com.google.fonts/check/contour_count](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/contour_count)
<pre>--- Rationale ---
Visually QAing thousands of glyphs by hand is tiring. Most glyphs can only be
constructured in a handful of ways. This means a glyph&#x27;s contour count will only
differ slightly amongst different fonts, e.g a &#x27;g&#x27; could either be 2 or 3
contours, depending on whether its double story or single story.
However, a quotedbl should have 2 contours, unless the font belongs to a display
family.
This check currently does not cover variable fonts because there&#x27;s plenty of
alternative ways of constructing glyphs with multiple outlines for each feature
in a VarFont. The expected contour count data for this check is currently
optimized for the typical construction of glyphs in static fonts.</pre>

* ⚠ **WARN** This check inspects the glyph outlines and detects the total number of contours in each of them. The expected values are infered from the typical ammounts of contours observed in a large collection of reference font families. The divergences listed below may simply indicate a significantly different design on some of your glyphs. On the other hand, some of these may flag actual bugs in the font such as glyphs mapped to an incorrect codepoint. Please consider reviewing the design and codepoint assignment of these to make sure they are correct.

The following glyphs do not have the recommended number of contours:

Glyph name: ustraitstrokecy	Contours detected: 2	Expected: 1
Glyph name: fi	Contours detected: 1	Expected: 3
Glyph name: fl	Contours detected: 1	Expected: 2 [code: contour-count]

</details>
<details>
<summary>⚠ <b>WARN:</b> Is there kerning info for non-ligated sequences?</summary>

* [com.google.fonts/check/kerning_for_non_ligated_sequences](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/kerning_for_non_ligated_sequences)
<pre>--- Rationale ---
Fonts with ligatures should have kerning on the corresponding non-ligated
sequences for text where ligatures aren&#x27;t used (eg
https://github.com/impallari/Raleway/issues/14).</pre>

* ⚠ **WARN** GPOS table lacks kerning info for the following non-ligated sequences:
	- f + f
	- f + i
	- i + f
	- f + l
	- l + f
	- i + l

   [code: lacks-kern-info]

</details>
<details>
<summary>⚠ <b>WARN:</b> Ensure fonts have ScriptLangTags declared on the 'meta' table.</summary>

* [com.google.fonts/check/meta/script_lang_tags](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/meta/script_lang_tags)
<pre>--- Rationale ---
The OpenType &#x27;meta&#x27; table originated at Apple. Microsoft added it to OT with
just two DataMap records:
- dlng: comma-separated ScriptLangTags that indicate which scripts, or languages
and scripts, with possible variants, the font is designed for
- slng: comma-separated ScriptLangTags that indicate which scripts, or languages
and scripts, with possible variants, the font supports
The slng structure is intended to describe which languages and scripts the font
overall supports. For example, a Traditional Chinese font that also contains
Latin characters, can indicate Hant,Latn, showing that it supports Hant, the
Traditional Chinese variant of the Hani script, and it also supports the Latn
script
The dlng structure is far more interesting. A font may contain various glyphs,
but only a particular subset of the glyphs may be truly &quot;leading&quot; in the design,
while other glyphs may have been included for technical reasons. Such a
Traditional Chinese font could only list Hant there, showing that it’s designed
for Traditional Chinese, but the font would omit Latn, because the developers
don’t think the font is really recommended for purely Latin-script use.
The tags used in the structures can comprise just script, or also language and
script. For example, if a font has Bulgarian Cyrillic alternates in the locl
feature for the cyrl BGR OT languagesystem, it could also indicate in dlng
explicitly that it supports bul-Cyrl. (Note that the scripts and languages in
meta use the ISO language and script codes, not the OpenType ones).
This check ensures that the font has the meta table containing the slng and dlng
structures.
All families in the Google Fonts collection should contain the &#x27;meta&#x27; table.
Windows 10 already uses it when deciding on which fonts to fall back to. The
Google Fonts API and also other environments could use the data for smarter
filtering. Most importantly, those entries should be added to the Noto fonts.
In the font making process, some environments store this data in external files
already. But the meta table provides a convenient way to store this inside the
font file, so some tools may add the data, and unrelated tools may read this
data. This makes the solution much more portable and universal.</pre>

* ⚠ **WARN** This font file does not have a 'meta' table. [code: lacks-meta-table]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check font contains no unreachable glyphs</summary>

* [com.google.fonts/check/unreachable_glyphs](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/universal.html#com.google.fonts/check/unreachable_glyphs)
<pre>--- Rationale ---
Glyphs are either accessible directly through Unicode codepoints or through
substitution rules. Any glyphs not accessible by either of these means are
redundant and serve only to increase the font&#x27;s file size.</pre>

* ⚠ **WARN** The following glyphs could not be reached by codepoint or substitution rules:
 - Euro.BRACKET.125
 - parenright.denominator
 - .null
 - yen.BRACKET.125
 - parenleft.numerator
 - uni030C.alt
 - brevecombcy
 - parenleft.denominator
 - uni20B4.BRACKET.125 
 - parenright.numerator
 [code: unreachable-glyphs]

</details>
<details>
<summary>⚠ <b>WARN:</b> Are there any misaligned on-curve points?</summary>

* [com.google.fonts/check/outline_alignment_miss](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_alignment_miss)
<pre>--- Rationale ---
This check heuristically looks for on-curve points which are close to, but do
not sit on, significant boundary coordinates. For example, a point which has a
Y-coordinate of 1 or -1 might be a misplaced baseline point. As well as the
baseline, here we also check for points near the x-height (but only for lower
case Latin letters), cap-height, ascender and descender Y coordinates.
Not all such misaligned curve points are a mistake, and sometimes the design may
call for points in locations near the boundaries. As this check is liable to
generate significant numbers of false positives, it will pass if there are more
than 100 reported misalignments.</pre>

* ⚠ **WARN** The following glyphs have on-curve points which have potentially incorrect y coordinates:
	* quotedbl (U+0022): X=312.5,Y=700.5 (should be at cap-height 700?)
	* quotedbl (U+0022): X=567.5,Y=700.5 (should be at cap-height 700?)
	* dollar (U+0024): X=211.0,Y=-2.0 (should be at baseline 0?)
	* ampersand (U+0026): X=357.5,Y=-2.0 (should be at baseline 0?)
	* quotesingle (U+0027): X=312.5,Y=700.5 (should be at cap-height 700?)
	* b (U+0062): X=139.5,Y=702.0 (should be at cap-height 700?)
	* b (U+0062): X=362.5,Y=702.0 (should be at cap-height 700?)
	* d (U+0064): X=470.5,Y=702.0 (should be at cap-height 700?)
	* d (U+0064): X=693.5,Y=702.0 (should be at cap-height 700?)
	* h (U+0068): X=139.5,Y=702.0 (should be at cap-height 700?) and 90 more. [code: found-misalignments]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do any segments have colinear vectors?</summary>

* [com.google.fonts/check/outline_colinear_vectors](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_colinear_vectors)
<pre>--- Rationale ---
This check looks for consecutive line segments which have the same angle. This
normally happens if an outline point has been added by accident.
This check is not run for variable fonts, as they may legitimately have colinear
vectors.</pre>

* ⚠ **WARN** The following glyphs have colinear vectors:
	* uni04A2 (U+04A2): L<<450.0,220.0>--<450.0,220.0>> -> L<<450.0,220.0>--<450.0,220.0>> [code: found-colinear-vectors]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do outlines contain any jaggy segments?</summary>

* [com.google.fonts/check/outline_jaggy_segments](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_jaggy_segments)
<pre>--- Rationale ---
This check heuristically detects outline segments which form a particularly
small angle, indicative of an outline error. This may cause false positives in
cases such as extreme ink traps, so should be regarded as advisory and backed up
by manual inspection.</pre>

* ⚠ **WARN** The following glyphs have jaggy segments:
	* uni0494 (U+0494): B<<296.5,180.5>-<279.0,172.0>-<274.0,149.0>>/L<<274.0,149.0>--<275.0,153.0>> = 1.7714697400342114
	* uni0494 (U+0494): L<<274.0,149.0>--<275.0,153.0>>/L<<275.0,153.0>--<248.0,27.0>> = 1.9414863909143467
	* uni0496 (U+0496): L<<847.0,0.0>--<847.0,0.0>>/B<<847.0,0.0>-<829.0,1.0>-<822.0,10.0>> = 3.1798301198641643 and uni049B (U+049B): L<<356.0,0.0>--<356.0,0.0>>/B<<356.0,0.0>-<347.0,2.0>-<342.0,6.5>> = 12.528807709151492 [code: found-jaggy-segments]

</details>
<br>
</details>
<details>
<summary><b>[12] Rubik-MediumItalic.ttf</b></summary>
<details>
<summary>💔 <b>ERROR:</b> Check samples can be rendered.</summary>

* [com.google.fonts/check/metadata/can_render_samples](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/metadata/can_render_samples)
<pre>--- Rationale ---
In order to prevent tofu from being seen on fonts.google.com, this check
verifies that all samples provided on METADATA.pb can be properly rendered by
the font.</pre>

* 💔 **ERROR** Failed with AttributeError: 'NoneType' object has no attribute 'sample_glyphs'

</details>
<details>
<summary>🔥 <b>FAIL:</b> Check license file has good copyright string.</summary>

* [com.google.fonts/check/license/OFL_copyright](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/license/OFL_copyright)
<pre>--- Rationale ---
An OFL.txt file&#x27;s first line should be the font copyright e.g:
&quot;Copyright 2019 The Montserrat Project Authors
(https://github.com/julietaula/montserrat)&quot;</pre>

* 🔥 **FAIL** First line in license file does not match expected format: "copyright 20** the my font project authors (https://github.com/googlefonts/my-font-repository)"

</details>
<details>
<summary>⚠ <b>WARN:</b> Checking OS/2 achVendID.</summary>

* [com.google.fonts/check/vendor_id](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/vendor_id)
<pre>--- Rationale ---
Microsoft keeps a list of font vendors and their respective contact info. This
list is updated regularly and is indexed by a 4-char &quot;Vendor ID&quot; which is stored
in the achVendID field of the OS/2 table.
Registering your ID is not mandatory, but it is a good practice since some
applications may display the type designer / type foundry contact info on some
dialog and also because that info will be visible on Microsoft&#x27;s website:
https://docs.microsoft.com/en-us/typography/vendors/
This check verifies whether or not a given font&#x27;s vendor ID is registered in
that list or if it has some of the default values used by the most common font
editors.
Each new FontBakery release includes a cached copy of that list of vendor IDs.
If you registered recently, you&#x27;re safe to ignore warnings emitted by this
check, since your ID will soon be included in one of our upcoming releases.</pre>

* ⚠ **WARN** OS/2 VendorID value 'NONE' is not yet recognized. If you registered it recently, then it's safe to ignore this warning message. Otherwise, you should set it to your own unique 4 character code, and register it with Microsoft at https://www.microsoft.com/typography/links/vendorlist.aspx
 [code: unknown]

</details>
<details>
<summary>⚠ <b>WARN:</b> Font has old ttfautohint applied?</summary>

* [com.google.fonts/check/old_ttfautohint](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/old_ttfautohint)
<pre>--- Rationale ---
Check if font has been hinted with an outdated version of ttfautohint.</pre>

* ⚠ **WARN** ttfautohint used in font = 1.8.3; latest = 1.8.4; Need to re-run with the newer version! [code: old-ttfa]

</details>
<details>
<summary>⚠ <b>WARN:</b> Glyphs are similiar to Google Fonts version?</summary>

* [com.google.fonts/check/production_glyphs_similarity](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/production_glyphs_similarity)

* ⚠ **WARN** Following glyphs differ greatly from Google Fonts version: [Euro, Euro.BRACKET.125, Hbar, Ustraitstrokecy, hbar, uni044E, uni0462, uni0463, uni0473, uni0492, uni0493, uni0496, uni0497, uni049A, uni049B, uni04A0, uni04A1, uni04A2, uni04A3, uni04B6, uni04B7, uni04CB, uni04CC, uni04E8, uni04E9, uni04F6, uni04F7, uni0524, uni0525, uni05B8, uni05D2, uni05E0, uni05E2, uni20AE, uni20B4, uni20B4.BRACKET.125, uni20B9, uniFB32, uniFB40, yen, yen.BRACKET.125, zero.tf.zero, zero.zero]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check if each glyph has the recommended amount of contours.</summary>

* [com.google.fonts/check/contour_count](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/contour_count)
<pre>--- Rationale ---
Visually QAing thousands of glyphs by hand is tiring. Most glyphs can only be
constructured in a handful of ways. This means a glyph&#x27;s contour count will only
differ slightly amongst different fonts, e.g a &#x27;g&#x27; could either be 2 or 3
contours, depending on whether its double story or single story.
However, a quotedbl should have 2 contours, unless the font belongs to a display
family.
This check currently does not cover variable fonts because there&#x27;s plenty of
alternative ways of constructing glyphs with multiple outlines for each feature
in a VarFont. The expected contour count data for this check is currently
optimized for the typical construction of glyphs in static fonts.</pre>

* ⚠ **WARN** This check inspects the glyph outlines and detects the total number of contours in each of them. The expected values are infered from the typical ammounts of contours observed in a large collection of reference font families. The divergences listed below may simply indicate a significantly different design on some of your glyphs. On the other hand, some of these may flag actual bugs in the font such as glyphs mapped to an incorrect codepoint. Please consider reviewing the design and codepoint assignment of these to make sure they are correct.

The following glyphs do not have the recommended number of contours:

Glyph name: ustraitstrokecy	Contours detected: 2	Expected: 1
Glyph name: fi	Contours detected: 1	Expected: 3
Glyph name: fl	Contours detected: 1	Expected: 2 [code: contour-count]

</details>
<details>
<summary>⚠ <b>WARN:</b> Is there kerning info for non-ligated sequences?</summary>

* [com.google.fonts/check/kerning_for_non_ligated_sequences](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/kerning_for_non_ligated_sequences)
<pre>--- Rationale ---
Fonts with ligatures should have kerning on the corresponding non-ligated
sequences for text where ligatures aren&#x27;t used (eg
https://github.com/impallari/Raleway/issues/14).</pre>

* ⚠ **WARN** GPOS table lacks kerning info for the following non-ligated sequences:
	- f + f
	- f + i
	- i + f
	- f + l
	- l + f
	- i + l

   [code: lacks-kern-info]

</details>
<details>
<summary>⚠ <b>WARN:</b> Ensure fonts have ScriptLangTags declared on the 'meta' table.</summary>

* [com.google.fonts/check/meta/script_lang_tags](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/meta/script_lang_tags)
<pre>--- Rationale ---
The OpenType &#x27;meta&#x27; table originated at Apple. Microsoft added it to OT with
just two DataMap records:
- dlng: comma-separated ScriptLangTags that indicate which scripts, or languages
and scripts, with possible variants, the font is designed for
- slng: comma-separated ScriptLangTags that indicate which scripts, or languages
and scripts, with possible variants, the font supports
The slng structure is intended to describe which languages and scripts the font
overall supports. For example, a Traditional Chinese font that also contains
Latin characters, can indicate Hant,Latn, showing that it supports Hant, the
Traditional Chinese variant of the Hani script, and it also supports the Latn
script
The dlng structure is far more interesting. A font may contain various glyphs,
but only a particular subset of the glyphs may be truly &quot;leading&quot; in the design,
while other glyphs may have been included for technical reasons. Such a
Traditional Chinese font could only list Hant there, showing that it’s designed
for Traditional Chinese, but the font would omit Latn, because the developers
don’t think the font is really recommended for purely Latin-script use.
The tags used in the structures can comprise just script, or also language and
script. For example, if a font has Bulgarian Cyrillic alternates in the locl
feature for the cyrl BGR OT languagesystem, it could also indicate in dlng
explicitly that it supports bul-Cyrl. (Note that the scripts and languages in
meta use the ISO language and script codes, not the OpenType ones).
This check ensures that the font has the meta table containing the slng and dlng
structures.
All families in the Google Fonts collection should contain the &#x27;meta&#x27; table.
Windows 10 already uses it when deciding on which fonts to fall back to. The
Google Fonts API and also other environments could use the data for smarter
filtering. Most importantly, those entries should be added to the Noto fonts.
In the font making process, some environments store this data in external files
already. But the meta table provides a convenient way to store this inside the
font file, so some tools may add the data, and unrelated tools may read this
data. This makes the solution much more portable and universal.</pre>

* ⚠ **WARN** This font file does not have a 'meta' table. [code: lacks-meta-table]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check font contains no unreachable glyphs</summary>

* [com.google.fonts/check/unreachable_glyphs](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/universal.html#com.google.fonts/check/unreachable_glyphs)
<pre>--- Rationale ---
Glyphs are either accessible directly through Unicode codepoints or through
substitution rules. Any glyphs not accessible by either of these means are
redundant and serve only to increase the font&#x27;s file size.</pre>

* ⚠ **WARN** The following glyphs could not be reached by codepoint or substitution rules:
 - Euro.BRACKET.125
 - parenright.denominator
 - .null
 - yen.BRACKET.125
 - parenleft.numerator
 - uni030C.alt
 - brevecombcy
 - parenleft.denominator
 - uni20B4.BRACKET.125 
 - parenright.numerator
 [code: unreachable-glyphs]

</details>
<details>
<summary>⚠ <b>WARN:</b> Are there any misaligned on-curve points?</summary>

* [com.google.fonts/check/outline_alignment_miss](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_alignment_miss)
<pre>--- Rationale ---
This check heuristically looks for on-curve points which are close to, but do
not sit on, significant boundary coordinates. For example, a point which has a
Y-coordinate of 1 or -1 might be a misplaced baseline point. As well as the
baseline, here we also check for points near the x-height (but only for lower
case Latin letters), cap-height, ascender and descender Y coordinates.
Not all such misaligned curve points are a mistake, and sometimes the design may
call for points in locations near the boundaries. As this check is liable to
generate significant numbers of false positives, it will pass if there are more
than 100 reported misalignments.</pre>

* ⚠ **WARN** The following glyphs have on-curve points which have potentially incorrect y coordinates:
	* i (U+0069): X=149.0,Y=702.0 (should be at cap-height 700?)
	* i (U+0069): X=289.0,Y=702.0 (should be at cap-height 700?)
	* j (U+006A): X=159.0,Y=702.0 (should be at cap-height 700?)
	* j (U+006A): X=302.0,Y=702.0 (should be at cap-height 700?)
	* j (U+006A): X=14.0,Y=1.0 (should be at baseline 0?)
	* j (U+006A): X=149.0,Y=-1.0 (should be at baseline 0?)
	* braceleft (U+007B): X=206.5,Y=-1.5 (should be at baseline 0?)
	* atilde (U+00E3): X=266.5,Y=701.0 (should be at cap-height 700?)
	* ntilde (U+00F1): X=282.5,Y=701.0 (should be at cap-height 700?)
	* otilde (U+00F5): X=265.5,Y=701.0 (should be at cap-height 700?) and 68 more. [code: found-misalignments]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do any segments have colinear vectors?</summary>

* [com.google.fonts/check/outline_colinear_vectors](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_colinear_vectors)
<pre>--- Rationale ---
This check looks for consecutive line segments which have the same angle. This
normally happens if an outline point has been added by accident.
This check is not run for variable fonts, as they may legitimately have colinear
vectors.</pre>

* ⚠ **WARN** The following glyphs have colinear vectors:
	* uni04CB (U+04CB): L<<563.0,84.0>--<563.0,84.0>> -> L<<563.0,84.0>--<563.0,84.0>> [code: found-colinear-vectors]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do outlines contain any jaggy segments?</summary>

* [com.google.fonts/check/outline_jaggy_segments](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_jaggy_segments)
<pre>--- Rationale ---
This check heuristically detects outline segments which form a particularly
small angle, indicative of an outline error. This may cause false positives in
cases such as extreme ink traps, so should be regarded as advisory and backed up
by manual inspection.</pre>

* ⚠ **WARN** The following glyphs have jaggy segments:
	* uni0494 (U+0494): B<<233.0,273.5>-<208.0,252.0>-<199.0,210.0>>/L<<199.0,210.0>--<199.0,211.0>> = 12.094757077012089
	* uni0494 (U+0494): L<<199.0,210.0>--<199.0,211.0>>/L<<199.0,211.0>--<160.0,24.0>> = 11.780523776915402 and uni04A1 (U+04A1): L<<138.0,24.0>--<222.0,415.0>>/L<<222.0,415.0>--<222.0,414.0>> = 12.12477582008083 [code: found-jaggy-segments]

</details>
<br>
</details>
<details>
<summary><b>[12] Rubik-SemiBoldItalic.ttf</b></summary>
<details>
<summary>💔 <b>ERROR:</b> Check samples can be rendered.</summary>

* [com.google.fonts/check/metadata/can_render_samples](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/metadata/can_render_samples)
<pre>--- Rationale ---
In order to prevent tofu from being seen on fonts.google.com, this check
verifies that all samples provided on METADATA.pb can be properly rendered by
the font.</pre>

* 💔 **ERROR** Failed with AttributeError: 'NoneType' object has no attribute 'sample_glyphs'

</details>
<details>
<summary>🔥 <b>FAIL:</b> Check license file has good copyright string.</summary>

* [com.google.fonts/check/license/OFL_copyright](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/license/OFL_copyright)
<pre>--- Rationale ---
An OFL.txt file&#x27;s first line should be the font copyright e.g:
&quot;Copyright 2019 The Montserrat Project Authors
(https://github.com/julietaula/montserrat)&quot;</pre>

* 🔥 **FAIL** First line in license file does not match expected format: "copyright 20** the my font project authors (https://github.com/googlefonts/my-font-repository)"

</details>
<details>
<summary>⚠ <b>WARN:</b> Checking OS/2 achVendID.</summary>

* [com.google.fonts/check/vendor_id](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/vendor_id)
<pre>--- Rationale ---
Microsoft keeps a list of font vendors and their respective contact info. This
list is updated regularly and is indexed by a 4-char &quot;Vendor ID&quot; which is stored
in the achVendID field of the OS/2 table.
Registering your ID is not mandatory, but it is a good practice since some
applications may display the type designer / type foundry contact info on some
dialog and also because that info will be visible on Microsoft&#x27;s website:
https://docs.microsoft.com/en-us/typography/vendors/
This check verifies whether or not a given font&#x27;s vendor ID is registered in
that list or if it has some of the default values used by the most common font
editors.
Each new FontBakery release includes a cached copy of that list of vendor IDs.
If you registered recently, you&#x27;re safe to ignore warnings emitted by this
check, since your ID will soon be included in one of our upcoming releases.</pre>

* ⚠ **WARN** OS/2 VendorID value 'NONE' is not yet recognized. If you registered it recently, then it's safe to ignore this warning message. Otherwise, you should set it to your own unique 4 character code, and register it with Microsoft at https://www.microsoft.com/typography/links/vendorlist.aspx
 [code: unknown]

</details>
<details>
<summary>⚠ <b>WARN:</b> Font has old ttfautohint applied?</summary>

* [com.google.fonts/check/old_ttfautohint](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/old_ttfautohint)
<pre>--- Rationale ---
Check if font has been hinted with an outdated version of ttfautohint.</pre>

* ⚠ **WARN** ttfautohint used in font = 1.8.3; latest = 1.8.4; Need to re-run with the newer version! [code: old-ttfa]

</details>
<details>
<summary>⚠ <b>WARN:</b> Glyphs are similiar to Google Fonts version?</summary>

* [com.google.fonts/check/production_glyphs_similarity](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/production_glyphs_similarity)

* ⚠ **WARN** Following glyphs differ greatly from Google Fonts version: [Euro, Euro.BRACKET.125, Hbar, Ustraitstrokecy, hbar, uni044E, uni0462, uni0463, uni0473, uni0492, uni0493, uni0496, uni0497, uni0498, uni049A, uni049B, uni04A0, uni04A1, uni04A2, uni04A3, uni04AA, uni04B6, uni04B7, uni04B8, uni04CB, uni04CC, uni04E8, uni04E9, uni04F6, uni04F7, uni0524, uni0525, uni05B8, uni05D2, uni05DE, uni05E0, uni05E2, uni05EA, uni20AE, uni20B4, uni20B4.BRACKET.125, uni20B9, uniFB2F, uniFB32, uniFB3E, uniFB40, uniFB4A, yen, yen.BRACKET.125, zero.tf.zero, zero.zero]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check if each glyph has the recommended amount of contours.</summary>

* [com.google.fonts/check/contour_count](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/contour_count)
<pre>--- Rationale ---
Visually QAing thousands of glyphs by hand is tiring. Most glyphs can only be
constructured in a handful of ways. This means a glyph&#x27;s contour count will only
differ slightly amongst different fonts, e.g a &#x27;g&#x27; could either be 2 or 3
contours, depending on whether its double story or single story.
However, a quotedbl should have 2 contours, unless the font belongs to a display
family.
This check currently does not cover variable fonts because there&#x27;s plenty of
alternative ways of constructing glyphs with multiple outlines for each feature
in a VarFont. The expected contour count data for this check is currently
optimized for the typical construction of glyphs in static fonts.</pre>

* ⚠ **WARN** This check inspects the glyph outlines and detects the total number of contours in each of them. The expected values are infered from the typical ammounts of contours observed in a large collection of reference font families. The divergences listed below may simply indicate a significantly different design on some of your glyphs. On the other hand, some of these may flag actual bugs in the font such as glyphs mapped to an incorrect codepoint. Please consider reviewing the design and codepoint assignment of these to make sure they are correct.

The following glyphs do not have the recommended number of contours:

Glyph name: ustraitstrokecy	Contours detected: 2	Expected: 1
Glyph name: fi	Contours detected: 1	Expected: 3
Glyph name: fl	Contours detected: 1	Expected: 2 [code: contour-count]

</details>
<details>
<summary>⚠ <b>WARN:</b> Is there kerning info for non-ligated sequences?</summary>

* [com.google.fonts/check/kerning_for_non_ligated_sequences](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/kerning_for_non_ligated_sequences)
<pre>--- Rationale ---
Fonts with ligatures should have kerning on the corresponding non-ligated
sequences for text where ligatures aren&#x27;t used (eg
https://github.com/impallari/Raleway/issues/14).</pre>

* ⚠ **WARN** GPOS table lacks kerning info for the following non-ligated sequences:
	- f + f
	- f + i
	- i + f
	- f + l
	- l + f
	- i + l

   [code: lacks-kern-info]

</details>
<details>
<summary>⚠ <b>WARN:</b> Ensure fonts have ScriptLangTags declared on the 'meta' table.</summary>

* [com.google.fonts/check/meta/script_lang_tags](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/meta/script_lang_tags)
<pre>--- Rationale ---
The OpenType &#x27;meta&#x27; table originated at Apple. Microsoft added it to OT with
just two DataMap records:
- dlng: comma-separated ScriptLangTags that indicate which scripts, or languages
and scripts, with possible variants, the font is designed for
- slng: comma-separated ScriptLangTags that indicate which scripts, or languages
and scripts, with possible variants, the font supports
The slng structure is intended to describe which languages and scripts the font
overall supports. For example, a Traditional Chinese font that also contains
Latin characters, can indicate Hant,Latn, showing that it supports Hant, the
Traditional Chinese variant of the Hani script, and it also supports the Latn
script
The dlng structure is far more interesting. A font may contain various glyphs,
but only a particular subset of the glyphs may be truly &quot;leading&quot; in the design,
while other glyphs may have been included for technical reasons. Such a
Traditional Chinese font could only list Hant there, showing that it’s designed
for Traditional Chinese, but the font would omit Latn, because the developers
don’t think the font is really recommended for purely Latin-script use.
The tags used in the structures can comprise just script, or also language and
script. For example, if a font has Bulgarian Cyrillic alternates in the locl
feature for the cyrl BGR OT languagesystem, it could also indicate in dlng
explicitly that it supports bul-Cyrl. (Note that the scripts and languages in
meta use the ISO language and script codes, not the OpenType ones).
This check ensures that the font has the meta table containing the slng and dlng
structures.
All families in the Google Fonts collection should contain the &#x27;meta&#x27; table.
Windows 10 already uses it when deciding on which fonts to fall back to. The
Google Fonts API and also other environments could use the data for smarter
filtering. Most importantly, those entries should be added to the Noto fonts.
In the font making process, some environments store this data in external files
already. But the meta table provides a convenient way to store this inside the
font file, so some tools may add the data, and unrelated tools may read this
data. This makes the solution much more portable and universal.</pre>

* ⚠ **WARN** This font file does not have a 'meta' table. [code: lacks-meta-table]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check font contains no unreachable glyphs</summary>

* [com.google.fonts/check/unreachable_glyphs](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/universal.html#com.google.fonts/check/unreachable_glyphs)
<pre>--- Rationale ---
Glyphs are either accessible directly through Unicode codepoints or through
substitution rules. Any glyphs not accessible by either of these means are
redundant and serve only to increase the font&#x27;s file size.</pre>

* ⚠ **WARN** The following glyphs could not be reached by codepoint or substitution rules:
 - Euro.BRACKET.125
 - parenright.denominator
 - .null
 - yen.BRACKET.125
 - parenleft.numerator
 - uni030C.alt
 - brevecombcy
 - parenleft.denominator
 - uni20B4.BRACKET.125 
 - parenright.numerator
 [code: unreachable-glyphs]

</details>
<details>
<summary>⚠ <b>WARN:</b> Are there any misaligned on-curve points?</summary>

* [com.google.fonts/check/outline_alignment_miss](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_alignment_miss)
<pre>--- Rationale ---
This check heuristically looks for on-curve points which are close to, but do
not sit on, significant boundary coordinates. For example, a point which has a
Y-coordinate of 1 or -1 might be a misplaced baseline point. As well as the
baseline, here we also check for points near the x-height (but only for lower
case Latin letters), cap-height, ascender and descender Y coordinates.
Not all such misaligned curve points are a mistake, and sometimes the design may
call for points in locations near the boundaries. As this check is liable to
generate significant numbers of false positives, it will pass if there are more
than 100 reported misalignments.</pre>

* ⚠ **WARN** The following glyphs have on-curve points which have potentially incorrect y coordinates:
	* dollar (U+0024): X=465.0,Y=702.0 (should be at cap-height 700?)
	* at (U+0040): X=694.0,Y=0.5 (should be at baseline 0?)
	* cent (U+00A2): X=162.0,Y=1.0 (should be at baseline 0?)
	* uni00B5 (U+00B5): X=160.0,Y=2.0 (should be at baseline 0?)
	* atilde (U+00E3): X=404.0,Y=702.0 (should be at cap-height 700?)
	* atilde (U+00E3): X=455.5,Y=700.5 (should be at cap-height 700?)
	* ntilde (U+00F1): X=418.0,Y=702.0 (should be at cap-height 700?)
	* ntilde (U+00F1): X=469.5,Y=700.5 (should be at cap-height 700?)
	* otilde (U+00F5): X=401.0,Y=702.0 (should be at cap-height 700?)
	* otilde (U+00F5): X=452.5,Y=700.5 (should be at cap-height 700?) and 35 more. [code: found-misalignments]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do any segments have colinear vectors?</summary>

* [com.google.fonts/check/outline_colinear_vectors](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_colinear_vectors)
<pre>--- Rationale ---
This check looks for consecutive line segments which have the same angle. This
normally happens if an outline point has been added by accident.
This check is not run for variable fonts, as they may legitimately have colinear
vectors.</pre>

* ⚠ **WARN** The following glyphs have colinear vectors:
	* uni04A1 (U+04A1): L<<217.0,402.0>--<216.0,402.0>> -> L<<216.0,402.0>--<69.0,402.0>>
	* uni05DC (U+05DC): L<<237.0,448.0>--<236.0,448.0>> -> L<<236.0,448.0>--<113.0,448.0>>
	* uni05DC (U+05DC): L<<262.0,448.0>--<237.0,448.0>> -> L<<237.0,448.0>--<236.0,448.0>>
	* uniFB3C (U+FB3C): L<<237.0,448.0>--<236.0,448.0>> -> L<<236.0,448.0>--<113.0,448.0>> and uniFB3C (U+FB3C): L<<262.0,448.0>--<237.0,448.0>> -> L<<237.0,448.0>--<236.0,448.0>> [code: found-colinear-vectors]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do outlines contain any jaggy segments?</summary>

* [com.google.fonts/check/outline_jaggy_segments](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_jaggy_segments)
<pre>--- Rationale ---
This check heuristically detects outline segments which form a particularly
small angle, indicative of an outline error. This may cause false positives in
cases such as extreme ink traps, so should be regarded as advisory and backed up
by manual inspection.</pre>

* ⚠ **WARN** The following glyphs have jaggy segments:
	* uni0494 (U+0494): B<<242.0,255.0>-<220.0,236.0>-<213.0,199.0>>/L<<213.0,199.0>--<213.0,201.0>> = 10.713123022791033 and uni0494 (U+0494): L<<213.0,199.0>--<213.0,201.0>>/L<<213.0,201.0>--<175.0,25.0>> = 12.183656585987368 [code: found-jaggy-segments]

</details>
<br>
</details>
<details>
<summary><b>[11] Rubik-ExtraBold.ttf</b></summary>
<details>
<summary>💔 <b>ERROR:</b> Check samples can be rendered.</summary>

* [com.google.fonts/check/metadata/can_render_samples](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/metadata/can_render_samples)
<pre>--- Rationale ---
In order to prevent tofu from being seen on fonts.google.com, this check
verifies that all samples provided on METADATA.pb can be properly rendered by
the font.</pre>

* 💔 **ERROR** Failed with AttributeError: 'NoneType' object has no attribute 'sample_glyphs'

</details>
<details>
<summary>🔥 <b>FAIL:</b> Check license file has good copyright string.</summary>

* [com.google.fonts/check/license/OFL_copyright](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/license/OFL_copyright)
<pre>--- Rationale ---
An OFL.txt file&#x27;s first line should be the font copyright e.g:
&quot;Copyright 2019 The Montserrat Project Authors
(https://github.com/julietaula/montserrat)&quot;</pre>

* 🔥 **FAIL** First line in license file does not match expected format: "copyright 20** the my font project authors (https://github.com/googlefonts/my-font-repository)"

</details>
<details>
<summary>⚠ <b>WARN:</b> Checking OS/2 achVendID.</summary>

* [com.google.fonts/check/vendor_id](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/vendor_id)
<pre>--- Rationale ---
Microsoft keeps a list of font vendors and their respective contact info. This
list is updated regularly and is indexed by a 4-char &quot;Vendor ID&quot; which is stored
in the achVendID field of the OS/2 table.
Registering your ID is not mandatory, but it is a good practice since some
applications may display the type designer / type foundry contact info on some
dialog and also because that info will be visible on Microsoft&#x27;s website:
https://docs.microsoft.com/en-us/typography/vendors/
This check verifies whether or not a given font&#x27;s vendor ID is registered in
that list or if it has some of the default values used by the most common font
editors.
Each new FontBakery release includes a cached copy of that list of vendor IDs.
If you registered recently, you&#x27;re safe to ignore warnings emitted by this
check, since your ID will soon be included in one of our upcoming releases.</pre>

* ⚠ **WARN** OS/2 VendorID value 'NONE' is not yet recognized. If you registered it recently, then it's safe to ignore this warning message. Otherwise, you should set it to your own unique 4 character code, and register it with Microsoft at https://www.microsoft.com/typography/links/vendorlist.aspx
 [code: unknown]

</details>
<details>
<summary>⚠ <b>WARN:</b> Font has old ttfautohint applied?</summary>

* [com.google.fonts/check/old_ttfautohint](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/old_ttfautohint)
<pre>--- Rationale ---
Check if font has been hinted with an outdated version of ttfautohint.</pre>

* ⚠ **WARN** ttfautohint used in font = 1.8.3; latest = 1.8.4; Need to re-run with the newer version! [code: old-ttfa]

</details>
<details>
<summary>⚠ <b>WARN:</b> Glyphs are similiar to Google Fonts version?</summary>

* [com.google.fonts/check/production_glyphs_similarity](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/production_glyphs_similarity)

* ⚠ **WARN** Following glyphs differ greatly from Google Fonts version: [Euro, Hbar, Ustraitstrokecy, hbar, uni040E, uni0423, uni0443, uni044E, uni045E, uni0462, uni0463, uni0473, uni0492, uni0496, uni0497, uni0498, uni0499, uni049A, uni049B, uni04A2, uni04A3, uni04AA, uni04AB, uni04B6, uni04B7, uni04B8, uni04B9, uni04CB, uni04CC, uni04E8, uni04E9, uni04EE, uni04EF, uni04F0, uni04F1, uni04F2, uni04F3, uni04F6, uni04F7, uni0524, uni0525, uni05B8, uni05D2, uni05DC, uni05DE, uni05E0, uni05E2, uni05EA, uni20AE, uni20B4, uni20B4.BRACKET.125, uni20B9, uniFB2F, uniFB32, uniFB3C, uniFB3E, uniFB40, uniFB4A, yen, zero.tf.zero, zero.zero]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check if each glyph has the recommended amount of contours.</summary>

* [com.google.fonts/check/contour_count](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/contour_count)
<pre>--- Rationale ---
Visually QAing thousands of glyphs by hand is tiring. Most glyphs can only be
constructured in a handful of ways. This means a glyph&#x27;s contour count will only
differ slightly amongst different fonts, e.g a &#x27;g&#x27; could either be 2 or 3
contours, depending on whether its double story or single story.
However, a quotedbl should have 2 contours, unless the font belongs to a display
family.
This check currently does not cover variable fonts because there&#x27;s plenty of
alternative ways of constructing glyphs with multiple outlines for each feature
in a VarFont. The expected contour count data for this check is currently
optimized for the typical construction of glyphs in static fonts.</pre>

* ⚠ **WARN** This check inspects the glyph outlines and detects the total number of contours in each of them. The expected values are infered from the typical ammounts of contours observed in a large collection of reference font families. The divergences listed below may simply indicate a significantly different design on some of your glyphs. On the other hand, some of these may flag actual bugs in the font such as glyphs mapped to an incorrect codepoint. Please consider reviewing the design and codepoint assignment of these to make sure they are correct.

The following glyphs do not have the recommended number of contours:

Glyph name: uni0493	Contours detected: 2	Expected: 1
Glyph name: ustraitstrokecy	Contours detected: 2	Expected: 1
Glyph name: fi	Contours detected: 1	Expected: 3
Glyph name: fl	Contours detected: 1	Expected: 2
Glyph name: uni0493	Contours detected: 2	Expected: 1 [code: contour-count]

</details>
<details>
<summary>⚠ <b>WARN:</b> Is there kerning info for non-ligated sequences?</summary>

* [com.google.fonts/check/kerning_for_non_ligated_sequences](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/kerning_for_non_ligated_sequences)
<pre>--- Rationale ---
Fonts with ligatures should have kerning on the corresponding non-ligated
sequences for text where ligatures aren&#x27;t used (eg
https://github.com/impallari/Raleway/issues/14).</pre>

* ⚠ **WARN** GPOS table lacks kerning info for the following non-ligated sequences:
	- f + f
	- f + i
	- i + f
	- f + l
	- l + f
	- i + l

   [code: lacks-kern-info]

</details>
<details>
<summary>⚠ <b>WARN:</b> Ensure fonts have ScriptLangTags declared on the 'meta' table.</summary>

* [com.google.fonts/check/meta/script_lang_tags](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/meta/script_lang_tags)
<pre>--- Rationale ---
The OpenType &#x27;meta&#x27; table originated at Apple. Microsoft added it to OT with
just two DataMap records:
- dlng: comma-separated ScriptLangTags that indicate which scripts, or languages
and scripts, with possible variants, the font is designed for
- slng: comma-separated ScriptLangTags that indicate which scripts, or languages
and scripts, with possible variants, the font supports
The slng structure is intended to describe which languages and scripts the font
overall supports. For example, a Traditional Chinese font that also contains
Latin characters, can indicate Hant,Latn, showing that it supports Hant, the
Traditional Chinese variant of the Hani script, and it also supports the Latn
script
The dlng structure is far more interesting. A font may contain various glyphs,
but only a particular subset of the glyphs may be truly &quot;leading&quot; in the design,
while other glyphs may have been included for technical reasons. Such a
Traditional Chinese font could only list Hant there, showing that it’s designed
for Traditional Chinese, but the font would omit Latn, because the developers
don’t think the font is really recommended for purely Latin-script use.
The tags used in the structures can comprise just script, or also language and
script. For example, if a font has Bulgarian Cyrillic alternates in the locl
feature for the cyrl BGR OT languagesystem, it could also indicate in dlng
explicitly that it supports bul-Cyrl. (Note that the scripts and languages in
meta use the ISO language and script codes, not the OpenType ones).
This check ensures that the font has the meta table containing the slng and dlng
structures.
All families in the Google Fonts collection should contain the &#x27;meta&#x27; table.
Windows 10 already uses it when deciding on which fonts to fall back to. The
Google Fonts API and also other environments could use the data for smarter
filtering. Most importantly, those entries should be added to the Noto fonts.
In the font making process, some environments store this data in external files
already. But the meta table provides a convenient way to store this inside the
font file, so some tools may add the data, and unrelated tools may read this
data. This makes the solution much more portable and universal.</pre>

* ⚠ **WARN** This font file does not have a 'meta' table. [code: lacks-meta-table]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check font contains no unreachable glyphs</summary>

* [com.google.fonts/check/unreachable_glyphs](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/universal.html#com.google.fonts/check/unreachable_glyphs)
<pre>--- Rationale ---
Glyphs are either accessible directly through Unicode codepoints or through
substitution rules. Any glyphs not accessible by either of these means are
redundant and serve only to increase the font&#x27;s file size.</pre>

* ⚠ **WARN** The following glyphs could not be reached by codepoint or substitution rules:
 - Euro.BRACKET.125
 - parenright.denominator
 - .null
 - yen.BRACKET.125
 - parenleft.numerator
 - uni030C.alt
 - brevecombcy
 - parenleft.denominator
 - uni20B4.BRACKET.125 
 - parenright.numerator
 [code: unreachable-glyphs]

</details>
<details>
<summary>⚠ <b>WARN:</b> Are there any misaligned on-curve points?</summary>

* [com.google.fonts/check/outline_alignment_miss](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_alignment_miss)
<pre>--- Rationale ---
This check heuristically looks for on-curve points which are close to, but do
not sit on, significant boundary coordinates. For example, a point which has a
Y-coordinate of 1 or -1 might be a misplaced baseline point. As well as the
baseline, here we also check for points near the x-height (but only for lower
case Latin letters), cap-height, ascender and descender Y coordinates.
Not all such misaligned curve points are a mistake, and sometimes the design may
call for points in locations near the boundaries. As this check is liable to
generate significant numbers of false positives, it will pass if there are more
than 100 reported misalignments.</pre>

* ⚠ **WARN** The following glyphs have on-curve points which have potentially incorrect y coordinates:
	* quotedbl (U+0022): X=272.5,Y=701.0 (should be at cap-height 700?)
	* quotedbl (U+0022): X=445.0,Y=701.0 (should be at cap-height 700?)
	* quotedbl (U+0022): X=40.0,Y=701.0 (should be at cap-height 700?)
	* quotedbl (U+0022): X=213.0,Y=701.0 (should be at cap-height 700?)
	* dollar (U+0024): X=419.0,Y=702.0 (should be at cap-height 700?)
	* ampersand (U+0026): X=407.5,Y=1.5 (should be at baseline 0?)
	* quotesingle (U+0027): X=40.0,Y=701.0 (should be at cap-height 700?)
	* quotesingle (U+0027): X=213.0,Y=701.0 (should be at cap-height 700?)
	* parenleft (U+0028): X=355.0,Y=-1.0 (should be at baseline 0?)
	* parenright (U+0029): X=48.0,Y=-1.0 (should be at baseline 0?) and 46 more. [code: found-misalignments]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do outlines contain any semi-vertical or semi-horizontal lines?</summary>

* [com.google.fonts/check/outline_semi_vertical](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_semi_vertical)
<pre>--- Rationale ---
This check detects line segments which are nearly, but not quite, exactly
horizontal or vertical. Sometimes such lines are created by design, but often
they are indicative of a design error.
This check is disabled for italic styles, which often contain nearly-upright
lines.</pre>

* ⚠ **WARN** The following glyphs have semi-vertical/semi-horizontal lines:
 * g (U+0067): L<<597.0,494.0>--<598.0,16.0>>
 * gbreve (U+011F): L<<597.0,494.0>--<598.0,16.0>>
 * gcircumflex (U+011D): L<<597.0,494.0>--<598.0,16.0>>
 * gdotaccent (U+0121): L<<597.0,494.0>--<598.0,16.0>>
 * uni0123 (U+0123): L<<597.0,494.0>--<598.0,16.0>>
 * uni0474 (U+0474): L<<719.0,675.0>--<718.0,528.0>>
 * uni05E9 (U+05E9): L<<228.0,546.0>--<229.0,318.0>>
 * uniFB2A (U+FB2A): L<<228.0,546.0>--<229.0,318.0>>
 * uniFB2B (U+FB2B): L<<228.0,546.0>--<229.0,318.0>>
 * uniFB2C (U+FB2C): L<<228.0,546.0>--<229.0,318.0>> and 3 more. [code: found-semi-vertical]

</details>
<br>
</details>
<details>
<summary><b>[12] Rubik-Bold.ttf</b></summary>
<details>
<summary>💔 <b>ERROR:</b> Check samples can be rendered.</summary>

* [com.google.fonts/check/metadata/can_render_samples](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/metadata/can_render_samples)
<pre>--- Rationale ---
In order to prevent tofu from being seen on fonts.google.com, this check
verifies that all samples provided on METADATA.pb can be properly rendered by
the font.</pre>

* 💔 **ERROR** Failed with AttributeError: 'NoneType' object has no attribute 'sample_glyphs'

</details>
<details>
<summary>🔥 <b>FAIL:</b> Check license file has good copyright string.</summary>

* [com.google.fonts/check/license/OFL_copyright](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/license/OFL_copyright)
<pre>--- Rationale ---
An OFL.txt file&#x27;s first line should be the font copyright e.g:
&quot;Copyright 2019 The Montserrat Project Authors
(https://github.com/julietaula/montserrat)&quot;</pre>

* 🔥 **FAIL** First line in license file does not match expected format: "copyright 20** the my font project authors (https://github.com/googlefonts/my-font-repository)"

</details>
<details>
<summary>⚠ <b>WARN:</b> Checking OS/2 achVendID.</summary>

* [com.google.fonts/check/vendor_id](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/vendor_id)
<pre>--- Rationale ---
Microsoft keeps a list of font vendors and their respective contact info. This
list is updated regularly and is indexed by a 4-char &quot;Vendor ID&quot; which is stored
in the achVendID field of the OS/2 table.
Registering your ID is not mandatory, but it is a good practice since some
applications may display the type designer / type foundry contact info on some
dialog and also because that info will be visible on Microsoft&#x27;s website:
https://docs.microsoft.com/en-us/typography/vendors/
This check verifies whether or not a given font&#x27;s vendor ID is registered in
that list or if it has some of the default values used by the most common font
editors.
Each new FontBakery release includes a cached copy of that list of vendor IDs.
If you registered recently, you&#x27;re safe to ignore warnings emitted by this
check, since your ID will soon be included in one of our upcoming releases.</pre>

* ⚠ **WARN** OS/2 VendorID value 'NONE' is not yet recognized. If you registered it recently, then it's safe to ignore this warning message. Otherwise, you should set it to your own unique 4 character code, and register it with Microsoft at https://www.microsoft.com/typography/links/vendorlist.aspx
 [code: unknown]

</details>
<details>
<summary>⚠ <b>WARN:</b> Font has old ttfautohint applied?</summary>

* [com.google.fonts/check/old_ttfautohint](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/old_ttfautohint)
<pre>--- Rationale ---
Check if font has been hinted with an outdated version of ttfautohint.</pre>

* ⚠ **WARN** ttfautohint used in font = 1.8.3; latest = 1.8.4; Need to re-run with the newer version! [code: old-ttfa]

</details>
<details>
<summary>⚠ <b>WARN:</b> Glyphs are similiar to Google Fonts version?</summary>

* [com.google.fonts/check/production_glyphs_similarity](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/production_glyphs_similarity)

* ⚠ **WARN** Following glyphs differ greatly from Google Fonts version: [Euro, Euro.BRACKET.125, Hbar, Ustraitstrokecy, hbar, uni044E, uni0462, uni0463, uni0473, uni0492, uni0496, uni0497, uni0498, uni0499, uni049A, uni049B, uni04A2, uni04A3, uni04AA, uni04AB, uni04B6, uni04B7, uni04B8, uni04B9, uni04CB, uni04CC, uni04E8, uni04E9, uni04F6, uni04F7, uni0524, uni0525, uni05B8, uni05D2, uni05DC, uni05DE, uni05E0, uni05E2, uni05EA, uni20AE, uni20B4, uni20B4.BRACKET.125, uni20B9, uniFB2F, uniFB32, uniFB3C, uniFB3E, uniFB40, uniFB4A, yen, yen.BRACKET.125, zero.tf.zero, zero.zero]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check if each glyph has the recommended amount of contours.</summary>

* [com.google.fonts/check/contour_count](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/contour_count)
<pre>--- Rationale ---
Visually QAing thousands of glyphs by hand is tiring. Most glyphs can only be
constructured in a handful of ways. This means a glyph&#x27;s contour count will only
differ slightly amongst different fonts, e.g a &#x27;g&#x27; could either be 2 or 3
contours, depending on whether its double story or single story.
However, a quotedbl should have 2 contours, unless the font belongs to a display
family.
This check currently does not cover variable fonts because there&#x27;s plenty of
alternative ways of constructing glyphs with multiple outlines for each feature
in a VarFont. The expected contour count data for this check is currently
optimized for the typical construction of glyphs in static fonts.</pre>

* ⚠ **WARN** This check inspects the glyph outlines and detects the total number of contours in each of them. The expected values are infered from the typical ammounts of contours observed in a large collection of reference font families. The divergences listed below may simply indicate a significantly different design on some of your glyphs. On the other hand, some of these may flag actual bugs in the font such as glyphs mapped to an incorrect codepoint. Please consider reviewing the design and codepoint assignment of these to make sure they are correct.

The following glyphs do not have the recommended number of contours:

Glyph name: uni0493	Contours detected: 2	Expected: 1
Glyph name: ustraitstrokecy	Contours detected: 2	Expected: 1
Glyph name: fi	Contours detected: 1	Expected: 3
Glyph name: fl	Contours detected: 1	Expected: 2
Glyph name: uni0493	Contours detected: 2	Expected: 1 [code: contour-count]

</details>
<details>
<summary>⚠ <b>WARN:</b> Is there kerning info for non-ligated sequences?</summary>

* [com.google.fonts/check/kerning_for_non_ligated_sequences](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/kerning_for_non_ligated_sequences)
<pre>--- Rationale ---
Fonts with ligatures should have kerning on the corresponding non-ligated
sequences for text where ligatures aren&#x27;t used (eg
https://github.com/impallari/Raleway/issues/14).</pre>

* ⚠ **WARN** GPOS table lacks kerning info for the following non-ligated sequences:
	- f + f
	- f + i
	- i + f
	- f + l
	- l + f
	- i + l

   [code: lacks-kern-info]

</details>
<details>
<summary>⚠ <b>WARN:</b> Ensure fonts have ScriptLangTags declared on the 'meta' table.</summary>

* [com.google.fonts/check/meta/script_lang_tags](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/meta/script_lang_tags)
<pre>--- Rationale ---
The OpenType &#x27;meta&#x27; table originated at Apple. Microsoft added it to OT with
just two DataMap records:
- dlng: comma-separated ScriptLangTags that indicate which scripts, or languages
and scripts, with possible variants, the font is designed for
- slng: comma-separated ScriptLangTags that indicate which scripts, or languages
and scripts, with possible variants, the font supports
The slng structure is intended to describe which languages and scripts the font
overall supports. For example, a Traditional Chinese font that also contains
Latin characters, can indicate Hant,Latn, showing that it supports Hant, the
Traditional Chinese variant of the Hani script, and it also supports the Latn
script
The dlng structure is far more interesting. A font may contain various glyphs,
but only a particular subset of the glyphs may be truly &quot;leading&quot; in the design,
while other glyphs may have been included for technical reasons. Such a
Traditional Chinese font could only list Hant there, showing that it’s designed
for Traditional Chinese, but the font would omit Latn, because the developers
don’t think the font is really recommended for purely Latin-script use.
The tags used in the structures can comprise just script, or also language and
script. For example, if a font has Bulgarian Cyrillic alternates in the locl
feature for the cyrl BGR OT languagesystem, it could also indicate in dlng
explicitly that it supports bul-Cyrl. (Note that the scripts and languages in
meta use the ISO language and script codes, not the OpenType ones).
This check ensures that the font has the meta table containing the slng and dlng
structures.
All families in the Google Fonts collection should contain the &#x27;meta&#x27; table.
Windows 10 already uses it when deciding on which fonts to fall back to. The
Google Fonts API and also other environments could use the data for smarter
filtering. Most importantly, those entries should be added to the Noto fonts.
In the font making process, some environments store this data in external files
already. But the meta table provides a convenient way to store this inside the
font file, so some tools may add the data, and unrelated tools may read this
data. This makes the solution much more portable and universal.</pre>

* ⚠ **WARN** This font file does not have a 'meta' table. [code: lacks-meta-table]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check font contains no unreachable glyphs</summary>

* [com.google.fonts/check/unreachable_glyphs](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/universal.html#com.google.fonts/check/unreachable_glyphs)
<pre>--- Rationale ---
Glyphs are either accessible directly through Unicode codepoints or through
substitution rules. Any glyphs not accessible by either of these means are
redundant and serve only to increase the font&#x27;s file size.</pre>

* ⚠ **WARN** The following glyphs could not be reached by codepoint or substitution rules:
 - Euro.BRACKET.125
 - parenright.denominator
 - .null
 - yen.BRACKET.125
 - parenleft.numerator
 - uni030C.alt
 - brevecombcy
 - parenleft.denominator
 - uni20B4.BRACKET.125 
 - parenright.numerator
 [code: unreachable-glyphs]

</details>
<details>
<summary>⚠ <b>WARN:</b> Are there any misaligned on-curve points?</summary>

* [com.google.fonts/check/outline_alignment_miss](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_alignment_miss)
<pre>--- Rationale ---
This check heuristically looks for on-curve points which are close to, but do
not sit on, significant boundary coordinates. For example, a point which has a
Y-coordinate of 1 or -1 might be a misplaced baseline point. As well as the
baseline, here we also check for points near the x-height (but only for lower
case Latin letters), cap-height, ascender and descender Y coordinates.
Not all such misaligned curve points are a mistake, and sometimes the design may
call for points in locations near the boundaries. As this check is liable to
generate significant numbers of false positives, it will pass if there are more
than 100 reported misalignments.</pre>

* ⚠ **WARN** The following glyphs have on-curve points which have potentially incorrect y coordinates:
	* quotedbl (U+0022): X=255.5,Y=702.0 (should be at cap-height 700?)
	* quotedbl (U+0022): X=405.5,Y=702.0 (should be at cap-height 700?)
	* quotedbl (U+0022): X=46.5,Y=702.0 (should be at cap-height 700?)
	* quotedbl (U+0022): X=196.5,Y=702.0 (should be at cap-height 700?)
	* quotesingle (U+0027): X=46.5,Y=702.0 (should be at cap-height 700?)
	* quotesingle (U+0027): X=196.5,Y=702.0 (should be at cap-height 700?)
	* cent (U+00A2): X=221.0,Y=-1.0 (should be at baseline 0?)
	* cent (U+00A2): X=370.0,Y=-2.0 (should be at baseline 0?)
	* macron (U+00AF): X=58.0,Y=698.0 (should be at cap-height 700?)
	* macron (U+00AF): X=382.0,Y=698.0 (should be at cap-height 700?) and 50 more. [code: found-misalignments]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do any segments have colinear vectors?</summary>

* [com.google.fonts/check/outline_colinear_vectors](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_colinear_vectors)
<pre>--- Rationale ---
This check looks for consecutive line segments which have the same angle. This
normally happens if an outline point has been added by accident.
This check is not run for variable fonts, as they may legitimately have colinear
vectors.</pre>

* ⚠ **WARN** The following glyphs have colinear vectors:
	* uni05DC (U+05DC): L<<195.0,434.0>--<193.0,434.0>> -> L<<193.0,434.0>--<61.0,434.0>>
	* uni05DC (U+05DC): L<<218.0,434.0>--<195.0,434.0>> -> L<<195.0,434.0>--<193.0,434.0>>
	* uniFB3C (U+FB3C): L<<195.0,434.0>--<193.0,434.0>> -> L<<193.0,434.0>--<61.0,434.0>> and uniFB3C (U+FB3C): L<<218.0,434.0>--<195.0,434.0>> -> L<<195.0,434.0>--<193.0,434.0>> [code: found-colinear-vectors]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do outlines contain any semi-vertical or semi-horizontal lines?</summary>

* [com.google.fonts/check/outline_semi_vertical](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_semi_vertical)
<pre>--- Rationale ---
This check detects line segments which are nearly, but not quite, exactly
horizontal or vertical. Sometimes such lines are created by design, but often
they are indicative of a design error.
This check is disabled for italic styles, which often contain nearly-upright
lines.</pre>

* ⚠ **WARN** The following glyphs have semi-vertical/semi-horizontal lines:
 * uni0434 (U+0434): L<<249.0,131.0>--<399.0,132.0>>
 * uni0446 (U+0446): L<<568.0,495.0>--<567.0,131.0>>
 * uni0474 (U+0474): L<<702.0,678.0>--<701.0,561.0>>
 * uni05E3 (U+05E3): L<<527.0,315.0>--<528.0,-99.0>>
 * uni05E9 (U+05E9): L<<207.0,547.0>--<208.0,302.0>>
 * uni05EA (U+05EA): L<<275.0,0.0>--<68.0,1.0>>
 * uniFB2A (U+FB2A): L<<207.0,547.0>--<208.0,302.0>>
 * uniFB2B (U+FB2B): L<<207.0,547.0>--<208.0,302.0>>
 * uniFB2C (U+FB2C): L<<207.0,547.0>--<208.0,302.0>>
 * uniFB2D (U+FB2D): L<<207.0,547.0>--<208.0,302.0>> and 3 more. [code: found-semi-vertical]

</details>
<br>
</details>
<details>
<summary><b>[12] Rubik-Black.ttf</b></summary>
<details>
<summary>💔 <b>ERROR:</b> Check samples can be rendered.</summary>

* [com.google.fonts/check/metadata/can_render_samples](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/metadata/can_render_samples)
<pre>--- Rationale ---
In order to prevent tofu from being seen on fonts.google.com, this check
verifies that all samples provided on METADATA.pb can be properly rendered by
the font.</pre>

* 💔 **ERROR** Failed with AttributeError: 'NoneType' object has no attribute 'sample_glyphs'

</details>
<details>
<summary>🔥 <b>FAIL:</b> Check license file has good copyright string.</summary>

* [com.google.fonts/check/license/OFL_copyright](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/license/OFL_copyright)
<pre>--- Rationale ---
An OFL.txt file&#x27;s first line should be the font copyright e.g:
&quot;Copyright 2019 The Montserrat Project Authors
(https://github.com/julietaula/montserrat)&quot;</pre>

* 🔥 **FAIL** First line in license file does not match expected format: "copyright 20** the my font project authors (https://github.com/googlefonts/my-font-repository)"

</details>
<details>
<summary>⚠ <b>WARN:</b> Checking OS/2 achVendID.</summary>

* [com.google.fonts/check/vendor_id](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/vendor_id)
<pre>--- Rationale ---
Microsoft keeps a list of font vendors and their respective contact info. This
list is updated regularly and is indexed by a 4-char &quot;Vendor ID&quot; which is stored
in the achVendID field of the OS/2 table.
Registering your ID is not mandatory, but it is a good practice since some
applications may display the type designer / type foundry contact info on some
dialog and also because that info will be visible on Microsoft&#x27;s website:
https://docs.microsoft.com/en-us/typography/vendors/
This check verifies whether or not a given font&#x27;s vendor ID is registered in
that list or if it has some of the default values used by the most common font
editors.
Each new FontBakery release includes a cached copy of that list of vendor IDs.
If you registered recently, you&#x27;re safe to ignore warnings emitted by this
check, since your ID will soon be included in one of our upcoming releases.</pre>

* ⚠ **WARN** OS/2 VendorID value 'NONE' is not yet recognized. If you registered it recently, then it's safe to ignore this warning message. Otherwise, you should set it to your own unique 4 character code, and register it with Microsoft at https://www.microsoft.com/typography/links/vendorlist.aspx
 [code: unknown]

</details>
<details>
<summary>⚠ <b>WARN:</b> Font has old ttfautohint applied?</summary>

* [com.google.fonts/check/old_ttfautohint](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/old_ttfautohint)
<pre>--- Rationale ---
Check if font has been hinted with an outdated version of ttfautohint.</pre>

* ⚠ **WARN** ttfautohint used in font = 1.8.3; latest = 1.8.4; Need to re-run with the newer version! [code: old-ttfa]

</details>
<details>
<summary>⚠ <b>WARN:</b> Glyphs are similiar to Google Fonts version?</summary>

* [com.google.fonts/check/production_glyphs_similarity](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/production_glyphs_similarity)

* ⚠ **WARN** Following glyphs differ greatly from Google Fonts version: [Euro, Euro.BRACKET.125, Hbar, Ustraitstrokecy, hbar, uni040E, uni0423, uni0443, uni044E, uni045E, uni0462, uni0463, uni0473, uni0492, uni0496, uni0497, uni0498, uni0499, uni049A, uni049B, uni04A2, uni04A3, uni04AA, uni04AB, uni04B6, uni04B7, uni04B8, uni04B9, uni04CB, uni04CC, uni04E8, uni04E9, uni04EE, uni04EF, uni04F0, uni04F1, uni04F2, uni04F3, uni04F6, uni04F7, uni0524, uni0525, uni05B8, uni05D2, uni05DC, uni05DE, uni05E0, uni05E2, uni05EA, uni20AE, uni20B4, uni20B9, uniFB2F, uniFB32, uniFB3C, uniFB3E, uniFB40, uniFB4A, yen, zero.tf.zero, zero.zero]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check if each glyph has the recommended amount of contours.</summary>

* [com.google.fonts/check/contour_count](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/contour_count)
<pre>--- Rationale ---
Visually QAing thousands of glyphs by hand is tiring. Most glyphs can only be
constructured in a handful of ways. This means a glyph&#x27;s contour count will only
differ slightly amongst different fonts, e.g a &#x27;g&#x27; could either be 2 or 3
contours, depending on whether its double story or single story.
However, a quotedbl should have 2 contours, unless the font belongs to a display
family.
This check currently does not cover variable fonts because there&#x27;s plenty of
alternative ways of constructing glyphs with multiple outlines for each feature
in a VarFont. The expected contour count data for this check is currently
optimized for the typical construction of glyphs in static fonts.</pre>

* ⚠ **WARN** This check inspects the glyph outlines and detects the total number of contours in each of them. The expected values are infered from the typical ammounts of contours observed in a large collection of reference font families. The divergences listed below may simply indicate a significantly different design on some of your glyphs. On the other hand, some of these may flag actual bugs in the font such as glyphs mapped to an incorrect codepoint. Please consider reviewing the design and codepoint assignment of these to make sure they are correct.

The following glyphs do not have the recommended number of contours:

Glyph name: uni0493	Contours detected: 2	Expected: 1
Glyph name: ustraitstrokecy	Contours detected: 2	Expected: 1
Glyph name: fi	Contours detected: 1	Expected: 3
Glyph name: fl	Contours detected: 1	Expected: 2
Glyph name: uni0493	Contours detected: 2	Expected: 1 [code: contour-count]

</details>
<details>
<summary>⚠ <b>WARN:</b> Is there kerning info for non-ligated sequences?</summary>

* [com.google.fonts/check/kerning_for_non_ligated_sequences](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/kerning_for_non_ligated_sequences)
<pre>--- Rationale ---
Fonts with ligatures should have kerning on the corresponding non-ligated
sequences for text where ligatures aren&#x27;t used (eg
https://github.com/impallari/Raleway/issues/14).</pre>

* ⚠ **WARN** GPOS table lacks kerning info for the following non-ligated sequences:
	- f + f
	- f + i
	- i + f
	- f + l
	- l + f
	- i + l

   [code: lacks-kern-info]

</details>
<details>
<summary>⚠ <b>WARN:</b> Ensure fonts have ScriptLangTags declared on the 'meta' table.</summary>

* [com.google.fonts/check/meta/script_lang_tags](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/meta/script_lang_tags)
<pre>--- Rationale ---
The OpenType &#x27;meta&#x27; table originated at Apple. Microsoft added it to OT with
just two DataMap records:
- dlng: comma-separated ScriptLangTags that indicate which scripts, or languages
and scripts, with possible variants, the font is designed for
- slng: comma-separated ScriptLangTags that indicate which scripts, or languages
and scripts, with possible variants, the font supports
The slng structure is intended to describe which languages and scripts the font
overall supports. For example, a Traditional Chinese font that also contains
Latin characters, can indicate Hant,Latn, showing that it supports Hant, the
Traditional Chinese variant of the Hani script, and it also supports the Latn
script
The dlng structure is far more interesting. A font may contain various glyphs,
but only a particular subset of the glyphs may be truly &quot;leading&quot; in the design,
while other glyphs may have been included for technical reasons. Such a
Traditional Chinese font could only list Hant there, showing that it’s designed
for Traditional Chinese, but the font would omit Latn, because the developers
don’t think the font is really recommended for purely Latin-script use.
The tags used in the structures can comprise just script, or also language and
script. For example, if a font has Bulgarian Cyrillic alternates in the locl
feature for the cyrl BGR OT languagesystem, it could also indicate in dlng
explicitly that it supports bul-Cyrl. (Note that the scripts and languages in
meta use the ISO language and script codes, not the OpenType ones).
This check ensures that the font has the meta table containing the slng and dlng
structures.
All families in the Google Fonts collection should contain the &#x27;meta&#x27; table.
Windows 10 already uses it when deciding on which fonts to fall back to. The
Google Fonts API and also other environments could use the data for smarter
filtering. Most importantly, those entries should be added to the Noto fonts.
In the font making process, some environments store this data in external files
already. But the meta table provides a convenient way to store this inside the
font file, so some tools may add the data, and unrelated tools may read this
data. This makes the solution much more portable and universal.</pre>

* ⚠ **WARN** This font file does not have a 'meta' table. [code: lacks-meta-table]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check font contains no unreachable glyphs</summary>

* [com.google.fonts/check/unreachable_glyphs](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/universal.html#com.google.fonts/check/unreachable_glyphs)
<pre>--- Rationale ---
Glyphs are either accessible directly through Unicode codepoints or through
substitution rules. Any glyphs not accessible by either of these means are
redundant and serve only to increase the font&#x27;s file size.</pre>

* ⚠ **WARN** The following glyphs could not be reached by codepoint or substitution rules:
 - Euro.BRACKET.125
 - parenright.denominator
 - .null
 - yen.BRACKET.125
 - parenleft.numerator
 - uni030C.alt
 - brevecombcy
 - parenleft.denominator
 - uni20B4.BRACKET.125 
 - parenright.numerator
 [code: unreachable-glyphs]

</details>
<details>
<summary>⚠ <b>WARN:</b> Are there any misaligned on-curve points?</summary>

* [com.google.fonts/check/outline_alignment_miss](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_alignment_miss)
<pre>--- Rationale ---
This check heuristically looks for on-curve points which are close to, but do
not sit on, significant boundary coordinates. For example, a point which has a
Y-coordinate of 1 or -1 might be a misplaced baseline point. As well as the
baseline, here we also check for points near the x-height (but only for lower
case Latin letters), cap-height, ascender and descender Y coordinates.
Not all such misaligned curve points are a mistake, and sometimes the design may
call for points in locations near the boundaries. As this check is liable to
generate significant numbers of false positives, it will pass if there are more
than 100 reported misalignments.</pre>

* ⚠ **WARN** The following glyphs have on-curve points which have potentially incorrect y coordinates:
	* quotedbl (U+0022): X=289.5,Y=700.5 (should be at cap-height 700?)
	* quotedbl (U+0022): X=484.5,Y=700.5 (should be at cap-height 700?)
	* quotedbl (U+0022): X=34.5,Y=700.5 (should be at cap-height 700?)
	* quotedbl (U+0022): X=229.5,Y=700.5 (should be at cap-height 700?)
	* ampersand (U+0026): X=406.5,Y=-2.0 (should be at baseline 0?)
	* quotesingle (U+0027): X=34.5,Y=700.5 (should be at cap-height 700?)
	* quotesingle (U+0027): X=229.5,Y=700.5 (should be at cap-height 700?)
	* b (U+0062): X=53.0,Y=702.0 (should be at cap-height 700?)
	* b (U+0062): X=276.0,Y=702.0 (should be at cap-height 700?)
	* d (U+0064): X=385.0,Y=702.0 (should be at cap-height 700?) and 84 more. [code: found-misalignments]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do any segments have colinear vectors?</summary>

* [com.google.fonts/check/outline_colinear_vectors](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_colinear_vectors)
<pre>--- Rationale ---
This check looks for consecutive line segments which have the same angle. This
normally happens if an outline point has been added by accident.
This check is not run for variable fonts, as they may legitimately have colinear
vectors.</pre>

* ⚠ **WARN** The following glyphs have colinear vectors:
	* uni049C (U+049C): L<<393.0,448.0>--<394.0,450.0>> -> L<<394.0,450.0>--<523.0,678.0>>
	* uni05E9 (U+05E9): L<<250.0,545.0>--<250.0,335.0>> -> L<<250.0,335.0>--<250.0,334.0>>
	* uniFB2A (U+FB2A): L<<250.0,545.0>--<250.0,335.0>> -> L<<250.0,335.0>--<250.0,334.0>>
	* uniFB2B (U+FB2B): L<<250.0,545.0>--<250.0,335.0>> -> L<<250.0,335.0>--<250.0,334.0>>
	* uniFB2C (U+FB2C): L<<250.0,545.0>--<250.0,335.0>> -> L<<250.0,335.0>--<250.0,334.0>>
	* uniFB2D (U+FB2D): L<<250.0,545.0>--<250.0,335.0>> -> L<<250.0,335.0>--<250.0,334.0>> and uniFB49 (U+FB49): L<<250.0,545.0>--<250.0,335.0>> -> L<<250.0,335.0>--<250.0,334.0>> [code: found-colinear-vectors]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do outlines contain any semi-vertical or semi-horizontal lines?</summary>

* [com.google.fonts/check/outline_semi_vertical](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_semi_vertical)
<pre>--- Rationale ---
This check detects line segments which are nearly, but not quite, exactly
horizontal or vertical. Sometimes such lines are created by design, but often
they are indicative of a design error.
This check is disabled for italic styles, which often contain nearly-upright
lines.</pre>

* ⚠ **WARN** The following glyphs have semi-vertical/semi-horizontal lines:
 * g (U+0067): L<<620.0,493.0>--<621.0,17.0>>
 * gbreve (U+011F): L<<620.0,493.0>--<621.0,17.0>>
 * gcircumflex (U+011D): L<<620.0,493.0>--<621.0,17.0>>
 * gdotaccent (U+0121): L<<620.0,493.0>--<621.0,17.0>>
 * uni0123 (U+0123): L<<620.0,493.0>--<621.0,17.0>>
 * uni0474 (U+0474): L<<736.0,672.0>--<735.0,495.0>>
 * uni05E3 (U+05E3): L<<548.0,308.0>--<549.0,-97.0>> and uniFB43 (U+FB43): L<<548.0,308.0>--<549.0,-97.0>> [code: found-semi-vertical]

</details>
<br>
</details>
<details>
<summary><b>[12] Rubik-Medium.ttf</b></summary>
<details>
<summary>💔 <b>ERROR:</b> Check samples can be rendered.</summary>

* [com.google.fonts/check/metadata/can_render_samples](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/metadata/can_render_samples)
<pre>--- Rationale ---
In order to prevent tofu from being seen on fonts.google.com, this check
verifies that all samples provided on METADATA.pb can be properly rendered by
the font.</pre>

* 💔 **ERROR** Failed with AttributeError: 'NoneType' object has no attribute 'sample_glyphs'

</details>
<details>
<summary>🔥 <b>FAIL:</b> Check license file has good copyright string.</summary>

* [com.google.fonts/check/license/OFL_copyright](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/license/OFL_copyright)
<pre>--- Rationale ---
An OFL.txt file&#x27;s first line should be the font copyright e.g:
&quot;Copyright 2019 The Montserrat Project Authors
(https://github.com/julietaula/montserrat)&quot;</pre>

* 🔥 **FAIL** First line in license file does not match expected format: "copyright 20** the my font project authors (https://github.com/googlefonts/my-font-repository)"

</details>
<details>
<summary>⚠ <b>WARN:</b> Checking OS/2 achVendID.</summary>

* [com.google.fonts/check/vendor_id](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/vendor_id)
<pre>--- Rationale ---
Microsoft keeps a list of font vendors and their respective contact info. This
list is updated regularly and is indexed by a 4-char &quot;Vendor ID&quot; which is stored
in the achVendID field of the OS/2 table.
Registering your ID is not mandatory, but it is a good practice since some
applications may display the type designer / type foundry contact info on some
dialog and also because that info will be visible on Microsoft&#x27;s website:
https://docs.microsoft.com/en-us/typography/vendors/
This check verifies whether or not a given font&#x27;s vendor ID is registered in
that list or if it has some of the default values used by the most common font
editors.
Each new FontBakery release includes a cached copy of that list of vendor IDs.
If you registered recently, you&#x27;re safe to ignore warnings emitted by this
check, since your ID will soon be included in one of our upcoming releases.</pre>

* ⚠ **WARN** OS/2 VendorID value 'NONE' is not yet recognized. If you registered it recently, then it's safe to ignore this warning message. Otherwise, you should set it to your own unique 4 character code, and register it with Microsoft at https://www.microsoft.com/typography/links/vendorlist.aspx
 [code: unknown]

</details>
<details>
<summary>⚠ <b>WARN:</b> Font has old ttfautohint applied?</summary>

* [com.google.fonts/check/old_ttfautohint](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/old_ttfautohint)
<pre>--- Rationale ---
Check if font has been hinted with an outdated version of ttfautohint.</pre>

* ⚠ **WARN** ttfautohint used in font = 1.8.3; latest = 1.8.4; Need to re-run with the newer version! [code: old-ttfa]

</details>
<details>
<summary>⚠ <b>WARN:</b> Glyphs are similiar to Google Fonts version?</summary>

* [com.google.fonts/check/production_glyphs_similarity](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/production_glyphs_similarity)

* ⚠ **WARN** Following glyphs differ greatly from Google Fonts version: [Euro, Euro.BRACKET.125, Hbar, Ustraitstrokecy, hbar, uni044E, uni0462, uni0463, uni0473, uni0492, uni0496, uni0497, uni049A, uni049B, uni04A2, uni04A3, uni04B6, uni04B7, uni04CB, uni04CC, uni04E8, uni04E9, uni04F6, uni04F7, uni0524, uni0525, uni05B8, uni05D2, uni05E0, uni05E2, uni20AE, uni20B4, uni20B4.BRACKET.125, uni20B9, uniFB32, uniFB40, yen, yen.BRACKET.125, zero.tf.zero, zero.zero]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check if each glyph has the recommended amount of contours.</summary>

* [com.google.fonts/check/contour_count](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/contour_count)
<pre>--- Rationale ---
Visually QAing thousands of glyphs by hand is tiring. Most glyphs can only be
constructured in a handful of ways. This means a glyph&#x27;s contour count will only
differ slightly amongst different fonts, e.g a &#x27;g&#x27; could either be 2 or 3
contours, depending on whether its double story or single story.
However, a quotedbl should have 2 contours, unless the font belongs to a display
family.
This check currently does not cover variable fonts because there&#x27;s plenty of
alternative ways of constructing glyphs with multiple outlines for each feature
in a VarFont. The expected contour count data for this check is currently
optimized for the typical construction of glyphs in static fonts.</pre>

* ⚠ **WARN** This check inspects the glyph outlines and detects the total number of contours in each of them. The expected values are infered from the typical ammounts of contours observed in a large collection of reference font families. The divergences listed below may simply indicate a significantly different design on some of your glyphs. On the other hand, some of these may flag actual bugs in the font such as glyphs mapped to an incorrect codepoint. Please consider reviewing the design and codepoint assignment of these to make sure they are correct.

The following glyphs do not have the recommended number of contours:

Glyph name: uni0493	Contours detected: 2	Expected: 1
Glyph name: ustraitstrokecy	Contours detected: 2	Expected: 1
Glyph name: fi	Contours detected: 1	Expected: 3
Glyph name: fl	Contours detected: 1	Expected: 2
Glyph name: uni0493	Contours detected: 2	Expected: 1 [code: contour-count]

</details>
<details>
<summary>⚠ <b>WARN:</b> Is there kerning info for non-ligated sequences?</summary>

* [com.google.fonts/check/kerning_for_non_ligated_sequences](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/kerning_for_non_ligated_sequences)
<pre>--- Rationale ---
Fonts with ligatures should have kerning on the corresponding non-ligated
sequences for text where ligatures aren&#x27;t used (eg
https://github.com/impallari/Raleway/issues/14).</pre>

* ⚠ **WARN** GPOS table lacks kerning info for the following non-ligated sequences:
	- f + f
	- f + i
	- i + f
	- f + l
	- l + f
	- i + l

   [code: lacks-kern-info]

</details>
<details>
<summary>⚠ <b>WARN:</b> Ensure fonts have ScriptLangTags declared on the 'meta' table.</summary>

* [com.google.fonts/check/meta/script_lang_tags](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/meta/script_lang_tags)
<pre>--- Rationale ---
The OpenType &#x27;meta&#x27; table originated at Apple. Microsoft added it to OT with
just two DataMap records:
- dlng: comma-separated ScriptLangTags that indicate which scripts, or languages
and scripts, with possible variants, the font is designed for
- slng: comma-separated ScriptLangTags that indicate which scripts, or languages
and scripts, with possible variants, the font supports
The slng structure is intended to describe which languages and scripts the font
overall supports. For example, a Traditional Chinese font that also contains
Latin characters, can indicate Hant,Latn, showing that it supports Hant, the
Traditional Chinese variant of the Hani script, and it also supports the Latn
script
The dlng structure is far more interesting. A font may contain various glyphs,
but only a particular subset of the glyphs may be truly &quot;leading&quot; in the design,
while other glyphs may have been included for technical reasons. Such a
Traditional Chinese font could only list Hant there, showing that it’s designed
for Traditional Chinese, but the font would omit Latn, because the developers
don’t think the font is really recommended for purely Latin-script use.
The tags used in the structures can comprise just script, or also language and
script. For example, if a font has Bulgarian Cyrillic alternates in the locl
feature for the cyrl BGR OT languagesystem, it could also indicate in dlng
explicitly that it supports bul-Cyrl. (Note that the scripts and languages in
meta use the ISO language and script codes, not the OpenType ones).
This check ensures that the font has the meta table containing the slng and dlng
structures.
All families in the Google Fonts collection should contain the &#x27;meta&#x27; table.
Windows 10 already uses it when deciding on which fonts to fall back to. The
Google Fonts API and also other environments could use the data for smarter
filtering. Most importantly, those entries should be added to the Noto fonts.
In the font making process, some environments store this data in external files
already. But the meta table provides a convenient way to store this inside the
font file, so some tools may add the data, and unrelated tools may read this
data. This makes the solution much more portable and universal.</pre>

* ⚠ **WARN** This font file does not have a 'meta' table. [code: lacks-meta-table]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check font contains no unreachable glyphs</summary>

* [com.google.fonts/check/unreachable_glyphs](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/universal.html#com.google.fonts/check/unreachable_glyphs)
<pre>--- Rationale ---
Glyphs are either accessible directly through Unicode codepoints or through
substitution rules. Any glyphs not accessible by either of these means are
redundant and serve only to increase the font&#x27;s file size.</pre>

* ⚠ **WARN** The following glyphs could not be reached by codepoint or substitution rules:
 - Euro.BRACKET.125
 - parenright.denominator
 - .null
 - yen.BRACKET.125
 - parenleft.numerator
 - uni030C.alt
 - brevecombcy
 - parenleft.denominator
 - uni20B4.BRACKET.125 
 - parenright.numerator
 [code: unreachable-glyphs]

</details>
<details>
<summary>⚠ <b>WARN:</b> Are there any misaligned on-curve points?</summary>

* [com.google.fonts/check/outline_alignment_miss](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_alignment_miss)
<pre>--- Rationale ---
This check heuristically looks for on-curve points which are close to, but do
not sit on, significant boundary coordinates. For example, a point which has a
Y-coordinate of 1 or -1 might be a misplaced baseline point. As well as the
baseline, here we also check for points near the x-height (but only for lower
case Latin letters), cap-height, ascender and descender Y coordinates.
Not all such misaligned curve points are a mistake, and sometimes the design may
call for points in locations near the boundaries. As this check is liable to
generate significant numbers of false positives, it will pass if there are more
than 100 reported misalignments.</pre>

* ⚠ **WARN** The following glyphs have on-curve points which have potentially incorrect y coordinates:
	* i (U+0069): X=62.0,Y=702.0 (should be at cap-height 700?)
	* i (U+0069): X=202.0,Y=702.0 (should be at cap-height 700?)
	* j (U+006A): X=73.0,Y=702.0 (should be at cap-height 700?)
	* j (U+006A): X=216.0,Y=702.0 (should be at cap-height 700?)
	* j (U+006A): X=77.0,Y=1.0 (should be at baseline 0?)
	* j (U+006A): X=212.0,Y=-1.0 (should be at baseline 0?)
	* braceleft (U+007B): X=255.0,Y=-1.5 (should be at baseline 0?)
	* uni00B5 (U+00B5): X=323.0,Y=1.0 (should be at baseline 0?)
	* atilde (U+00E3): X=170.5,Y=701.0 (should be at cap-height 700?)
	* ntilde (U+00F1): X=201.5,Y=701.0 (should be at cap-height 700?) and 64 more. [code: found-misalignments]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do any segments have colinear vectors?</summary>

* [com.google.fonts/check/outline_colinear_vectors](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_colinear_vectors)
<pre>--- Rationale ---
This check looks for consecutive line segments which have the same angle. This
normally happens if an outline point has been added by accident.
This check is not run for variable fonts, as they may legitimately have colinear
vectors.</pre>

* ⚠ **WARN** The following glyphs have colinear vectors:
	* uni0524 (U+0524): L<<512.0,24.0>--<512.0,124.0>> -> L<<512.0,124.0>--<512.0,125.0>> [code: found-colinear-vectors]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do outlines contain any semi-vertical or semi-horizontal lines?</summary>

* [com.google.fonts/check/outline_semi_vertical](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_semi_vertical)
<pre>--- Rationale ---
This check detects line segments which are nearly, but not quite, exactly
horizontal or vertical. Sometimes such lines are created by design, but often
they are indicative of a design error.
This check is disabled for italic styles, which often contain nearly-upright
lines.</pre>

* ⚠ **WARN** The following glyphs have semi-vertical/semi-horizontal lines:
 * g (U+0067): L<<548.0,495.0>--<549.0,13.0>>
 * gbreve (U+011F): L<<548.0,495.0>--<549.0,13.0>>
 * gcircumflex (U+011D): L<<548.0,495.0>--<549.0,13.0>>
 * gdotaccent (U+0121): L<<548.0,495.0>--<549.0,13.0>>
 * uni0123 (U+0123): L<<548.0,495.0>--<549.0,13.0>>
 * uni0434 (U+0434): L<<208.0,106.0>--<403.0,107.0>>
 * uni05E9 (U+05E9): L<<182.0,547.0>--<184.0,284.0>>
 * uni05EA (U+05EA): L<<246.0,0.0>--<72.0,1.0>>
 * uniFB2A (U+FB2A): L<<182.0,547.0>--<184.0,284.0>>
 * uniFB2B (U+FB2B): L<<182.0,547.0>--<184.0,284.0>> and 4 more. [code: found-semi-vertical]

</details>
<br>
</details>
<details>
<summary><b>[11] Rubik-Italic.ttf</b></summary>
<details>
<summary>💔 <b>ERROR:</b> Check samples can be rendered.</summary>

* [com.google.fonts/check/metadata/can_render_samples](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/metadata/can_render_samples)
<pre>--- Rationale ---
In order to prevent tofu from being seen on fonts.google.com, this check
verifies that all samples provided on METADATA.pb can be properly rendered by
the font.</pre>

* 💔 **ERROR** Failed with AttributeError: 'NoneType' object has no attribute 'sample_glyphs'

</details>
<details>
<summary>🔥 <b>FAIL:</b> Check license file has good copyright string.</summary>

* [com.google.fonts/check/license/OFL_copyright](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/license/OFL_copyright)
<pre>--- Rationale ---
An OFL.txt file&#x27;s first line should be the font copyright e.g:
&quot;Copyright 2019 The Montserrat Project Authors
(https://github.com/julietaula/montserrat)&quot;</pre>

* 🔥 **FAIL** First line in license file does not match expected format: "copyright 20** the my font project authors (https://github.com/googlefonts/my-font-repository)"

</details>
<details>
<summary>⚠ <b>WARN:</b> Checking OS/2 achVendID.</summary>

* [com.google.fonts/check/vendor_id](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/vendor_id)
<pre>--- Rationale ---
Microsoft keeps a list of font vendors and their respective contact info. This
list is updated regularly and is indexed by a 4-char &quot;Vendor ID&quot; which is stored
in the achVendID field of the OS/2 table.
Registering your ID is not mandatory, but it is a good practice since some
applications may display the type designer / type foundry contact info on some
dialog and also because that info will be visible on Microsoft&#x27;s website:
https://docs.microsoft.com/en-us/typography/vendors/
This check verifies whether or not a given font&#x27;s vendor ID is registered in
that list or if it has some of the default values used by the most common font
editors.
Each new FontBakery release includes a cached copy of that list of vendor IDs.
If you registered recently, you&#x27;re safe to ignore warnings emitted by this
check, since your ID will soon be included in one of our upcoming releases.</pre>

* ⚠ **WARN** OS/2 VendorID value 'NONE' is not yet recognized. If you registered it recently, then it's safe to ignore this warning message. Otherwise, you should set it to your own unique 4 character code, and register it with Microsoft at https://www.microsoft.com/typography/links/vendorlist.aspx
 [code: unknown]

</details>
<details>
<summary>⚠ <b>WARN:</b> Font has old ttfautohint applied?</summary>

* [com.google.fonts/check/old_ttfautohint](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/old_ttfautohint)
<pre>--- Rationale ---
Check if font has been hinted with an outdated version of ttfautohint.</pre>

* ⚠ **WARN** ttfautohint used in font = 1.8.3; latest = 1.8.4; Need to re-run with the newer version! [code: old-ttfa]

</details>
<details>
<summary>⚠ <b>WARN:</b> Glyphs are similiar to Google Fonts version?</summary>

* [com.google.fonts/check/production_glyphs_similarity](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/production_glyphs_similarity)

* ⚠ **WARN** Following glyphs differ greatly from Google Fonts version: [A, AE, AEacute, Aacute, Abreve, Acircumflex, Adieresis, Agrave, Amacron, Aogonek, Aring, Atilde, B, C, Cacute, Ccaron, Ccedilla, Ccircumflex, Cdotaccent, D, Dcaron, Dcroat, E, Eacute, Ebreve, Ecaron, Ecircumflex, Edieresis, Edotaccent, Egrave, Emacron, Eng, Eogonek, Eth, Euro, Euro.BRACKET.125, F, G, Gbreve, Gcircumflex, Gdotaccent, H, Hbar, Hcircumflex, I, IJ, Iacute, Ibreve, Icircumflex, Idieresis, Idotaccent, Igrave, Imacron, Iogonek, Itilde, J, Jcircumflex, K, L, Lacute, Lcaron, Ldot, Lslash, M, N, Nacute, Ncaron, Ntilde, O, OE, Oacute, Obreve, Ocircumflex, Odieresis, Ograve, Ohungarumlaut, Omacron, Oslash, Oslashacute, Otilde, P, Q, R, Racute, Rcaron, S, Sacute, Scaron, Scedilla, Scircumflex, T, Tbar, Tcaron, Thorn, U, Uacute, Ubreve, Ucircumflex, Udieresis, Ugrave, Uhungarumlaut, Umacron, Uogonek, Uring, Ustraitcy, Ustraitstrokecy, Utilde, V, W, Wacute, Wcircumflex, Wdieresis, Wgrave, X, Y, Yacute, Ycircumflex, Ydieresis, Ygrave, Z, Zacute, Zcaron, Zdotaccent, a, aacute, abreve, acircumflex, adieresis, ae, aeacute, agrave, amacron, ampersand, aogonek, approxequal, approxequal.case, aring, asciitilde, asciitilde.case, asterisk, at, at.case, atilde, b, backslash, bar, braceleft, braceleft.case, braceright, braceright.case, bracketleft, bracketleft.case, bracketright, bracketright.case, brokenbar, c, cacute, ccaron, ccedilla, ccircumflex, cdotaccent, cent, colon, copyright, currency, d, dagger, daggerdbl, dcaron, dcroat, degree, divide, divide.case, dollar, dotlessi, e, eacute, ebreve, ecaron, ecircumflex, edieresis, edotaccent, egrave, eight, eight.dnom, eight.numr, eight.tf, ellipsis, emacron, emdash, emdash.case, endash, endash.case, eng, eogonek, equal, equal.case, estimated, eth, exclam, exclamdown, f, f_f, f_f_i, f_f_l, fi, five, five.dnom, five.numr, five.tf, fiveeighths, fl, florin, four, four.dnom, four.numr, four.tf, fraction, g, gbreve, gcircumflex, gdotaccent, germandbls, greater, greaterequal, guillemotleft, guillemotleft.case, guillemotright, guillemotright.case, guilsinglleft, guilsinglleft.case, guilsinglright, guilsinglright.case, h, hbar, hcircumflex, hyphen, hyphen.case, i, iacute, ibreve, icircumflex, idieresis, igrave, ij, imacron, infinity, integral, iogonek, itilde, j, jcircumflex, k, kgreenlandic, l, lacute, lcaron, ldot, less, lessequal, logicalnot, longs, lozenge, lslash, m, minus, minus.case, multiply, multiply.case, n, nacute, napostrophe, ncaron, nine, nine.dnom, nine.numr, nine.tf, notequal, notequal.case, ntilde, numbersign, o, oacute, obreve, ocircumflex, odieresis, oe, ograve, ohungarumlaut, omacron, one, one.tf, oneeighth, onehalf, onequarter, oslash, oslashacute, otilde, p, paragraph, parenleft, parenleft.case, parenleft.tf, parenright, parenright.case, parenright.tf, partialdiff, percent, perthousand, plus, plus.case, plusminus, product, q, question, questiondown, quotedbl, quotedblbase, quotedblleft, quotedblright, r, racute, radical, rcaron, registered, s, sacute, scaron, scedilla, scircumflex, section, semicolon, seven, seven.tf, seveneighths, six, six.tf, slash, sterling, summation, t, tbar, tcaron, thorn, three, three.dnom, three.numr, three.tf, threeeighths, threequarters, trademark, two, two.dnom, two.numr, two.tf, u, uacute, ubreve, ucircumflex, udieresis, ugrave, uhungarumlaut, umacron, underscore, uni004A0301, uni006A0301, uni00AD, uni00B2, uni00B3, uni00B5, uni0122, uni0123, uni0136, uni0137, uni013B, uni013C, uni0145, uni0146, uni0156, uni0157, uni0218, uni0219, uni021A, uni021B, uni0237, uni0400, uni0401, uni0402, uni0403, uni0404, uni0405, uni0406, uni0407, uni0408, uni0409, uni040A, uni040B, uni040C, uni040D, uni040E, uni040F, uni0410, uni0411, uni0412, uni0413, uni0414, uni0415, uni0416, uni0417, uni0418, uni0419, uni041A, uni041B, uni041C, uni041D, uni041E, uni041F, uni0420, uni0421, uni0422, uni0423, uni0424, uni0425, uni0426, uni0427, uni0428, uni0429, uni042A, uni042B, uni042C, uni042D, uni042E, uni042F, uni0430, uni0431, uni0432, uni0433, uni0434, uni0435, uni0436, uni0437, uni0438, uni0439, uni043A, uni043B, uni043C, uni043D, uni043E, uni043F, uni0440, uni0441, uni0442, uni0443, uni0444, uni0445, uni0446, uni0447, uni0448, uni0449, uni044A, uni044B, uni044C, uni044D, uni044E, uni044F, uni0450, uni0451, uni0452, uni0453, uni0454, uni0455, uni0456, uni0457, uni0458, uni0459, uni045A, uni045B, uni045C, uni045D, uni045E, uni045F, uni0462, uni0463, uni046A, uni046B, uni0472, uni0473, uni0474, uni0475, uni0490, uni0491, uni0492, uni0493, uni0494, uni0495, uni0496, uni0497, uni0498, uni0499, uni049A, uni049B, uni049C, uni049D, uni04A0, uni04A1, uni04A2, uni04A3, uni04A4, uni04A5, uni04AA, uni04AB, uni04B6, uni04B7, uni04B8, uni04B9, uni04BA, uni04BB, uni04C0, uni04C1, uni04C2, uni04CB, uni04CC, uni04CF, uni04D0, uni04D1, uni04D2, uni04D3, uni04D4, uni04D5, uni04D6, uni04D7, uni04D8, uni04D9, uni04DC, uni04DD, uni04DE, uni04DF, uni04E2, uni04E3, uni04E4, uni04E5, uni04E6, uni04E7, uni04E8, uni04E9, uni04EE, uni04EF, uni04F0, uni04F1, uni04F2, uni04F3, uni04F4, uni04F5, uni04F6, uni04F7, uni04F8, uni04F9, uni051A, uni051B, uni051C, uni051D, uni0524, uni0525, uni05B8, uni05D0, uni05D1, uni05D2, uni05D3, uni05D4, uni05D5, uni05D6, uni05D7, uni05D8, uni05D9, uni05DA, uni05DB, uni05DC, uni05DD, uni05DE, uni05DF, uni05E0, uni05E1, uni05E2, uni05E3, uni05E4, uni05E5, uni05E6, uni05E7, uni05E8, uni05E9, uni05EA, uni05F2, uni05F4, uni2070, uni2074, uni2075, uni2078, uni2079, uni2080, uni2082, uni2083, uni2084, uni2085, uni2088, uni2089, uni20AA, uni20AE, uni20B4, uni20B4.BRACKET.125, uni20B8, uni20B9, uni20BD, uni2116, uni2153, uni2154, uni2206, uni2215, uniFB2A, uniFB2B, uniFB2C, uniFB2D, uniFB2E, uniFB2F, uniFB30, uniFB31, uniFB32, uniFB33, uniFB34, uniFB35, uniFB36, uniFB38, uniFB39, uniFB3A, uniFB3B, uniFB3C, uniFB3E, uniFB40, uniFB41, uniFB43, uniFB44, uniFB46, uniFB47, uniFB48, uniFB49, uniFB4A, uniFB4B, uogonek, uring, ustraitcy, ustraitstrokecy, utilde, v, w, wacute, wcircumflex, wdieresis, wgrave, x, y, yacute, ycircumflex, ydieresis, yen, yen.BRACKET.125, ygrave, z, zacute, zcaron, zdotaccent, zero, zero.dnom, zero.numr, zero.tf, zero.tf.zero, zero.zero]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check if each glyph has the recommended amount of contours.</summary>

* [com.google.fonts/check/contour_count](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/contour_count)
<pre>--- Rationale ---
Visually QAing thousands of glyphs by hand is tiring. Most glyphs can only be
constructured in a handful of ways. This means a glyph&#x27;s contour count will only
differ slightly amongst different fonts, e.g a &#x27;g&#x27; could either be 2 or 3
contours, depending on whether its double story or single story.
However, a quotedbl should have 2 contours, unless the font belongs to a display
family.
This check currently does not cover variable fonts because there&#x27;s plenty of
alternative ways of constructing glyphs with multiple outlines for each feature
in a VarFont. The expected contour count data for this check is currently
optimized for the typical construction of glyphs in static fonts.</pre>

* ⚠ **WARN** This check inspects the glyph outlines and detects the total number of contours in each of them. The expected values are infered from the typical ammounts of contours observed in a large collection of reference font families. The divergences listed below may simply indicate a significantly different design on some of your glyphs. On the other hand, some of these may flag actual bugs in the font such as glyphs mapped to an incorrect codepoint. Please consider reviewing the design and codepoint assignment of these to make sure they are correct.

The following glyphs do not have the recommended number of contours:

Glyph name: ustraitstrokecy	Contours detected: 2	Expected: 1
Glyph name: fi	Contours detected: 1	Expected: 3
Glyph name: fl	Contours detected: 1	Expected: 2 [code: contour-count]

</details>
<details>
<summary>⚠ <b>WARN:</b> Is there kerning info for non-ligated sequences?</summary>

* [com.google.fonts/check/kerning_for_non_ligated_sequences](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/kerning_for_non_ligated_sequences)
<pre>--- Rationale ---
Fonts with ligatures should have kerning on the corresponding non-ligated
sequences for text where ligatures aren&#x27;t used (eg
https://github.com/impallari/Raleway/issues/14).</pre>

* ⚠ **WARN** GPOS table lacks kerning info for the following non-ligated sequences:
	- f + f
	- f + i
	- i + f
	- f + l
	- l + f
	- i + l

   [code: lacks-kern-info]

</details>
<details>
<summary>⚠ <b>WARN:</b> Ensure fonts have ScriptLangTags declared on the 'meta' table.</summary>

* [com.google.fonts/check/meta/script_lang_tags](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/meta/script_lang_tags)
<pre>--- Rationale ---
The OpenType &#x27;meta&#x27; table originated at Apple. Microsoft added it to OT with
just two DataMap records:
- dlng: comma-separated ScriptLangTags that indicate which scripts, or languages
and scripts, with possible variants, the font is designed for
- slng: comma-separated ScriptLangTags that indicate which scripts, or languages
and scripts, with possible variants, the font supports
The slng structure is intended to describe which languages and scripts the font
overall supports. For example, a Traditional Chinese font that also contains
Latin characters, can indicate Hant,Latn, showing that it supports Hant, the
Traditional Chinese variant of the Hani script, and it also supports the Latn
script
The dlng structure is far more interesting. A font may contain various glyphs,
but only a particular subset of the glyphs may be truly &quot;leading&quot; in the design,
while other glyphs may have been included for technical reasons. Such a
Traditional Chinese font could only list Hant there, showing that it’s designed
for Traditional Chinese, but the font would omit Latn, because the developers
don’t think the font is really recommended for purely Latin-script use.
The tags used in the structures can comprise just script, or also language and
script. For example, if a font has Bulgarian Cyrillic alternates in the locl
feature for the cyrl BGR OT languagesystem, it could also indicate in dlng
explicitly that it supports bul-Cyrl. (Note that the scripts and languages in
meta use the ISO language and script codes, not the OpenType ones).
This check ensures that the font has the meta table containing the slng and dlng
structures.
All families in the Google Fonts collection should contain the &#x27;meta&#x27; table.
Windows 10 already uses it when deciding on which fonts to fall back to. The
Google Fonts API and also other environments could use the data for smarter
filtering. Most importantly, those entries should be added to the Noto fonts.
In the font making process, some environments store this data in external files
already. But the meta table provides a convenient way to store this inside the
font file, so some tools may add the data, and unrelated tools may read this
data. This makes the solution much more portable and universal.</pre>

* ⚠ **WARN** This font file does not have a 'meta' table. [code: lacks-meta-table]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check font contains no unreachable glyphs</summary>

* [com.google.fonts/check/unreachable_glyphs](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/universal.html#com.google.fonts/check/unreachable_glyphs)
<pre>--- Rationale ---
Glyphs are either accessible directly through Unicode codepoints or through
substitution rules. Any glyphs not accessible by either of these means are
redundant and serve only to increase the font&#x27;s file size.</pre>

* ⚠ **WARN** The following glyphs could not be reached by codepoint or substitution rules:
 - Euro.BRACKET.125
 - parenright.denominator
 - .null
 - yen.BRACKET.125
 - parenleft.numerator
 - uni030C.alt
 - brevecombcy
 - parenleft.denominator
 - uni20B4.BRACKET.125 
 - parenright.numerator
 [code: unreachable-glyphs]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do any segments have colinear vectors?</summary>

* [com.google.fonts/check/outline_colinear_vectors](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_colinear_vectors)
<pre>--- Rationale ---
This check looks for consecutive line segments which have the same angle. This
normally happens if an outline point has been added by accident.
This check is not run for variable fonts, as they may legitimately have colinear
vectors.</pre>

* ⚠ **WARN** The following glyphs have colinear vectors:
	* uni04CB (U+04CB): L<<531.0,71.0>--<531.0,71.0>> -> L<<531.0,71.0>--<531.0,71.0>> and uni0524 (U+0524): L<<488.0,90.0>--<488.0,90.0>> -> L<<488.0,90.0>--<488.0,90.0>> [code: found-colinear-vectors]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do outlines contain any jaggy segments?</summary>

* [com.google.fonts/check/outline_jaggy_segments](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_jaggy_segments)
<pre>--- Rationale ---
This check heuristically detects outline segments which form a particularly
small angle, indicative of an outline error. This may cause false positives in
cases such as extreme ink traps, so should be regarded as advisory and backed up
by manual inspection.</pre>

* ⚠ **WARN** The following glyphs have jaggy segments:
	* uni0495 (U+0495): L<<202.0,440.0>--<163.0,254.0>>/L<<163.0,254.0>--<167.0,273.0>> = 0.04658192429955475 [code: found-jaggy-segments]

</details>
<br>
</details>
<details>
<summary><b>[12] Rubik-LightItalic.ttf</b></summary>
<details>
<summary>💔 <b>ERROR:</b> Check samples can be rendered.</summary>

* [com.google.fonts/check/metadata/can_render_samples](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/metadata/can_render_samples)
<pre>--- Rationale ---
In order to prevent tofu from being seen on fonts.google.com, this check
verifies that all samples provided on METADATA.pb can be properly rendered by
the font.</pre>

* 💔 **ERROR** Failed with AttributeError: 'NoneType' object has no attribute 'sample_glyphs'

</details>
<details>
<summary>🔥 <b>FAIL:</b> Check license file has good copyright string.</summary>

* [com.google.fonts/check/license/OFL_copyright](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/license/OFL_copyright)
<pre>--- Rationale ---
An OFL.txt file&#x27;s first line should be the font copyright e.g:
&quot;Copyright 2019 The Montserrat Project Authors
(https://github.com/julietaula/montserrat)&quot;</pre>

* 🔥 **FAIL** First line in license file does not match expected format: "copyright 20** the my font project authors (https://github.com/googlefonts/my-font-repository)"

</details>
<details>
<summary>⚠ <b>WARN:</b> Checking OS/2 achVendID.</summary>

* [com.google.fonts/check/vendor_id](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/vendor_id)
<pre>--- Rationale ---
Microsoft keeps a list of font vendors and their respective contact info. This
list is updated regularly and is indexed by a 4-char &quot;Vendor ID&quot; which is stored
in the achVendID field of the OS/2 table.
Registering your ID is not mandatory, but it is a good practice since some
applications may display the type designer / type foundry contact info on some
dialog and also because that info will be visible on Microsoft&#x27;s website:
https://docs.microsoft.com/en-us/typography/vendors/
This check verifies whether or not a given font&#x27;s vendor ID is registered in
that list or if it has some of the default values used by the most common font
editors.
Each new FontBakery release includes a cached copy of that list of vendor IDs.
If you registered recently, you&#x27;re safe to ignore warnings emitted by this
check, since your ID will soon be included in one of our upcoming releases.</pre>

* ⚠ **WARN** OS/2 VendorID value 'NONE' is not yet recognized. If you registered it recently, then it's safe to ignore this warning message. Otherwise, you should set it to your own unique 4 character code, and register it with Microsoft at https://www.microsoft.com/typography/links/vendorlist.aspx
 [code: unknown]

</details>
<details>
<summary>⚠ <b>WARN:</b> Font has old ttfautohint applied?</summary>

* [com.google.fonts/check/old_ttfautohint](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/old_ttfautohint)
<pre>--- Rationale ---
Check if font has been hinted with an outdated version of ttfautohint.</pre>

* ⚠ **WARN** ttfautohint used in font = 1.8.3; latest = 1.8.4; Need to re-run with the newer version! [code: old-ttfa]

</details>
<details>
<summary>⚠ <b>WARN:</b> Glyphs are similiar to Google Fonts version?</summary>

* [com.google.fonts/check/production_glyphs_similarity](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/production_glyphs_similarity)

* ⚠ **WARN** Following glyphs differ greatly from Google Fonts version: [Euro, Hbar, uni05B8, uni20AE, uni20B4, yen]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check if each glyph has the recommended amount of contours.</summary>

* [com.google.fonts/check/contour_count](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/contour_count)
<pre>--- Rationale ---
Visually QAing thousands of glyphs by hand is tiring. Most glyphs can only be
constructured in a handful of ways. This means a glyph&#x27;s contour count will only
differ slightly amongst different fonts, e.g a &#x27;g&#x27; could either be 2 or 3
contours, depending on whether its double story or single story.
However, a quotedbl should have 2 contours, unless the font belongs to a display
family.
This check currently does not cover variable fonts because there&#x27;s plenty of
alternative ways of constructing glyphs with multiple outlines for each feature
in a VarFont. The expected contour count data for this check is currently
optimized for the typical construction of glyphs in static fonts.</pre>

* ⚠ **WARN** This check inspects the glyph outlines and detects the total number of contours in each of them. The expected values are infered from the typical ammounts of contours observed in a large collection of reference font families. The divergences listed below may simply indicate a significantly different design on some of your glyphs. On the other hand, some of these may flag actual bugs in the font such as glyphs mapped to an incorrect codepoint. Please consider reviewing the design and codepoint assignment of these to make sure they are correct.

The following glyphs do not have the recommended number of contours:

Glyph name: ustraitstrokecy	Contours detected: 2	Expected: 1
Glyph name: fi	Contours detected: 1	Expected: 3
Glyph name: fl	Contours detected: 1	Expected: 2 [code: contour-count]

</details>
<details>
<summary>⚠ <b>WARN:</b> Is there kerning info for non-ligated sequences?</summary>

* [com.google.fonts/check/kerning_for_non_ligated_sequences](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/kerning_for_non_ligated_sequences)
<pre>--- Rationale ---
Fonts with ligatures should have kerning on the corresponding non-ligated
sequences for text where ligatures aren&#x27;t used (eg
https://github.com/impallari/Raleway/issues/14).</pre>

* ⚠ **WARN** GPOS table lacks kerning info for the following non-ligated sequences:
	- f + f
	- f + i
	- i + f
	- f + l
	- l + f
	- i + l

   [code: lacks-kern-info]

</details>
<details>
<summary>⚠ <b>WARN:</b> Ensure fonts have ScriptLangTags declared on the 'meta' table.</summary>

* [com.google.fonts/check/meta/script_lang_tags](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/meta/script_lang_tags)
<pre>--- Rationale ---
The OpenType &#x27;meta&#x27; table originated at Apple. Microsoft added it to OT with
just two DataMap records:
- dlng: comma-separated ScriptLangTags that indicate which scripts, or languages
and scripts, with possible variants, the font is designed for
- slng: comma-separated ScriptLangTags that indicate which scripts, or languages
and scripts, with possible variants, the font supports
The slng structure is intended to describe which languages and scripts the font
overall supports. For example, a Traditional Chinese font that also contains
Latin characters, can indicate Hant,Latn, showing that it supports Hant, the
Traditional Chinese variant of the Hani script, and it also supports the Latn
script
The dlng structure is far more interesting. A font may contain various glyphs,
but only a particular subset of the glyphs may be truly &quot;leading&quot; in the design,
while other glyphs may have been included for technical reasons. Such a
Traditional Chinese font could only list Hant there, showing that it’s designed
for Traditional Chinese, but the font would omit Latn, because the developers
don’t think the font is really recommended for purely Latin-script use.
The tags used in the structures can comprise just script, or also language and
script. For example, if a font has Bulgarian Cyrillic alternates in the locl
feature for the cyrl BGR OT languagesystem, it could also indicate in dlng
explicitly that it supports bul-Cyrl. (Note that the scripts and languages in
meta use the ISO language and script codes, not the OpenType ones).
This check ensures that the font has the meta table containing the slng and dlng
structures.
All families in the Google Fonts collection should contain the &#x27;meta&#x27; table.
Windows 10 already uses it when deciding on which fonts to fall back to. The
Google Fonts API and also other environments could use the data for smarter
filtering. Most importantly, those entries should be added to the Noto fonts.
In the font making process, some environments store this data in external files
already. But the meta table provides a convenient way to store this inside the
font file, so some tools may add the data, and unrelated tools may read this
data. This makes the solution much more portable and universal.</pre>

* ⚠ **WARN** This font file does not have a 'meta' table. [code: lacks-meta-table]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check font contains no unreachable glyphs</summary>

* [com.google.fonts/check/unreachable_glyphs](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/universal.html#com.google.fonts/check/unreachable_glyphs)
<pre>--- Rationale ---
Glyphs are either accessible directly through Unicode codepoints or through
substitution rules. Any glyphs not accessible by either of these means are
redundant and serve only to increase the font&#x27;s file size.</pre>

* ⚠ **WARN** The following glyphs could not be reached by codepoint or substitution rules:
 - Euro.BRACKET.125
 - parenright.denominator
 - .null
 - yen.BRACKET.125
 - parenleft.numerator
 - uni030C.alt
 - brevecombcy
 - parenleft.denominator
 - uni20B4.BRACKET.125 
 - parenright.numerator
 [code: unreachable-glyphs]

</details>
<details>
<summary>⚠ <b>WARN:</b> Are there any misaligned on-curve points?</summary>

* [com.google.fonts/check/outline_alignment_miss](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_alignment_miss)
<pre>--- Rationale ---
This check heuristically looks for on-curve points which are close to, but do
not sit on, significant boundary coordinates. For example, a point which has a
Y-coordinate of 1 or -1 might be a misplaced baseline point. As well as the
baseline, here we also check for points near the x-height (but only for lower
case Latin letters), cap-height, ascender and descender Y coordinates.
Not all such misaligned curve points are a mistake, and sometimes the design may
call for points in locations near the boundaries. As this check is liable to
generate significant numbers of false positives, it will pass if there are more
than 100 reported misalignments.</pre>

* ⚠ **WARN** The following glyphs have on-curve points which have potentially incorrect y coordinates:
	* parenleft (U+0028): X=288.0,Y=698.5 (should be at cap-height 700?)
	* parenright (U+0029): X=199.0,Y=698.0 (should be at cap-height 700?)
	* one (U+0031): X=342.0,Y=699.0 (should be at cap-height 700?)
	* at (U+0040): X=645.0,Y=-1.5 (should be at baseline 0?)
	* braceright (U+007D): X=296.5,Y=699.5 (should be at cap-height 700?)
	* questiondown (U+00BF): X=197.0,Y=-2.0 (should be at baseline 0?)
	* oslash (U+00F8): X=15.0,Y=1.0 (should be at baseline 0?)
	* ccaron (U+010D): X=232.0,Y=699.0 (should be at cap-height 700?)
	* eogonek (U+0119): X=164.0,Y=-2.0 (should be at baseline 0?)
	* ecaron (U+011B): X=246.0,Y=699.0 (should be at cap-height 700?) and 29 more. [code: found-misalignments]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do any segments have colinear vectors?</summary>

* [com.google.fonts/check/outline_colinear_vectors](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_colinear_vectors)
<pre>--- Rationale ---
This check looks for consecutive line segments which have the same angle. This
normally happens if an outline point has been added by accident.
This check is not run for variable fonts, as they may legitimately have colinear
vectors.</pre>

* ⚠ **WARN** The following glyphs have colinear vectors:
	* uni0524 (U+0524): L<<496.0,60.0>--<496.0,60.0>> -> L<<496.0,60.0>--<496.0,60.0>> [code: found-colinear-vectors]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do outlines contain any jaggy segments?</summary>

* [com.google.fonts/check/outline_jaggy_segments](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_jaggy_segments)
<pre>--- Rationale ---
This check heuristically detects outline segments which form a particularly
small angle, indicative of an outline error. This may cause false positives in
cases such as extreme ink traps, so should be regarded as advisory and backed up
by manual inspection.</pre>

* ⚠ **WARN** The following glyphs have jaggy segments:
	* uni0495 (U+0495): L<<185.0,462.0>--<139.0,242.0>>/L<<139.0,242.0>--<146.0,277.0>> = 0.4999504830075268 [code: found-jaggy-segments]

</details>
<br>
</details>

### Summary

| 💔 ERROR | 🔥 FAIL | ⚠ WARN | 💤 SKIP | ℹ INFO | 🍞 PASS | 🔎 DEBUG |
|:-----:|:----:|:----:|:----:|:----:|:----:|:----:|
| 14 | 14 | 136 | 1368 | 99 | 1227 | 0 |
| 0% | 0% | 5% | 48% | 3% | 43% | 0% |

**Note:** The following loglevels were omitted in this report:
* **SKIP**
* **INFO**
* **PASS**
* **DEBUG**