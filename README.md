## XPipe Java dependencies

This repository contains Java module generation rules for dependencies used by XPipe.
As JLink effectively requires proper modules as inputs but many established java libraries did not add proper support yet, using an approach like this is required.

The modules are generated with the help of https://github.com/moditect/moditect-gradle-plugin.
The generated `module-info.java` only contains the necessary declarations to make a library work.
