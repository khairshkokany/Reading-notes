# Intent Filters

![images](https://tutorial.eyehunts.com/wp-content/uploads/2018/06/what-is-android-Intent-Filters-examples-768x565.png)

- If your app can perform an action that might be useful from another app, your app should be prepared to respond to action requests by specifying the appropriate intent filter in your activity.
  
- To allow other apps to start your activity in this way, you need to add an <intent-filter> element in your manifest file for the corresponding <activity> element.


## Add an Intent Filter

- The system may send a given Intent to an activity if that activity has an intent filter fulfills the following criteria of the Intent object:

  - Action
  - Data
  - Category

- Each incoming intent specifies only one action and one data type, but it's OK to declare multiple instances of the <action>, <category>, and <data> elements in each <intent-filter>.

## Handle the Intent in Your Activity
 - In order to decide what action to take in your activity, you can read the Intent that was used to start it.
 - As your activity starts, call getIntent() to retrieve the Intent that started the activity.

## Return a Result
- If you want to return a result to the activity that invoked yours, simply call setResult() to specify the result code and result Intent.
