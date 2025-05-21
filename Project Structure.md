〇プロジェクトの構成

・main.dartのソースコード

import 'package:flutter/material.dart';

void main() {
  runApp(MyApp());
}

class MyApp extends StatelessWidget {

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      tetle: 'Flutter Demo',
      home: Text(
        'Hello, Flutter World!!',
        style: TextStyle(fontSize:32.0),
      ),
    );
  }
}

・アプリ画面とウィジェットツリー

・StatlessWidgetクラス(静的)

・MaterialAppクラス

・ScaffoldとAppBar
import 'package:flutter/material.dart';

void main() {
  runApp(MyApp());
}

class MyApp extends StatelessWidget {

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      tetle: 'Flutter Demo',
      home: Scaffold(
        appBar: AppBar(
            title: Txt('Hello Flutter!'),
        ),
        body: Text(
          'Hello, Flutter World!!',
          style: TextStyle(fontSize:32.0),
        ),
      ),
    );
  }
}
