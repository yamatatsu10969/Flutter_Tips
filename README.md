# Flutter_Tips

## Option + Enter をとりあえず押してみるの大事。
- method 作成
- widget 作成
- remove もできる
- コンストラクタの作成
- import もできる
- なんでもできそう。

## コンストラクター作れる
setter, getter を作成可能
コードの画面で、 cmd + n で generate constractor みたいなやつある

## 設定
<img width="1030" alt="Screen_Shot_2020-03-24_at_13_48_14" src="https://user-images.githubusercontent.com/43805056/77389367-57b30380-6dd6-11ea-9bb1-20b8ee1737a9.png">

# UI
- Placeholder 使うと一時的に置けるのでいいな

- 親の widget のサイズを知りたい時
  - LayoutBuilder を使う
  - [dart - How can I layout widgets based on the size of the parent? - Stack Overflow](https://stackoverflow.com/questions/41558368/how-can-i-layout-widgets-based-on-the-size-of-the-parent)


# Widget
- Widget のサイズが大きすぎて、キーボードが出てきた時に使える
  - SingleChildScrollView 
  - Flexible
  

- Dialog
  - 
  
  
## Text
- TextField 
  - デコるために使うのは、 InputDecoration
    - hintText, errorText など使える
  - border はコンストラクターでしか指定できない。noneはできる。
  - focusNode で、次の field を指定できる
  - .done + onEditingComplete でメソッド呼べる
  - controller で、文字を管理できる。clear など。
  
- Forms + TextFormField 
  - Global Key を設定しておけば、アクションをした時に一斉にvalidator をかけることができる
  - [Flutter & Firebase: Build a Complete App for iOS & Android | Udemy](https://www.udemy.com/course/flutter-firebase-build-a-complete-app-for-ios-android/learn/lecture/15441738#overview)
  
- TextField + TextEditingController 
  - 文字を入力するたびにバリデーションや、onChange を走らせることができる


# Navigator
- id 管理良いかも 
- Navigator.of(context, rootNavigator: true).push でタブバー消える

# BottomNavigation
- [Flutter Case Study: Multiple Navigators with BottomNavigationBar](https://medium.com/coding-with-flutter/flutter-case-study-multiple-navigators-with-bottomnavigationbar-90eb6caa6dbf)

# Date
- [Dart/Flutter での多言語対応あれこれ - Flutter 🇯🇵 - Medium](https://medium.com/flutter-jp/intl-beb5b9e8ee73)

# Error
- map 使っている時に、toList がつけずに型が合わないことがある。
- Coupertino と Materialは一緒に使わない方がいい時がある。→ tabbar と floatingActionButton など。


# Exception
- parse → tryParse
- on PlatformException が便利
  - on PlatformException catch(e) → e.message でエラーが出るので！工数下げるためにこれでOKでは。
- Exception Handler 
  - [Flutter & Firebase: Build a Complete App for iOS & Android | Udemy](https://www.udemy.com/course/flutter-firebase-build-a-complete-app-for-ios-android/learn/lecture/15309790#overview)
  - print して、出てくるメッセージを使って handler を作成する

# Debug
  - [Flutter & Firebase: Build a Complete App for iOS & Android | Udemy](https://www.udemy.com/course/flutter-firebase-build-a-complete-app-for-ios-android/learn/lecture/15309804#overview)
    - error で返ってくるデータに合わせて、exceptionを作成する
  - 虫さんを押して、ホットリロード
  - コンソールで Variables を確認できる
  - 

# StateManagement
- [Flutter & Firebase: Build a Complete App for iOS & Android | Udemy](https://www.udemy.com/course/flutter-firebase-build-a-complete-app-for-ios-android/learn/lecture/15789070#overview)


# Architecture
- BLoC
  - 結構複雑になっちゃう
- Provider 
  - これだけで良さそう
[Flutter Provider: Introduction - YouTube](https://www.youtube.com/watch?v=O71rYKcxUgA)

- ChangeNotifier だけでも良さそう

# ShortCut
[Flutter — IDE Shortcuts for Faster Development - Flutter Community - Medium](https://medium.com/flutter-community/flutter-ide-shortcuts-for-faster-development-2ef45c51085b)


# Flutter LoadMap for Mr.Pawan

[「Learn Flutter Like A PRO By Building Apps ( Absolutely Free &amp; No Time Waste ) - My 2 Years of hard work to make this content. For the correct order to learn. Here is the Full Thread 👇🏻 Retweet for awareness. Flutter @mtechviral #Flutter https://t.co/zgsbClf2eN」 / Twitter](https://twitter.com/imthepk/status/1213003226070437891)



# Dart Cheat Sheet

![Image from iOS](https://user-images.githubusercontent.com/43805056/83322294-56e49500-a291-11ea-987f-e0a7675c9b10.jpg)

# HTTP 系
- chopper
  - [Chopper (Retrofit for Flutter) - #1 Basics - Dart HTTP Client Generator Tutorial - YouTube](https://www.youtube.com/watch?v=zFXK5EsrUF0)
  - [ResoCoder/flutter-chopper-tutorial-course](https://github.com/ResoCoder/flutter-chopper-tutorial-course)
- http
  
## HTTP 系を試す時
無料で API 接続ができて、レスポンスが返ってくる。練習に最適
[JSONPlaceholder - Fake online REST API for developers](https://jsonplaceholder.typicode.com/)

## 動画を試す時
- [Test your streaming URL - Radiant Media Player](https://www.radiantmediaplayer.com/test-your-streaming-url.html) // こっちがいい。
  - [public test videos](https://gist.github.com/jsturgis/3b19447b304616f18657) // これは HTTP から動画を取得するから使えなかった orz
- 動画のパッケージは chewie が最高
  - [chewie | Flutter Package](https://pub.dev/packages/chewie#-installing-tab-)
  - [chewie-flutter-tutorial/pubspec.yaml at master · ResoCoder/chewie-flutter-tutorial](https://github.com/ResoCoder/chewie-flutter-tutorial/blob/master/pubspec.yaml)
  - [Flutter Video Player – Chewie Tutorial - Reso Coder](https://resocoder.com/2019/04/13/flutter-video-player-chewie-tutorial/)

## 画像を試す時
- [Lorem Picsum](https://picsum.photos/)
- [Beautiful Free Images & Pictures | Unsplash](https://unsplash.com/)
