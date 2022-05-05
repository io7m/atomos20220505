Without `org.osgi:osgi.core:8.0.0`:

```
[INFO] --- maven-compiler-plugin:3.10.1:compile (default-compile) @ com.io7m.atomos20220505 ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 2 source files to /home/rm/git/com.github/io7m/atomos-example-20220505/target/classes
[INFO] -------------------------------------------------------------
[ERROR] COMPILATION ERROR : 
[INFO] -------------------------------------------------------------
[ERROR] module not found: osgi.core
[INFO] 1 error
[INFO] -------------------------------------------------------------
```

With `org.osgi:osgi.core:8.0.0`:

```
Error occurred during initialization of boot layer
java.lang.module.ResolutionException: Module osgi.core contains package org.osgi.framework.wiring, module org.apache.felix.framework exports package org.osgi.framework.wiring to osgi.core
```
