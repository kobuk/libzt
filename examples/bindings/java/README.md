## ZeroTier with Java via JNI
***

To get this example project to work, do the following:

- From libzt main directory, build shared library: `make shared_jni_lib`
- Copy the resultant dynamic library (`*.so` or `*.dylib`) from `build/` to this current directory
- Change to this directory and `make example_java_app`
- Run: `java -cp "." ExampleApp`


Notes:

Upon execution, it will load the libzt dynamic library via the `loadLibrary` method and begin generating an identity.