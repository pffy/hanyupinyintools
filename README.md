# HanyuPinyinTools

  + Hanyu Pinyin custom functions for Google Sheets
  + This is **Version 81.**


# INSTALL

> **NOTE:** Each method only affects one spreadsheet. 

### Method 1: Copy-paste `code.gs`

The source files in the `src` folder of this repo are automatically combined into a single Google Apps Script file using a GitHub workflow. The outfile has been saved to the `dist` folder as `code.gs`.

1. Open the `dist` folder.
2. Copy and paste the contents of the `code.gs` file to your Google Apps Script project file.
3. Save the project.
4. Return to your spreadsheet and start typing HanyuPinyinTools custom functions.


### Method 2: Make a copy.

1. **[Make of copy][copy]** of HanyuPinyinTools.

    + You can preview the Apps Script file.
    + You get your own personal copy of HanyuPinyinTools.
    + Distributed, decentralized copies prevent updates from breaking your spreadsheet.


# FUNCTIONS

### `=HANYUPINYIN(text)`

Converts Chinese characters to Hanyu Pinyin with tone numbers.

```visualbasic
// ni3 hao3
=HANYUPINYIN("你好")
```


### `=HANYUPINYIN_TONEMARKS(text)`

Converts Chinese characters to Hanyu Pinyin with backwards-compatible tone marks. The third tone is often represented by a [breve diacritic][wiki_breve]. This diacritic looks like the bottom half of a circle.

```visualbasic
// nĭ hăo
=HANYUPINYIN_TONEMARKS("你好")
```


### `=HANYUPINYIN_TONEMARKS_ISO(text)`

Converts Chinese characters to Hanyu Pinyin with [ISO-compliant][wiki_iso] tone marks. The third tone is always represented by a [caron diacritic][wiki_caron] (or haček). This diacritic looks like an inverted chevron.

```visualbasic
// nǐ hǎo
=HANYUPINYIN_TONEMARKS_ISO("你好")
```

### `=HANYUPINYIN_TONELESS(text)`

Converts Chinese characters to Hanyu Pinyin with ISO compliant tone marks.

```visualbasic
// ni hao
=HANYUPINYIN_TONELESS("你好")
```

# USES

A partial list of interesting uses

+ https://blogs.bodleian.ox.ac.uk/digital/2018/02/12/a-reconciliation-recipe-for-wikidata/
+ https://kaeritai.asia/archives/382


# LICENSE
  + MIT License
  + Impelements `concat-gs-files` workflow avaialble under the Unlicense license here:
    + https://github.com/pffy/code-gs
  

[wiki_breve]: https://en.wikipedia.org/wiki/Breve
[wiki_caron]: https://en.wikipedia.org/wiki/Caron
[wiki_iso]: https://www.iso.org/standard/61420.html
[copy]: https://docs.google.com/spreadsheets/d/1Uqm3gbPf3DSn314dCT75ZRsDrbkeMB0wRuuQM5ssXdY/copy
[dist]: https://github.com/pffy/hanyupinyintools/tree/main/dist
