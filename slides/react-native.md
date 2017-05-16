---

# :innocent:  React Native :innocent:
## ファイ部 BKB

---

# アジェンダ

* Introduction
* クロスプラットフォームの比較
* ReactとReact Native
* 開発フロー
* 実践

---

# :innocent: React Native is

# [Learn once, write anywhere](https://facebook.github.io/react-native/)

---

# :innocent:

* JavaScript と Reactでアプリをビルド
* Nativeで作動
* コンポーネント指向
* CSSっぽい Style Layout
* Objective-C, Swift, Javaなどのネイティブコードのインポート可能
* Nodeのエコシステム(ReactNativeがサポートしている標準APIしか使っていない場合は)
* 嬉しい開発サポート

<span style="color:red"> TODO: もっと増やす  </span>

---

# Nativeで作動?

---

# アーキテクチャ

![](https://scontent-nrt1-1.xx.fbcdn.net/v/t31.0-0/p600x600/18451640_1320297154720899_4206600920678887957_o.jpg?oh=d3748a85ccc193ed39560acca53fd8e0&oe=59BA49BD)

[http://www.reactnative.com/under-the-hood-of-react-native/](http://www.reactnative.com/under-the-hood-of-react-native/)

<!--
React NativeはJavaScriptCoreのランタイム上で動きNativeのAPIを動かす
Ruby Motionもランタイム上で動作しNativeのAPIを呼び出すが、RubyコードはLLVMによってバイトコードへとコンパイルされている
-->
---

#:innocent: クロスプラットフォームの比較

Frame Work | アーキテクチャ
-------|--------
React Native   | Native
NativeScript | Native
PhoneGap   | WebView
Ruby Motion | Native

---

# :innocent: ReactJSとReact Native :innocent:

---

#:innocent: React JS

```
import React from 'react';
import ReactDom    from 'react-dom';

class App extends React.Component {
  <div>
    <Header />
    <Main />
    <Footer />
  </div>
}

ReactDom.render(
  <App />,
  document.getElementById('app')
);

```

---

#:innocent: React JS

![](https://scontent.xx.fbcdn.net/v/t1.0-9/18403706_1320092604741354_8936771333364028686_n.jpg?oh=dc2404c65f303cbd43633c59f6464998&oe=59B8EFBB)

---

#:innocent: React Native

```
import React, { Component } from 'react';
import { AppRegistry } from 'react-native';

class App extends React.Component {
  <div>
    <Header />
    <Main />
    <Footer />
  </div>
}

AppRegistry.registerComponent(
  'Jugemu', ()=> App
);
```

---

#:innocent: React Native

JavaScript → ReactNative → iOS UI / Android UI
![](https://scontent.xx.fbcdn.net/v/t1.0-9/18527664_1320098144740800_5720499259349225849_n.jpg?oh=b7aa9eaa4557f0e3db1475dc4a975429&oe=59B39E80)

---

# :innocent: 開発フロー

---

# Getting Started

```
# Installing Dependencies

brew install node
brew install watchman

npm install -g react-native-cli

# 起動
react-native run-ios
```

---

# Develop
![](https://scontent.xx.fbcdn.net/v/t31.0-8/18489479_1320135324737082_7896970863086498350_o.jpg?oh=525fabc6a8877647cb7f71d974a2bb8b&oe=59764BE2)

---

# いいね!いいねー！

---

標準ライブラリ WEB APIもネイティブに再実装されている!!ワーイ!!

[Polyfills](https://facebook.github.io/react-native/docs/javascript-environment.html)

---

#:innocent: 実践 :innocent:

---

# App

このアプリを参考に実装

[https://github.com/naoya/HBFav2](https://github.com/naoya/HBFav2)

---

---
