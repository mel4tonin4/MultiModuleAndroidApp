# MultiModuleAndroidApp

**WARNING: This is a purposefully BROKEN PROJECT which triggers a bug in Android Studio.**

A multi-module Android application with resources and UI in two secondary modules

This project builds correctly and the application runs.

However, Android Studio seems to not be able to generate the R class.

**The problem is that multiple android (application and library) modules can share the same package but creating multiple R classes in the same Java package will result in a conflict. On specific occasions, your application may still build and run but the IDE will get confused.**

This project was created by starting from the "Navigation Drawer Activity" template, and then moving most of the resources to a module and the whole UI to another module.

This is now an assigned Android Studio issue with priprity P3: https://issuetracker.google.com/issues/151765079

**The IDE issue is that it fails to provide a proper diagnostics message for this issue, leaving you in the dark.**
