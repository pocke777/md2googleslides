---

# :innocent:  React Native :innocent:
## ファイ部 BKB

---

# アジェンダ

* React Native is...
* 開発フロー
* 実践

---

# Introduction
## [Learn once, write anywhere](https://facebook.github.io/react-native/)

---

![](https://i.gyazo.com/5a8fbcc12b665a97021b80b84013b5b2.png){.background}
# [react-native-macos](https://github.com/ptmt/react-native-macos)

---

![](https://i.gyazo.com/f25ef78d0bcd6ffdaf4166aa43df09b9.png){.background}
# [react-native-windows](https://github.com/Microsoft/react-native-windows)

---

# :innocent: React Native is

* WEB開発のスキルセットでネイティブアプリ開発に乗り込める(たまにネイティブ特有の問題にはぶつかる)
* NPMのエコシステムに乗っかれる(標準APIの制限はあり)
* Native UI (ハイパフォーマンス)
* 開発サポートが嬉しい

[Polyfills](https://facebook.github.io/react-native/docs/javascript-environment.html)

---

# アーキテクチャ

---

# :innocent:
## JS → Bridge → Native UI

![](https://i.gyazo.com/db166ee7e942aec639dd76162f504577.png)
[https://www.ibm.com/developerworks/jp/mobile/library/mo-bluemix-react-native-ios8/](https://www.ibm.com/developerworks/jp/mobile/library/mo-bluemix-react-native-ios8/)

---
# Data Flow

![](https://i.gyazo.com/20be933885d5c2bc85deed7350550fbe.png)
[https://speakerdeck.com/frantic/react-native-under-the-hood](https://speakerdeck.com/frantic/react-native-under-the-hood)

---
# Data Flow

![](https://i.gyazo.com/9db59f2571eef648cc4ee8514fd48b40.png)
[https://speakerdeck.com/frantic/react-native-under-the-hood](https://speakerdeck.com/frantic/react-native-under-the-hood)

---

# Other Cross Platform

Frame Work | Type
-------|--------
React Native | Native
NativeScript | Native
PhoneGap     | WebView
Ruby Motion  | Native

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

---

#:innocent: 実践 :innocent:

---

# App

このアプリを参考に実装

[https://github.com/naoya/HBFav2](https://github.com/naoya/HBFav2)

---

---
