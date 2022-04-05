# Activity-lifecycle-and-state

<img src="/Screenshot/two_activities_lifecyle.png" width="500" height="250"/>
<img src="/Screenshot/Shopping_list.gif" width="300" height="250"/>
<img src="/Screenshot/ActivityLifecycle_homework.gif" width="350" height="250"/>


If you run the homework app before implementing onSaveInstanceState(), what happens if you rotate the device?

Ans - The counter is reset to 0, but the contents of the EditText is preserved.

What Activity lifecycle methods are called when a device-configuration change (such as rotation) occurs?

Ans - Android shuts down your Activity by calling onPause(), onStop(), and onDestroy(), and then starts it over again, calling onCreate(), onStart(), and onResume().

When in the Activity lifecycle is onSaveInstanceState() called?

Ans - onSaveInstanceState() is called before the onStop() method.

Which Activity lifecycle methods are best to use for saving data before the Activity is finished or destroyed?

Ans - onPause() or onStop()
