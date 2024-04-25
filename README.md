## flatpickr-twyear

<!-- [![npm version](https://badge.fury.io/js/flatpickr.svg)](https://www.npmjs.com/package/flatpickr) -->

[![License](https://img.shields.io/badge/license-MIT-blue.svg?style=plastic)](https://raw.githubusercontent.com/flatpickr/flatpickr/master/LICENSE.md)

![sample_en](https://github.com/cottongrass0828/flatpickr-twyear/assets/72060740/47f34d5f-5691-4e71-8a1f-3a48caed1194)
![sample_zh-tw](https://github.com/cottongrass0828/flatpickr-twyear/assets/72060740/f215ffeb-f5bc-4d93-a66e-a15969e45a3a)

## Motivation

a forked and modify from [Flatpickr](https://flatpickr.js.org/)

Feature Overview:

- Adds support for ROC (Republic of China) calendar
- Uses 't' as the format character for ROC dates, e.g., t-m-d

---

<zh-TW>

一個從 Flatpickr 進行修改的分支

功能概述：

- 增加對民國年的支援
- 使用 t 做為民國年的格式化字串, 如：t-m-d

</zh-TW>

## New Config Options

| Config Option | Type    | Default | Description                                                     |
| ------------- | ------- | ------- | --------------------------------------------------------------- |
| year_tw       | Boolean | false   | Displays ROC era name and change year to ROC Year when enabled. |

## New Date Formatting Tokens

| Character | Description                                 | Example   |
| --------- | ------------------------------------------- | --------- |
| t         | A full numeric representation of a ROC year | 88 or 113 |

## How to use

First Step:

```html
<link rel="stylesheet" href="./flatpickr.min.css" />
<script src="./flatpickr.min.js"></script>

<!-- optional -->
<script src="./l10n/zh_tw.js"></script>
```

Second Step:
Default Locale - ROC Calendar:

```javascript
var fp = flatpickr(".date", {
  year_tw: true,
  dateFormat: "t-m-d",
});
```

Traditional Chinese - ROC Calendar:

```javascript
var fp = flatpickr(".date", {
  locale: "zh_tw",
  year_tw: true,
  dateFormat: "t-m-d",
});
```

---

<zh-TW>
第一步: 
  
```html
  <link rel="stylesheet" href="./flatpickr.min.css">
  <script src="./flatpickr.min.js"></script>

  <!-- optional -->
  <script src="./l10n/zh_tw.js"></script>

````

第二步:
預設語系-民國年:
```javascript
var fp = flatpickr(".date", {
  year_tw: true,
  dateFormat: "t-m-d",
});
````

繁體中文-民國年:
```javascript
var fp = flatpickr(".date", {
  locale: "zh_tw",
  year_tw: true,
  dateFormat: "t-m-d",
});
```

</zh-TW>

---

# flatpickr - javascript datetime picker

## Compatibility

IE9 and up, Edge, iOS Safari 6+, Chrome 8+, Firefox 6+

## Install & Use

Demos and documentation: https://flatpickr.js.org

## Supporting flatpickr

flatpickr will never change its license, pester users for donations, or engage in other user-hostile behavior.

Nevertheless, if you enjoyed working with this library or if its made your life easier, you can buy me a cup of coffee :)

<a href='https://ko-fi.com/A3381DJ9' target='_blank'><img height='36' style='border:0px;height:36px;' src='https://az743702.vo.msecnd.net/cdn/kofi4.png?v=0' border='0' alt='Buy Me a Coffee at ko-fi.com' /></a>
