<!-- 
This README describes the package. If you publish this package to pub.dev,
this README's contents appear on the landing page for your package.

For information about how to write a good package README, see the guide for
[writing package pages](https://dart.dev/guides/libraries/writing-package-pages). 

For general information about developing packages, see the Dart guide for
[creating packages](https://dart.dev/guides/libraries/create-library-packages)
and the Flutter guide for
[developing packages and plugins](https://flutter.dev/developing-packages). 
-->


## Features
<table>
  <tr>
    <td>
      <img src="https://firebasestorage.googleapis.com/v0/b/average-6fee8.appspot.com/o/Screenshot_1632894903.png?alt=media&token=1939ed8f-0249-4e1c-b839-f2e5cf453b6d" alt=" ">
    </td>
  </tr>
  </table>
  


## Getting started
start using the package.




## Usage
 
```dart
import 'package:flutter/material.dart';
import 'package:hover_card/hover_card.dart';
void main() {
  runApp(MyApp());
}
class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'Hover - Tilt 3D Effect',
      theme: ThemeData(
        primarySwatch: Colors.blue,
        visualDensity: VisualDensity.adaptivePlatformDensity,
      ),
      home: Material(
        child: Column(
          mainAxisAlignment: MainAxisAlignment.center,
          children: [
            const Text(
              'Hover - Tilt 3D Effect. \n   instagram : xr_yr ',
              style: TextStyle(
                  fontSize: 30,
                  fontWeight: FontWeight.w700,
                  color: Colors.black,
                  letterSpacing: 2),
            ),
            const SizedBox(height: 50),
            SizedBox(
              width: 150,
              height: 300,
              child: HoverCard(
                builder: (context, hovering) {
                  return Container(
                    color: const Color(0xFFE9E9E9),
                    child: const Center(
                      child: FlutterLogo(size: 100),
                    ),
                  );
                },
                depth: 10,
                depthColor: Colors.grey[500],
                onTap: () => print('Hello, World!'),
                shadow: BoxShadow(color: Colors.purple[100] as Color, blurRadius: 30, spreadRadius: -20, offset: const Offset(0, 40)),
              ),
            ),
          ],
        ),
      ),
    );
  }
}
```


