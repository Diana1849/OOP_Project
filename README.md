# Shapes OOP Project (Java)

A Java project that demonstrates core object-oriented programming concepts through a simple shapes hierarchy.

## OOP Concepts Used
- Interface: Drawable (howToDraw)
- Abstract classes: Shape (area, perimeter), ThreeDShape (volume)
- Inheritance: Circle extends Shape, Cube extends ThreeDShape
- Polymorphism: shapes are stored in a Drawable[] array and handled uniformly
- Method overriding and constructor overloading

## Classes
- Shape / ThreeDShape: abstract base classes
- Circle: area = pi * r^2, perimeter = 2 * pi * r
- Cube: area = 6 * s^2, perimeter = 12 * s, volume = s^3
- MyProject: reads shapes from command-line arguments and prints the results
- FileClass: reads shapes from an input file and writes the results to an output file

## Input Format
(Array_Size) (Shape) (Dimension) (Shape) (Dimension) ...

Example: 3 square 22 circle 22.5 cube 23.6

Supported shapes: circle, cube. Array size must be at least 2, and dimensions must be positive. Unsupported shapes are reported as invalid.

## How to Run
Requires JDK 23 and Maven.

Command line:
java com.mycompany.myproject.MyProject 2 circle 5 cube 3

From a file:
java com.mycompany.myproject.FileClass input.txt output.txt

## Output
Prints each shape's description and the total area of all shapes.
