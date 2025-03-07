README.md
Duck Behavior Simulation
Overview

This Java application demonstrates the behavior of different types of ducks using the Strategy Design Pattern. The program is based on the class diagram from O'Reilly's Head First Design Patterns book and extends it by adding new behavior interfaces for swimming.
Features

    Implements the Strategy Pattern to allow dynamic behavior changes.
    Uses separate interfaces for fly behavior and swim behavior.
    Implements different types of ducks as per the class diagram.
    Allows ducks to fly, swim, float, or drown based on their behavior.
    Uses separate Java files for modularity and maintainability.
    Follows best coding practices with structured code and meaningful comments.

Class Structure
1. Duck (Abstract Class)

    Defines common behavior and properties for all ducks.
    Contains a reference to FlyBehavior and SwimBehavior for dynamic behavior assignment.
    Implements a method to display the duck’s behavior.

2. FlyBehavior (Interface)

    Defines the fly() method.
    Implemented by:
        Fly – Ducks that can fly.
        NotFly – Ducks that cannot fly.

3. SwimBehavior (Interface)

    Defines the swim() method.
    Implemented by:
        Swim – Ducks that can swim.
        Float – Ducks that float on water.
        Drown – Ducks that cannot swim and drown.

4. Duck Subclasses

Each duck class extends Duck and assigns the appropriate FlyBehavior and SwimBehavior.

    MallardDuck – Flies and Swims
    RedheadDuck – Flies and Swims
    RubberDuck – Does not fly, Floats
    DecoyDuck – Does not fly, Floats
    ModelDuck – Initially does not fly, but can be changed dynamically

How to Use

    Clone the repository:

git clone https://github.com/yourusername/StrategyPattern.git

Compile the Java files:

javac *.java

Run the main program:

    java Main

    The program will display the behavior of different ducks as per their assigned behaviors.

File Structure

StrategyPattern/
│── src/
│   │── Duck.java               # Abstract class for all ducks
│   │── FlyBehavior.java        # Interface for flying behavior
│   │── Fly.java                # Implementation for ducks that fly
│   │── NotFly.java             # Implementation for ducks that do not fly
│   │── SwimBehavior.java       # Interface for swimming behavior
│   │── Swim.java               # Implementation for ducks that swim
│   │── Float.java              # Implementation for ducks that float
│   │── Drown.java              # Implementation for ducks that drown
│   │── MallardDuck.java        # MallardDuck class
│   │── RedheadDuck.java        # RedheadDuck class
│   │── RubberDuck.java         # RubberDuck class
│   │── DecoyDuck.java          # DecoyDuck class
│   │── ModelDuck.java          # ModelDuck class with dynamic behavior change
│   │── Main.java               # Main driver class for execution
│
│── README.md                   # This file
│── .gitignore                   # Git ignore file
│── LICENSE                      # License file (if applicable)
│── class_diagram.png            # UML Class Diagram of the program

Commit Guidelines

    Each Java file should be committed separately.
    Example commit messages:
        Added abstract class Duck with behavior references
        Implemented FlyBehavior and SwimBehavior interfaces
        Added Swim, Float, and Drown classes for swim behavior
        Implemented MallardDuck and RedheadDuck classes
        Updated Main.java with duck behavior execution

Submission Guidelines

    Convert all Java files into a single PDF file.
    Include the GitHub repository link at the end of the PDF file.

Author

    Name:Akhil Chivukula
    PRN: 230
    Batch: [Your Batch]
