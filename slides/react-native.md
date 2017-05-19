---

#  React Native Tour
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
# [macos](https://github.com/ptmt/react-native-macos)

---

![](https://i.gyazo.com/f25ef78d0bcd6ffdaf4166aa43df09b9.png){.background}
# [windows](https://github.com/Microsoft/react-native-windows)

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

# JSX

React | React Native
-------|--------
\<div> |  \<View>
\<span> | \<Text>
\<img> |  \<Image>

---

#:innocent: React JS

```
import React from 'react';
import ReactDom from 'react-dom';

class App extends React.Component {
  render() {
    return(
      <div>
        <Header />
        <Main />
        <Footer />
      </div>
    )
  }
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
  render() {
    return(
      <View>
        <Header />
        <Main />
        <Footer />
      </View>
    )
  }
}

AppRegistry.registerComponent(
  'Jugemu', ()=> App
);
```

---

#:innocent: React Native

![](https://i.gyazo.com/53732671566fafdcb58978cb2f76c044.png)

---

#:innocent:

## Reactはノードツリーの差分計算を行っているライブラリでレンダリング先がウェブであろうとアプリであろうとお構いなし

----
#:innocent:

## Reactによってコンポーネントを定義→ReactDomでブラウザへ書き込み →ネイティブUIへの書き込み → ReactNativeへ

---

# :innocent: 開発フロー

---

# Getting Started
```sh
# Installing Dependencies

brew install node
brew install watchman

npm install -g react-native-cli

# 起動
react-native run-ios
```

---

# Develop
![](https://i.gyazo.com/8c022d2cf9b35b484d90566ca5613f4e.png)

---

# Develop
![](https://i.gyazo.com/b4553bebca55d4fb68c0666fc9e690f6.png)

---

# Develop
![](https://i.gyazo.com/670ab846562bdfe145990e968969d74a.png)

---

# Develop
![](https://i.gyazo.com/240d8ff1878e20c6e1f54647506b6e37.png)

---

# いいね!いいねー！

---

#:innocent: 実践 :innocent:

---

# 参考実装

![](https://i.gyazo.com/e2e8a22eb42d69c3a64467cbaee67ac8.png)
[https://github.com/naoya/HBFav2](https://github.com/naoya/HBFav2)

---

# 各レイヤのポイント
レイヤ  | ポイント
-------|--------
ドメイン   | Viewと疎結合な部分はほとんどWebアプリと共通化が可能。Fluxアーキテクチャの利用もOK
View       | ReactNativeの提供するComponentを利用/Styleはサポートされている[プロパティ](https://github.com/vhpoet/react-native-styling-cheat-sheet)で実装
Navigation | Routerを使用して実装

---

# DEMO

---
