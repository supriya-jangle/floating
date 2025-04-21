import 'package:flutter/material.dart';
void main() => runApp(MyApp());
class MyApp extends StatelessWidget {
@override
 Widget build(BuildContext context) {
 return MaterialApp(
 home: FloatingActionButtonDemo(),
 );
 }
}
class FloatingActionButtonDemo extends StatelessWidget {
 @override
 Widget build(BuildContext context) {
 return Scaffold(
 appBar: AppBar(title: Text('FloatingActionButton Example')),
 body: Center(
 child: Text('Press the Floating Action Button!'),
 ),
 floatingActionButton: FloatingActionButton(
 onPressed: () {
 print('Floating Action Button Pressed!');
 },
 child: Icon(Icons.add), // Icon displayed on the FAB
 backgroundColor: Colors.blue, // Background color of the FAB
 ),
 );
 }
}
