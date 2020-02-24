# Usage

```
git clone https://github.com/frank-dspeed/example-typechecking-mjs
code example-typechecking-mjs
``` 

click on the index.mjs it will turn red. watch for the import statment.

in the working folder you find the same structure but it will not error and let you click on the imported module and it has type awareness

once https://github.com/microsoft/TypeScript/issues/27957 is solved that will not be needed anymore but it will take some years.


## Instructions for ECMAScript Authors at present
- use the .js extension maybe .es.js 
- give module hint via package.json fild type and set it to module.
- Create individual CJS and ESM Packages or offer 2 folders with individual package.json files that are honting to the module type
  - when using the 2 folder structure you can still use a inital package.json in the route that uses the module and main filds to point to the individual module folders.