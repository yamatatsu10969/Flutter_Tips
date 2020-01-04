# Flutter_Tips

## Option + Enter をとりあえず押してみるの大事。
- method 作成
- widget 作成
- remove もできる
- コンストラクタの作成
- import もできる
- なんでもできそう。

# UI
- Placeholder 使うと一時的に置けるのでいいな


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

# Error
- map 使っている時に、toList がつけずに型が合わないことがある。
- 

# Exception
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
