# Re-Vim-d

Re-Vim'd is a lightweight implementation of classic Vi editor using C++.   
We implemented most of the core features in Vim editor including: navigation, file open/save, editing, undo, macros, syntax-highlighting for the C++ language.

As a high-level overview, the program follows a Model View Controller (MVC) architecture
with support of dynamic module loading. 
Essentially, we have a lightweight vm core that relies on libdl to
dynamically load plugins at runtime. This design has provided several attractive advantages:

● Extensibility by design - since anything beyond the most basic features is expected to be
componentized, nearly anything can be created or even overridden in vm.  
● Modularity - we ensure all core functionality is flexible and more importantly pluggable.  
● Reduced compilation time - only the changed modules will require updating.  
● Easy to debug - complete program isolation significantly reduces code complexity.  
● Built for updates - new core features and APIs can be created later on with minimal impact
towards backwards compatibility.  

## Instruction 
``` bash
unzip <name-of-the-zip-file>.zip
cd build
./src/vm <file-to-be-open>
```

Disclaimer: Due to University of Waterloo Policy #71, source code of this project is not publically available. However, I am gladly willing to share the source code upon request for non-course purposes.
