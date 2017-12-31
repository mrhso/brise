<meta charset="UTF-8">

La brise
===
Rime schema repository

Project home
---
[rime.github.io](http://rime.github.io)

License
---
GPLv3

Contents
===
This software package contains a collection of configuration and data files
used by [Rime](http://rime.github.io) to support popular Chinese input methods.

A Rime input schema, which defines a specific input method in Rime's DSL,
consists of a schema file named `*.schema.yaml` where `*` is the schema ID,
and optionally an affiliated Rime dictionary file `*.dict.yaml`.
In the following lists of Rime schemata, only schema IDs are listed for brevity.

General
---
  - [`prelude`](https://github.com/rime/rime-prelude): the prelude package, providing Rime's default settings
  - [`essay`](https://github.com/rime/rime-essay): 八股文 / a shared vocabulary and language model

Preset schemata
---

Input methods that are fundamental, or prevalent in a region.

  - [`bopomofo`](https://github.com/rime/rime-bopomofo): 注音 / Zhuyin (aka. Bopomofo)
  - [`cangjie`](https://github.com/rime/rime-cangjie): 倉頡輸入法 / Cangjie input method
  - [`luna-pinyin`](https://github.com/rime/rime-luna-pinyin): 朙月拼音 / Pinyin in Tranditional Chinese
  - [`stroke`](https://github.com/rime/rime-stroke): 五筆畫 / five strokes
  - [`terra-pinyin`](https://github.com/rime/rime-terra-pinyin): 地球拼音 / School-taught Pinyin, with tone marks

Supplemental schemata
---

Including input methods that are widely used and those who implement major
modern dialects or historical diasystems. Less popular input methods with
small dictionaries or without independent dictionaries are also included.

  - [`combo-pinyin`](https://github.com/rime/rime-combo-pinyin): 宮保拼音 / Chord-typing Pinyin
  - [`double-pinyin`](https://github.com/rime/rime-double-pinyin): 雙拼 / Double Pinyin (ZiRanMa, ABC, flyPY, MSPY, PYJJ variants)
  - [`emoji`](https://github.com/rime/rime-emoji): 繪文字 / input emoji with English or Chinese Pinyin keywords
  - [`ipa`](https://github.com/rime/rime-ipa): 國際音標 / International Phonetic Alphabet
  - [`jyutping`](https://github.com/rime/rime-jyutping): 粵拼 / Cantonese
  - [`pinyin-simp`](https://github.com/rime/rime-pinyin-simp): 袖珍簡化字拼音 / Pinyin in Simplified Chinese
  - [`quick`](https://github.com/rime/rime-quick): 速成 / Simplified Cangjie
  - [`middle-chinese`](https://github.com/rime/rime-middle-chinese): 中古漢語拼音 / Middle Chinese Romanization
  - [`wubi`](https://github.com/rime/rime-wubi): 五筆字型
  - [`wugniu`](https://github.com/rime/rime-wugniu): 上海吳語 / Wu (Shanghainese)

Extra schemata
---

Established input methods used by a minority, and evolving new inventions,
are included in the source package but are not to be installed by default.

  - [`array`](https://github.com/rime/rime-array): 行列輸入法
  - [`scj`](https://github.com/rime/rime-scj): 快速倉頡
  - [`soutzoe`](https://github.com/rime/rime-soutzoe): 蘇州吳語 / Wu (Suzhounese)
  - [`stenotype`](https://github.com/rime/rime-stenotype): 打字速記法 / a stenographic system derived from ABC Easy Shorthand

Pull requests are welcome for anything notable that hasn't been included here,
but you'll be responsible for providing data files along with an open-source
license because licensing will be rigidly scrutinized by downstream packagers.

OpenCC configurations
---

[OpenCC](https://github.com/BYVoid/OpenCC) is used by many of the above input
methods for conversion to Simplified/Traditional Chinese or other variant forms.
As of OpenCC 1.0.2, some of the configurations used by brise are missing.
We provide those configuration files under `opencc/` as a backup, until they
become widely available via future versions of downstream OpenCC packages.

Install
===

Build dependencies
---
  - librime>=1.3 (for rime_deployer)

Runtime dependencies
---
  - librime>=1.3
  - opencc>=1.0.2

Build and install
---
```
make
sudo make install
```

Credits
===
We are grateful to the makers of the following open source projects:

  - [Android Pinyin IME](https://source.android.com/) (Apache 2.0)
  - [Chewing / 新酷音](http://chewing.im/) (GPL)
  - [ibus-table](https://github.com/acevery/ibus-table) (LGPL)
  - [OpenCC / 開放中文轉換](https://github.com/BYVoid/OpenCC) (Apache 2.0)
  - [moedict / 萌典](https://www.moedict.tw) (CC0 1.0)
  - [Rime 翰林院 / Rime Academy](https://github.com/rime-aca) (GPLv3)

Also to the inventors of the following Chinese input methods:

  - Cangjie / 倉頡輸入法 by 朱邦復
  - Array input method / 行列輸入法 by 廖明德
  - Wubi / 五筆字型 by 王永民
  - Scj / 快速倉頡 by 麥志洪
  - Middle Chinese Romanization / 中古漢語拼音 by 古韻

Contributors
===
I may have missed someone.
See the `AUTHORS` file for a more complete list of authors and their works.

  - [佛振](https://github.com/lotem)
  - [瑾昀](https://github.com/kunki)
  - [雪齋](https://github.com/LEOYoon-Tsaw)
  - [Patrick Tschang](https://github.com/Patricivs)
  - [Joseph J.C. Tang](https://github.com/jinntrance)
  - [lxk](http://101reset.com)
  - [Ye Zhou](https://github.com/zhouye)
  - Jiehong Ma
  - StarSasumi
  - 古韻
  - 寒寒豆
  - 四季的風
  - 上海閒話abc
  - 吳語越音
