import 'package:flutter/material.dart';
void main() {
runApp(const MyApp());
}
class MyApp extends StatelessWidget {
const MyApp({super.key});
@override
Widget build(BuildContext context) {
return MaterialApp(
home: MyHomePage(), //call
);
}
}
class MyHomePage extends StatelessWidget { //to call
const MyHomePage({super.key});
@override
Widget build(BuildContext context) {
return Scaffold(
appBar: AppBar(title: Text("Displaying an image"),
backgroundColor: Colors.lightGreen,),
body: Container(height: 600,
width: 600,
child: Image.asset('assets/Flower.jpg')
),
);
}
}
