# trial
//frameworks
import 'package:flutter/material.dart';

void main() {
  runApp(MyApp());
}

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        appBar: AppBar(title: Text('Picture and Word')),
        body: Center(
          child: Row(
            mainAxisAlignment: MainAxisAlignment.center,
            children: [
              Image.asset(
                'assets/images/picture.jpg', // Replace with your own image path
                width: 100, // Adjust the width as needed
                height: 100, // Adjust the height as needed
              ),
              SizedBox(width: 10), // Optional spacing between the picture and word
              Text(
                'Hello', // Replace with your own word
                style: TextStyle(fontSize: 24), // Adjust the font size as needed
              ),
            ],
          ),
        ),
      ),
    );
  }
}
