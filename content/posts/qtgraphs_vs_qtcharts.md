+++
title = "Qt Charts and Qt Graphs"
draft = true
+++

## Introduction

Visualizing data in the form of charts is essential to many applications. Some of applications are very data intensive such as medical or automative. Medical applications are very critical and it is very important to visualize real time data.

Qt provide different apis for drawing different kind of charts. One such API for QML is called Qt Charts. Qt Charts uses the Graphic View Framework for ease of integration. Qt Graphic View was introduced in Qt 4.2 replacing its predecessor QCanvas.Graphic view provides an item-based approach to model-view programming.

## The Graphic View Architecture
Graphic view provide an item-based approach to model-view programming. Several views can observe a single scene, and the scene contains items of varying geometric shapes.# The Scene
QGraphicScene provides a fast interface for managing a large number of items. It enable event propagations to the items, managing item state, such as selection and focus handling and provide untransformed rendering functionality. 

The scene serve as a container for QGraphicItem objects. QGraphicScene allows to render part of the scene into a paint device through the QGraphicScene::render() function.

# The View
QGraphicView provides the view widget, that visualizes the content of the scene. You can attach several views to the same scene, to provide several view ports into the same data set. The view receive view events from the keyboard and mouse, and translate these scene events before sending the events to the visualized scene. Using the transformation matrix, QGraphicsView::transform(), the view can transform the scene coordinate system. This allow advanced navigation features such as zomming and rotation. 

# The Item
QGraphicItem is the base class for graphical items in a base. 

## Paint System
Qt's paint system enables painting on screen and print devices using the same API's, and is primarily based on the QPainter, QPaintDevice and QPaintEngine.

## Qt Graphs

## Qt Quick Scene Graph
Qt Quick 2 makes use of a dedicated scene graph that is then traversed and rendered via a graphic API such as OpenGL ES, OpenGL, Vulkan, Metal, or Direct 3D. Using a scene graph for rendering compared to traditional imperative painting systems (QPainter and similar), means the scene to be rendered can be retained between frames and the complete set of primitives to render is known before rendering starts. The Scene Graph is closely tied to Qt Quick 2.0 and cannot be used standalone. The scene graph is managed and rendered by the QQuickWindow class. 

## [Graphics](https://doc.qt.io/qt-6/topics-graphics.html)
QtQuick uses scene graph for rendering as describe above. QtQuick3D is an add-on that provide high level API for creating 3D content and 3D user interfaces based on Qt Quick. It extends the Qt scene graph  which lets you implement the 3D content on 2D Qt Quick applications. 
# High Level Graphics with Qt GuI
Qt GUI provides a high level windowing, painting, and typography system. QPainter provides an API for drawing vector graphics, text and images onto different surfaces, or QPainDevice instances such as QImage, QOpenGLPaintDevice, QWidget, and QPainter. 
# Low Level Graphics with Qt GUI
Qt GUI provides cross-platform enablers for managing OpenGL contexts and Vulkan instances. Applicaiton that perform rendering directly with OpenGL, OpenGL ES, or Vulkan can use different Qt objects. 
Qt GuI also offers Qt Rendering Hardware Interface (QRhi) family of API, such as QRHI and QShader, for application that want to perform rendering using the portable, cross-platform 3D rendering infrastructure Qt itself uses to implement the Qt Quick scene graph and Qt Quick 3D rendering engine. 
