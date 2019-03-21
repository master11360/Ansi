# Ansi 
[![Status](https://travis-ci.org/MikeManzo/Ansi.svg?branch=master)](https://travis-ci.org/MikeManzo/Ansi)
![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/mikemanzo/Ansi.svg)
![GitHub last commit](https://img.shields.io/github/last-commit/MikeManzo/Ansi.svg)
![Cocoapods platforms](https://img.shields.io/cocoapods/p/Ansi.svg)
![GitHub All Releases](https://img.shields.io/github/downloads/MikeManzo/Ansi/total.svg)
![Swift](https://img.shields.io/badge/%20in-swift%204.2-orange.svg)

An ANSI parser forked from [Linus Oleander](https://github.com/oleander/Ansi) that has been updated for Swift 4.2.  You can use it two ways: You can read an escaped string and "ansifiy" it as an 'NSAttributedString', or you can take a standard string and output an ANSI escaped string suitable for a terminal or console.

# Support 
Currently ANSI supports 8 & 256 bit colors, italic, strikethrough, underline and bold text.

## Usage

```swift
import Ansi

let attr = "ABC\\e[3;4;33mDEF\\e[0mGHI".ansified()
attr // => "ABC" + "DEF".italic.underline.yellow + "GHI"
attr.string // => "ABCDEF GHI"
```

## Install

Add `pod 'Ansi'` to your `Podfile` and run `pod install`.
