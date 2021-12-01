## XPipe java dependencies

This repository contains gradle java module generation rules for XPipe dependencies.
As JLink effectively requires proper modules as inputs but many established java libraries did not add proper support yet, using an approach like this is required.
The modules are generated with the help of https://github.com/moditect/moditect-gradle-plugin.