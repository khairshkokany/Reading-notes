# Android Fundamentals

![img](https://google-developer-training.github.io/android-developer-phone-sms-course/adf_logo.png)

- Android apps can be written using 
1. Kotlin, 
2. Java, and 
3. C++ languages

- The Android SDK tools compile your code along with any data and resource files into an APK or an Android App Bundle.

- Each Android app lives in its own security sandbox, protected by the following Android security features:
1. The Android operating system is a multi-user Linux system in which each app is a different user.
 2. By default, the system assigns each app a unique Linux user ID (the ID is used only by the system and is unknown to the app). The system sets permissions for all the files in an app so that only the user ID assigned to that app can access them.
 3. Each process has its own virtual machine (VM), so an app's code runs in isolation from other apps.
 4. By default, every app runs in its own Linux process. The Android system starts the process when any of the app's components need to be executed, and then shuts down the process when it's no longer needed or when the system must recover memory for other apps.



> There are ways for an app to share data with other apps and for an app to access system services:

1. It's possible to arrange for two apps to share the same Linux user ID, in which case they are able to access each other's files. To conserve system resources, apps with the same user ID can also arrange to run in the same Linux process and share the same VM. The apps must also be signed with the same certificate.
2. An app can request permission to access device data such as the device's location, camera, and Bluetooth connection. The user has to explicitly grant these permissions.


> There are four different types of app components:
1. Activities: An activity is the entry point for interacting with the user. It represents a single screen with a user interface
2. Services: is a general-purpose entry point for keeping an app running in the background for all kinds of reasons. It is a component that runs in the background to perform long-running operations or to perform work for remote processes.
3. Broadcast receivers: is a component that enables the system to deliver events to the app outside of a regular user flow, allowing the app to respond to system-wide broadcast announcements.
4. Content providers: A content provider manages a shared set of app data that you can store in the file system, in a SQLite database, on the web, or on any other persistent storage location that your app can access. Through the content provider, other apps can query or modify the data if the content provider allows it.

- A unique aspect of the Android system design is that any app can start another app’s component.

**Activating components**
> Three of the four component types—activities, services, and broadcast receivers—are activated by an asynchronous message called an intent. Intents bind individual components to each other at runtime. You can think of them as the messengers that request an action from other components, whether the component belongs to your app or another.

**The manifest file**
> Before the Android system can start an app component, the system must know that the component exists by reading the app's manifest file, AndroidManifest.xml. Your app must declare all its components in this file, which must be at the root of the app project directory.

**Declaring components**

> The primary task of the manifest is to inform the system about the app's components. For example, a manifest file can declare an activity as follows:

```
<?xml version="1.0" encoding="utf-8"?>
<manifest ... >
    <application android:icon="@drawable/app_icon.png" ... >
        <activity android:name="com.example.project.ExampleActivity"
                  android:label="@string/example_label" ... >
        </activity>
        ...
    </application>
</manifest>
```



**Declaring component capabilities**
> As discussed above, in Activating components, you can use an Intent to start activities, services, and broadcast receivers. You can use an Intent by explicitly naming the target component (using the component class name) in the intent. You can also use an implicit intent, which describes the type of action to perform and, optionally, the data upon which you’d like to perform the action. The implicit intent allows the system to find a component on the device that can perform the action and start it. If there are multiple components that can perform the action described by the intent, the user selects which one to use.

```
<manifest ... >
    ...
    <application ... >
        <activity android:name="com.example.project.ComposeEmailActivity">
            <intent-filter>
                <action android:name="android.intent.action.SEND" />
                <data android:type="*/*" />
                <category android:name="android.intent.category.DEFAULT" />
            </intent-filter>
        </activity>
    </application>
</manifest>


```