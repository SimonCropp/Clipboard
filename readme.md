<!--
GENERATED FILE - DO NOT EDIT
This file was generated by [MarkdownSnippets](https://github.com/SimonCropp/MarkdownSnippets).
Source File: /readme.source.md
To change this file edit the source file and then run MarkdownSnippets.
-->

# <img src="/src/icon.png" height="30px"> TextCopy

[![Build status](https://ci.appveyor.com/api/projects/status/axnys9xch290ut79/branch/master?svg=true)](https://ci.appveyor.com/project/SimonCropp/textcopy)
[![Build status](https://travis-ci.org/SimonCropp/TextCopy.svg?branch=master)](https://travis-ci.org/SimonCropp/TextCopy)
[![NuGet Status](https://img.shields.io/nuget/v/TextCopy.svg)](https://www.nuget.org/packages/TextCopy/)

A cross platform package to copy text to and from the clipboard.

Support is available via a [Tidelift Subscription](https://tidelift.com/subscription/pkg/nuget-textcopy?utm_source=nuget-textcopy&utm_medium=referral&utm_campaign=enterprise).

<!-- toc -->
## Contents

  * [Usage](#usage)
    * [SetTextAsync](#settextasync)
    * [SetText](#settext)
    * [GetTextAsync](#gettextasync)
    * [GetText](#gettext)
  * [Instance API](#instance-api)
  * [Supported on](#supported-on)
  * [Notes on Linux](#notes-on-linux)
  * [Security contact information](#security-contact-information)<!-- endtoc -->


## NuGet package

https://nuget.org/packages/TextCopy/


## Usage


### SetTextAsync

<!-- snippet: SetTextAsync -->
<a id='snippet-settextasync'/></a>
```cs
await ClipboardService.SetTextAsync("Text to place in clipboard");
```
<sup><a href='/src/Tests/Snippets.cs#L35-L39' title='File snippet `settextasync` was extracted from'>snippet source</a> | <a href='#snippet-settextasync' title='Navigate to start of snippet `settextasync`'>anchor</a></sup>
<!-- endsnippet -->


### SetText

<!-- snippet: SetText -->
<a id='snippet-settext'/></a>
```cs
ClipboardService.SetText("Text to place in clipboard");
```
<sup><a href='/src/Tests/Snippets.cs#L10-L14' title='File snippet `settext` was extracted from'>snippet source</a> | <a href='#snippet-settext' title='Navigate to start of snippet `settext`'>anchor</a></sup>
<!-- endsnippet -->


### GetTextAsync

<!-- snippet: GetTextAsync -->
<a id='snippet-gettextasync'/></a>
```cs
var text = await ClipboardService.GetTextAsync();
```
<sup><a href='/src/Tests/Snippets.cs#L44-L48' title='File snippet `gettextasync` was extracted from'>snippet source</a> | <a href='#snippet-gettextasync' title='Navigate to start of snippet `gettextasync`'>anchor</a></sup>
<!-- endsnippet -->


### GetText

<!-- snippet: GetText -->
<a id='snippet-gettext'/></a>
```cs
var text = ClipboardService.GetText();
```
<sup><a href='/src/Tests/Snippets.cs#L26-L30' title='File snippet `gettext` was extracted from'>snippet source</a> | <a href='#snippet-gettext' title='Navigate to start of snippet `gettext`'>anchor</a></sup>
<!-- endsnippet -->


## Instance API

In adition to the above static API, there is an instance API exposed:

<!-- snippet: SetTextInstance -->
<a id='snippet-settextinstance'/></a>
```cs
var clipboard = new Clipboard();
clipboard.SetText("Text to place in clipboard");
```
<sup><a href='/src/Tests/Snippets.cs#L16-L21' title='File snippet `settextinstance` was extracted from'>snippet source</a> | <a href='#snippet-settextinstance' title='Navigate to start of snippet `settextinstance`'>anchor</a></sup>
<!-- endsnippet -->


## Supported on

 * Windows with .NET Framework 4.6.1 and up
 * Windows with .NET Core 2.0 and up
 * Windows with Mono 5.0 and up
 * OSX with .NET Core 2.0 and up
 * OSX with Mono 5.20.1 and up
 * Linux with .NET Core 2.0 and up
 * Linux with Mono 5.20.1 and up
 * Xamarin.Android 9.0 and up
 * Xamarin.iOS 10.0 and up
 * Universal Windows Platform version 10.0.16299 and up


## Notes on Linux

Linux uses [xclip](https://github.com/astrand/xclip) to access the clipboard. As such it needs to be installed and callable.


## Security contact information

To report a security vulnerability, use the [Tidelift security contact](https://tidelift.com/security). Tidelift will coordinate the fix and disclosure.


## Icon

[Clone](https://thenounproject.com/term/Clone/207435/) designed by [Wes Breazell](https://thenounproject.com/wes13/) from [The Noun Project](https://thenounproject.com).
