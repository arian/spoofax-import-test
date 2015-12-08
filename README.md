This projects shows that importing things from other modules are not working
correctly.

For example use these two files that work with this spoofax language:

**x.dummy**
```
module x
import y
reference x
```

**y.dummy**
```
module y
declare x
```

That works great, until:

1. you close all files and eclipse
2. you open eclipse
3. open `x.dummy`
4. see the *Unresolved reference* errors at `import y` and `reference x`.
