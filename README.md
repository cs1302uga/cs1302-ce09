# cs1302-ce09 More Shapes

> Quid adhuc laborat?
> **--Most Latin Teachers**

This class exercise explores how to utilize inheritance in Java to create new classes
that are directly based on existing ones, with an emphasis on code reuse and design
implications. It also revists how to commit and view changes to a local Git repository.

## Prerequisite Knowledge

* Inheritance and polymorphism in Java.
* UML Class Diagrams

## Questions

In your notes, clearly answer the following questions. These instructions assume that you are 
logged into the Nike server. 

**NOTE:** If a step requires you to enter in a command, please provide in your notes the full 
command that you typed to make the related action happen. If context is necessary (e.g., the 
command depends on your present working directory), then please note that context as well.

### Getting Started

1. Use Git to clone the repository for this exercise onto Nike into a subdirectory called `cs1302-ce09`:

   ```
   $ git clone --depth 1 https://github.com/cs1302uga/cs1302-ce09.git
   ```

1. **[ALL GROUP MEMBERS]**
   If you did not setup your Git username and email on Nike when working on `cs1302-ce07`,
   then please revist that exercise and follow the instructions presented there.

1. Change into the `cs1302-ce09` directory that was just created and look around. There should be
   multiple Java files contained within the directory structure. To see a listing of all of the 
   files under the `src` subdirectory, use the `find` command as follows:
   
   ```
   $ find src
   ```

   This is the same starter code from `cs1302-ce08`! Refer to your notes for that exercise about
   any inter-dependencies and/or inheritance between the files.

1. In your notes, draw a complete, proper UML diagram for the three classes contained in the
   starter code. **You might need to devote an entire page to this. We recommend using a pencil.** 
   Specifically, each individual class diagram should contain:

   * Class name;
   * Variables;
   * Constructors and methods;
   * If needed, a solid generalization arrow (`extends`) to a parent class; and
   * If needed, a dashed generalization arrow (`implements`) to an interface.

   In a class diagram, do not list inherited members unless they are explicitly overriden.
   Where applicable, be sure to include visibility modifiers (e.g., `+`, `#`, `~`, `-`) and
   type / return type information. Also, remember that generalization arrows have a triangle
   arrow head, which differentiates them from dependency and aggregration associations.

**CHECKPOINT**

1. Create and document a `Rectangle` class in the `cs1302.shapes` package. It should extend
   the `Shapes` class. In addition to including relevant instance variables for describing
   a rectangle, it should provide overrides for the `getArea` and `getPerimeter` methods.
   Additionally, include getter methods for the instance variables. 

1. Compile your `Rectangle` class. If you encounter any compililation errors:

   1. Write the error down in your notes;
   1. Fix the error in your code;
   1. Recompile; then
   1. Note the fix in your notes.
   1. Repeat as needed.

1. 

# On branch master
# Untracked files:
#   (use "git add <file>..." to include in what will be committed)
#
#	src/cs1302/shapes/Rectangle.java
nothing added to commit but untracked files present (use "git add" to track)


   Use the following commands to tell Git to add and commit the changes that you made to your
   source code to your local copy of the repository for this exercise.
   Modify the string associated with the `-m` (message) option to give a brief, one sentence 
   description of the changes you made to the source code.
   
   ```
   $ git add src
   $ git commit -m "added SomeClass that represents SOMETHING and implements Drivable."
   ```

1. Generate the API documentation website for all of the code in the `cs1302` package
   into the `doc` directory. You may need to create the `doc` directory if it does not already exist.
   Host the documentation on Nike using `cs1302-ce07-doc` as the name for your symbolic link. Write
   the full URL of your API documentation website in your notes.




