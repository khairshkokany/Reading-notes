# Espresso


![images](https://koenig-media.raywenderlich.com/uploads/2019/02/UITestingEspresso-feature.png)

``` @Test
public void greeterSaysHello() {
    onView(withId(R.id.name_field)).perform(typeText("Steve"));
    onView(withId(R.id.greet_button)).perform(click());
    onView(withText("Hello Steve!")).check(matches(isDisplayed()));
}
```
- Espresso is a testing framework for Android to make it easy to write reliable user interface tests.
- Espresso is targeted at developers, who believe that automated testing is an integral part of the development lifecycle.
- The Espresso Test Recorder tool lets you create UI tests for your app without writing any test code.
- Espresso Test Recorder then takes the saved recording and automatically generates a corresponding UI test that you can run to test your app.

- Espresso tests consist of two primary components:
  - UI interactions and assertions on View elements.
    - UI interactions include tap and type actions that a person may use to interact with your app.
    - Assertions verify the existence or contents of visual elements on the screen.

- Assertions verify the existence or contents of a View element through three main types:

  - text is: Checks the text content of the selected View element
  - exists: Checks that the View element is present in the current View hierarchy visible on the screen
  - does not exist: Checks that the View element is not present in the current View hierarchy