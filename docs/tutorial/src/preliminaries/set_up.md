# Set up MMTk and OpenJDK

This tutorial can be completed with any binding. However, for the sake of 
simplicity, only the setup for the OpenJDK binding will be described in detail 
here. If you would like to use another binding, you will need to follow the 
README files in their respective repositories 
([JikesRVM](https://github.com/mmtk/mmtk-jikesrvm), 
[V8](https://github.com/mmtk/mmtk-v8))
 to set them up, and find appropriate benchmarks for testing. 
 Also, while it may be useful to fork the relevant repositories to your own 
 account, it is not required for this tutorial.

First, set up OpenJDK, MMTk, and the binding:
1. Install the required dependencies following the instructions at [mmtk-dev-env](https://github.com/mmtk/mmtk-dev-env).
1. Clone the OpenJDK binding and mmtk-core repository following the instructions at the [OpenJDK binding repository]. The instructions provides multiple options for building the OpenGDK binding. Choose the following options:
   *  Get a local copy of MMTk-core:

      [Checkout MMTk core] is mentioned as an optional step in the instructions.
      However, we need it to be done in this tutorial.
      So don't skip this step.

   *  Use the `slowdebug` build option:
   
      This is the fastest debug variant to build, and allows for easier debugging and better 
      testing. The rest of the tutorial will assume you are using `slowdebug`.

## Keeping multiple JVM builds

If you do need to keep multiple JVMs with different configurations, you can do so by renaming the `build` folder or the 
folder generated within it (eg `linux-x86_64-normal-server-$DEBUG_LEVEL`) after build completes.

[OpenJDK binding repository]:https://github.com/mmtk/mmtk-openjdk/blob/master/README.md
[mmtk-core repository]:https://github.com/mmtk/mmtk-core/blob/master/README.md
[Checkout MMTk core]:https://github.com/mmtk/mmtk-openjdk/blob/master/README.md#checkout-mmtk-core-optional
