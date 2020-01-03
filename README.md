# Flutter_Tips

# Widget
- Widget のサイズが大きすぎて、キーボードが出てきた時に使える
  - SingleChildScrollView 
  - Flexible
  
- TextField 
  - デコるために使うのは、 InputDecoration
    - hintText, errorText など使える
  - border はコンストラクターでしか指定できない。noneはできる。
  - focusNode で、次の field を指定できる
  - .done + onEditingComplete でメソッド呼べる
  - controller で、文字を管理できる。clear など。
  
- Dialog
  - 

# Navigator
- id 管理良いかも 

# Error
- on PlatformException が便利
  - on PlatformException catch(e) → e.message でエラーが出るので！工数下げるためにこれでOKでは。

# Architecture
- BLoC
- Provider 
[Flutter Provider: Introduction - YouTube](https://www.youtube.com/watch?v=O71rYKcxUgA)


# ShortCut
[Flutter — IDE Shortcuts for Faster Development - Flutter Community - Medium](https://medium.com/flutter-community/flutter-ide-shortcuts-for-faster-development-2ef45c51085b)
