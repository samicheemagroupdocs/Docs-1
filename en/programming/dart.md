---
date: 2019-10-11
keywords: dart, .dart, dart file format, dart file, how to run dart files, .dart extension
author:
  display_name: Muhammad Ahmad Chishti
draft: false
toc: true
title: Dart File Format
linktitle: Dart
description: Learn about Dart file format and APIs that can create and open Dart files.
menu:
  docs:
    parent: "programming"
lastmod: 2021-05-18
---

## What is a Dart file? ##

A Dart file contains the source code of Dart programming language which is a client-optimized programming language developed by Google that is used to build apps for mobile, desktop, web, Iot (Internet of things) etc. Dart is an object-oriented language with a syntax similar to C. Dart can be compiled to either JavaScript or native code. You can run the Dart files in famous web browser just like as you can run a javascript file. A command line tool known as Dart virtual machine which comes with Dart SDK can is also used to compile and run the Dart files.

## Brief History ##

The Dart project was founded by Lars Bak and Kasper Lund and the first version was released on 14th November 2013. I the begining the Dart was criticized for the web fragmentation due to the plans for including a Dart VM in Google Chrome. Those plans were dropped and Dart focused on compiling to JavaScript with the release of version 1.9 in 2015.

Dart 2.0 was released in August 2018 in which the dart2native extension was introduced that compiled Dart code to native Linux, Windows, macOS platforms. This extension enabled self-contained executables due to which the Dart SDK was not required to run Dart apps om those platforms. This extension also integrated with Flutter making it possible to create cross-platform apps.

ECMA standardized Dart with the first edition in July 2014 and the second edition in December 2014.


## How to run/execute Dart code ##

Dart code can run in the following ways:

- **Compiled as JavaScript**: </br>The Dart code is compiled to JavaScript by using the dart2js compiler. The compiled JavaScript code is compatible with all major web browsers.
- **Stand-alone**: </br> The Dart Software Development Kit (SDK) ships with a stand-alone Dart VM that allows Dart code to run in the command-line interface. Dart ships with a complete standard library that allows users to write fully functional apps.
- **Ahead-of-time (AOT) compiled**: </br> Dart code can be AOT-compiled to machine code that allows mobile apps to be built with Flutter.
- **Native**: </br> With the dart2native compiler, Dart code can be compiled to self-contained executables that can run on Windows, Linux, and macOS.

## Dart File Format ##

Dart is a C-style object-oriented language that supports interfaces, mixins, abstract classes, reified generics, and type interface.

### Syntax ###

The following are some examples of Dart syntax.

#### Print to Console ####

```dart
// print "Hello World" to console
main() {
  print("Hello, World!");
}
```

#### Loops and Arrays ####

```dart
// loops and arrays
var names = {
  'John',
  'James',
  'Rose',
};
main() {
  for (var name in names) {
    print(name);
  }
}
```

#### Functions ####

```dart
// functions
int double(int x) {
  return x * 2;
}
main() {
  print("double of 10 is ${double(10)}");
}
```

#### Classes ####

```dart
// classes
abstract class Person {
  detail();
}

class Student implements Person {
  String firstName = "Jack";
  String lastName = "Wick";
  detail() => print("Student: $firstName $lastName");
}

main() {
  // The 'new' keyword is optional.
  Student student = Student();
  student.detail();
}
```

#### Mixins ####

Mixins are normal classes from which we can borrow methods/variables without inheriting them. This is done by using the *"with"* keyword.

```dart
class B {  
  method(){
     ....
  }
}

class A with B {
  ....
     ......
}
void main() {
  A a = A();
  a.method();  //We are able to access the method of B class without inheriting from it.
}
```

## References ##

- [Dart (programming language) - Wikipedia](https://en.wikipedia.org/wiki/Dart_(programming_language))
- [Dart](https://dart.dev/)
