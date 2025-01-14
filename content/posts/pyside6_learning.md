+++
title = "Learning Pyside6"
draft = true
+++
## Introduction

Qt is an application development and UI framework. Ui is developed using Qt widgets or QML. Qt Widgets is used for desktop application development whereas QML is used for mobile apps, embedded apps and so on. <br>
Qt framework is written in c++. Therefore the backend is traditionally written in Qt c++. The Qt C++ adds some additional capabilities to the standard c++. These capabilities include adding introspection to c++ through storing information to every QObject derived class (using Q_ObJECT macro).

Qt support python bindings for the Qt. Therefore python can be used to develop your application. Using PySide6, you can use Qt6API in your python application. And Shiboken6, a binding generator tool, that can be used to expose C++ projects to python, and a python module with some utility functions.

### Quick Start
Install the latest version of Pyside: <br>
'pip install pyside6'

