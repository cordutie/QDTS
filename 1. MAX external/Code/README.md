## Building the MAX external

The implementation of the algorithm in MAX was built using the `min devkit`, 
a software development kit containing an example package with the current 
best practices for package creation using modern C++ code. This implies that
in order to build the code it is necessary to first build a clone project
of the `min devkit`. In order to do this we refer to the actual documentation
of the `min devkit` which can be found [here](https://github.com/Cycling74/min-devkit),
however a small guide containing the general ideas can be found here:

> Prerequisites: Max 8, Ruby, CMake and Visual Studio or Xcode have to be 
installed prior to the build of the project.

1. Clone the `min devkit` repository inside the directory **MAX 8/Packages**.
2. From the `min devkit` folder, run the code `ruby script\create_package.rb .. \qdts`.
This will create a new package called *qdts*.
3. Copy and paste the folder *qdts.solver* inside this repository to the directory
*MAX 8/Packages/qdts/source/projects*.
4. Run CMake, indicate the directory of the *qdts* package, the subfolder build 
and your IDE. Configure the project twice and then build it. This will build
a project that can be run from your IDE.
5. Compile the project you just built.