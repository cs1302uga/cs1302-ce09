# cs1302-ce09 More Shapes

> 十人十色 (Ten People, Ten Colors)
> **--Japanese Idiom**

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
   a rectangle, it should provide a constructor and a set of overrides for the `getArea` and
   `getPerimeter` methods. Additionally, include getter methods for the instance variables. 

1. Compile your `Rectangle` class. If you encounter any compililation errors:

   1. Write the error down in your notes;
   1. Fix the error in your code;
   1. Recompile; then
   1. Note the fix in your notes.
   1. Repeat as needed.

1. Check the status of your local copy of the `cs1302-ce08` repository using the following
   command:

   ```
   $ git status
   ```

   You should see a message similar to the following:

   ```
   # On branch master
   # Untracked files:
   #   (use "git add <file>..." to include in what will be committed)
   #
   #	src/cs1302/shapes/Rectangle.java
   nothing added to commit but untracked files present (use "git add" to track)
   ```

   As the message suggests, your `Rectangle.java` file is untracked. To have Git track
   changes on this file, follow the instructions in the message. 

1. Now, use Git to commit the changes that you made to your source code to your local
   copy of the repository. Remember to use the `-m` (message) option to give a brief,
   one sentence description of the changes you made to the source code. If you forget
   the `-m` option, then you Git will likely throw you into the Vi program to enter
   a message! 😱 Don't be scared if this happens to you... Press `i`, type your sentence,
   then press the intuitive sequence of keys: `ESC`, `:`, `wq!`, followed by return.
   Next time, remember the `-m` option. 

1. Generate the API documentation website for all of the code in the `cs1302` package
   into the `doc` directory. You may need to create the `doc` directory if it does not already exist.
   Host the documentation on Nike using `cs1302-ce09-doc` as the name for your symbolic link. Write
   the full URL for the `Rectangle` class in your notes.

**CHECKPOINT**

1. Create and document a `Square` class in the `cs1302.shapes` package. It should extend
   your `Rectangle` class. You shouldn't need to introduce any new instance variables,
   but you should include a constructor that makes proper use of the `super` keyword.

1. Compile your `Square` class. If you encounter any compililation errors:

   1. Write the error down in your notes;
   1. Fix the error in your code;
   1. Recompile; then
   1. Note the fix in your notes.
   1. Repeat as needed. 
   
1. Use `wc` to check some coder stats! 

   1. How many lines are in `Rectangle.java`?
   1. How many lines are in `Square.java`?

1. Tell Git to track changes made to your `Square.java` file, then commit the changes
   to your local copy of the repository. Be sure to include a good log message. 

1. Generate the API documentation website for all of the code in the `cs1302` package
   into the `doc` directory. You may need to create the `doc` directory if it does not already exist.
   Host the documentation on Nike using `cs1302-ce07-doc` as the name for your symbolic link. Write
   the full URL for the `Square` class in your notes.

1. Create and document a `ShapeDriver` (driver) class in the `cs1302.shapes` package. Inside of the `main`
   method do the following:

   1. Create a `Shape` array, and populate it with two objects of each class. Something like the
      following (will need to be modified):

      ```java
      Shape shapes = new Shape[] {
          new Ellipse(1.1, 2.5), 
          new Circle(1.5)
      };
      ```
      
   1. Loop over the array. For each element in the array, print the name of the shape using the
      `getName` method as well as the return values of the `getArea` and `getPerimeter` methods.

1. Compile the `ShapeDriver` class and run it. 
   Is the output what you expected?

1. Tell Git to track changes made to your `ShapeDriver.java` file, then commit the changes
   to your local copy of the repository. Be sure to include a good log message. 

1. Regenerate the API documentation website for all of the code in the `cs1302` package.
   What is the direct URL to the API documentation for the class that you wrote
   for this checkpoint?

1. Use Git to view your commit log.

