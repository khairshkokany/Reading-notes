
# Location

![images](https://www.lifewire.com/thmb/6DrtO40qnoND20afLabJ8MHUN4w=/1614x1105/filters:fill(auto,1)/Maplocation_-5a492a4e482c52003601ea25.jpg)

- Using the Google Play services location APIs, your app can request the last known location of the user's device. In most cases, you are interested in the user's current location, which is usually equivalent to the last known location of the device.

- The fused location provider is one of the location APIs in Google Play services. It manages the underlying location technology and provides a simple API so that you can specify requirements at a high level, like high accuracy or low power. It also optimizes the device's use of battery power.


- Set up Google Play services
  - To access the fused location provider, your app's development project must include Google Play services.
- Specify app permissions
  - Apps whose features use location services must request location permissions, depending on the use cases of those features.
- Create location services client
- Get the last known location
- Choose the best location estimate