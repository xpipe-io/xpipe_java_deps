## XPipe Java dependencies

This repository contains Java module generation rules for dependencies used by XPipe.
As JLink effectively requires proper modules as inputs but many established java libraries did not add proper support yet, using an approach like this is required.

The modules are generated with the help of https://github.com/moditect/moditect-gradle-plugin.
The generated `module-info.java` only contains the necessary declarations to make a library work.


While gradle already has a (similar system)[https://docs.gradle.org/current/userguide/platforms.html] to better share dependencies, this system is lacking several features.
For one, it can't pass any other customizations to the build that are required by the dependencies, e.g. compiler parameters or annotation processors.