# Ansi 
[![Status](https://travis-ci.org/MikeManzo/Ansi.svg?branch=master)](https://travis-ci.org/MikeManzo/Ansi)
![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/mikemanzo/Ansi.svg)
![GitHub last commit](https://img.shields.io/github/last-commit/MikeManzo/Ansi.svg)
![Cocoapods platforms](https://img.shields.io/cocoapods/p/Ansi.svg)
![Swift](https://img.shields.io/badge/%20in-swift%204.2-orange.svg)

Ansi parser forked from [oleander](https://github.com/oleander/Ansi) updated for Swift 4.2 that constructs `NSAttributedString`s for ANSI-escaped text.

Currently only supports 8 & 256 bit colors, italic, strikethrough, underline and bold text.

## Usage

```swift
import Ansi

let attr = "ABC\\e[3;4;33mDEF\\e[0mGHI".ansified()
attr // => "ABC" + "DEF".italic.underline.yellow + "GHI"
attr.string // => "ABCDEF GHI"
```

## Install

Add `pod 'Ansi'` to your `Podfile` and run `pod install`.
