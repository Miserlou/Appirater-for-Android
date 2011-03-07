Introduction
------------
Appirater is a class that you can drop into any Android app that will help remind your users
to review your app on the Android Market. The code is released under the MIT/X11, so feel free to
modify and share your changes with the world.

This is a clean port of Appirater by [Arash Payan] [arash].

The original appirater for iOS can be found [here] [iosversion] and more information about it [here] [ioshomepage].

Getting Started
---------------
1. Add the Appirater code into your project
2. If you don't have INTERNET permission already, add it to your manifest file:
   <uses-permission android:name="android.permission.INTERNET"/>
   * This is only used to check if we can actually send a user to the market to rate the app.
3. Add a member for Appirater to your main activity
4. In your main activity's onCreate method, create the Appirater instance
   and call appLaunched( true )
5. In your main activity's onResume() method, call appEnteredForeground( true )
6. (OPTIONAL) Call userDidSignificantEvent(true) when the user does something 'significant'
   in the app.

License
-------
Copyright 2010. [Arash Payan] [arash]
Copyright 2011. [IJsbrand Slob] [huppie].
This library is distributed under the terms of the MIT/X11.

While not required, I greatly encourage and appreciate any improvements that you make
to this library be contributed back for the benefit of all who use Appirater.

[iosversion]: https://github.com/arashpayan/appirater/
[ioshomepage]: http://arashpayan.com/blog/index.php/2009/09/07/presenting-appirater/
[arash]: http://arashpayan.com
[huppie]:http://ijsbrandslob.com/