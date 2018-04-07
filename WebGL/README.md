# Welcome to WebGL

## What is WebGL ?

WebGL (Web Graphics Library) is the new standard for 3D graphics on the Web, It is designed for the purpose
of rendering 2D graphics and interactive 3D graphics. It is derived from OpenGL's ES 2.0 library
which is a low-level 3D API for phones and other mobile devices. WebGL provides similar functionality
of ES 2.0 (Embedded Systems) and performs well on modern 3D graphics hardware.


## Support Browsers
- Web Browsers
**I**nternet **E**xplorer ( 11 and above ), Google Chrome (39 and above) and 
Safari are given full support. Others give partial support.
- Mobile Browsers
IOS Safari (version 8.3) and Blackberry Browser (version 10) are given full support. Others give partial support.

## Advantages of WebGL
- JavaScript programming 
WebGL applications are written in JavaScript. Using these applications.
- Increasing support with mobile browsers
- Open source
- No need for compilation
- Automatic memory management
- Easy to set up

## Enviroment Setup

There is no need to set a different environment for WebGL. The browsers supporting WebGL have their own in-built setup for WebGL.

To create graphical applications on the web, HTML-5 provides a rich set of features such as 2D Canvas, WebGL, SVG, 3D CSS transforms, and SMIL. To write WebGL applications, we use the existing canvas element of HTML-5. 

WebGL is mostly a low-level rasterization API rather than a 3D API. To draw an image using WebGL, you have to pass a vector representing the image. It then converts the given vector into pixel format using OpenGL SL and displays the image on the screen. 

## WebGL – Coordinate System

Just like any other 3D system, you will have x, y and z axes in WebGL, where the z axis signifies depth. The coordinates in WebGL are restricted to (1, 1, 1) and (-1, -1, - 1). It means − if you consider the screen projecting WebGL graphics as a cube, then one corner of the cube will be (1, 1, 1) and the opposite corner will be (-1, -1, -1). WebGL won’t display anything that is drawn beyond these boundaries.

## WebGL Fundamentals

After getting the WebGL context of the canvas object, you can start drawing graphical elements using WebGL API in JavaScript.

Here are some fundamental terms you need to know before starting with WebGL.

- Vertices

Generally, to draw objects such as a polygon, we mark the points on the plane and join them to form a desired polygon. A vertex is a point which defines the conjunction of the edges of a 3D object. It is represented by three floating point values each representing x, y, z axes respectively.
Example,

In the following example, we are drawing a triangle with the following vertices − (0.5, 0.5), (-0.5, 0.5), (-0.5, -0.5).

Note − We have to store these vertices manually using JavaScript arrays and pass them to the WebGL rendering pipeline using vertex buffer.

- Indices

In WebGL, numerical values are used to identify the vertices. These numerical values are known as indices. These indices are used to draw meshes in WebGL.

Note − Just like vertices, we store the indices using JavaScript arrays and pass them to WebGL rendering pipeline using index buffer.

- Arrays

Unlike OpenGL and JoGL, there are no predefined methods in WebGL to render the vertices directly. We have to store them manually using JavaScript arrays.
Example

var vertices = [ 0.5, 0.5, 0.1,-0.5, 0.5,-0.5] 

- Buffers

Buffers are the memory areas of WebGL that hold the data. There are various buffers namely, drawing buffer, frame buffer, vetex buffer, and index buffer. The vertex buffer and index buffer are used to describe and process the geometry of the model.

'''

    Vertex buffer objects − This stores data corresponding to each vertex (per-vertex data)

    Index buffer objects This stores data about the indices.

    Frame buffer is a portion of graphics memory that hold the scene data. This buffer contains details such as width and height of the surface (in pixels), color of each pixel and their depth.

'''

After storing the vertices into arrays, we pass them to WegGL graphics pipeline using these Buffer objects.

- Mesh

To draw 2D or 3D objects, the WebGL API provides two methods namely, drawArrays() and drawElements(). These two methods accept a parameter called mode using which you can select the object you want to draw. The options provided by this field are restricted to points, lines, and triangles.

To draw a 3D object using these two methods, we have to construct one or more primitive polygons using points, lines, or triangles. Thereafter, using those primitive polygons, we can form a mesh.

A 3D object drawn using primitive polygons is called a mesh. WebGL offers several ways to draw 3D graphical objects, however users normally prefer to draw a mesh.

Example

In the following example, you can observe that we have drawn a square using two triangles→ {1, 2, 3} and {4, 1, 3}.




