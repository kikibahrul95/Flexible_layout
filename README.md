# Flexible_layout
flutter
import 'package:flutter/material.dart';

void main() => runApp(MyApp());

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(home: Scaffold(appBar: AppBar(title: Text("flexible layout"),),
    body: Column(
      
      children: <Widget>[
    
        Flexible(flex: 1,
        child:  Row(children: <Widget>[
          Flexible(flex: 1,
          child: Container(
            color: Colors.brown,
            Flexible(flex: 1,
          child: Container(
            color: Colors.lime,
        ],))
          Flexible(flex: 2,
          child: Container(
            color: Colors.brown,
          )),
          Flexible(flex: 1,
          child: Container(
            color: Colors.cyan,
          )),
      ],
    ),),

    );
  }
}
