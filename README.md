# Ansi [![Status](https://travis-ci.org/oleander/Ansi.svg?branch=master)](https://travis-ci.org/oleander/Ansi)

[![Version](https://img.shields.io/cocoapods/v/Hue.svg?style=flat)](http://cocoadocs.org/docsets/Ansi)
[![License](https://img.shields.io/cocoapods/l/Hue.svg?style=flat)](http://cocoadocs.org/docsets/Ansi)
[![Platform](https://img.shields.io/cocoapods/p/Hue.svg?style=flat)](http://cocoadocs.org/docsets/Ansi)
![Swift](https://img.shields.io/badge/%20in-swift%204.0-orange.svg)

Ansi parser written in Swift 3 (and now updated for Swift 4.2) for constructing `NSAttributedString`s. Currently supports 8 & 256 bit colors, italic, strikethrough, underline and bold text.

## Usage

```swift
import Ansi

let attr = "ABC\\e[3;4;33mDEF\\e[0mGHI".ansified()
attr // => "ABC" + "DEF".italic.underline.yellow + "GHI"
attr.string // => "ABCDEF GHI"
```

## Install

Add `pod 'Ansi'` to your `Podfile` and run `pod install`.
