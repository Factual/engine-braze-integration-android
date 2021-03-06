# Example

## Setup

### Add API Keys

**(1)** Locate your Factual Engine API Key from the [Factual Engine Dashboard](https://engine.factual.com/garage)

![Dashboard image](./images/apikey.png)

**(2)** Add your Factual Location Engine API Key in [Configuration.java](https://github.com/Factual/engine-braze-integration-android/tree/master/example/src/main/java/com/factual/engine/braze/Configuration.java#L5)

**(3)** Locate your Braze API Key for your app from the [Braze Dashboard](https://dashboard.braze.com) in **Developer Console** under the **APP SETTINGS** tab.  Go to **Identification** and use the API Key listed for your app.

**(4)** Add your Braze SDK API Key to [appboy.xml](https://github.com/Factual/engine-braze-integration-android/tree/master/example/src/main/res/values/appboy.xml#L3)

**(5)** Determine your [Braze Endpoint](https://www.braze.com/docs/user_guide/administrative/access_braze/sdk_endpoints/) and add it to [appboy.xml](https://github.com/Factual/engine-braze-integration-android/tree/master/example/src/main/res/values/appboy.xml#L4)

**(5)** In [Configuration.java](https://github.com/Factual/engine-braze-integration-android/tree/master/example/src/main/java/com/factual/engine/braze/Configuration.java) replace `"Your Braze User ID here"` and `"Your Braze User Email here"` to a test user id and user email which you can use to look up on Braze to ensure the data is being sent.

### Enable Push Notifications

The example app is setup to send a push notification using [Firebase](https://firebase.google.com/).  To view how to configure Braze's push notifications [click here](https://www.braze.com/docs/developer_guide/platform_integration_guides/android/push_notifications/integration/).  Add your Cloud Messaging Sender ID to [appboy.xml](https://github.com/Factual/engine-braze-integration-android/tree/master/example/src/main/res/values/appboy.xml#L5)

### Explore

From here you can setup a Braze Campaign to trigger actions based on Engine custom events. [See here](https://github.com/Factual/engine-braze-integration#example) for an example of sending a push notification for when a user is near a coffee shop.

### Testing

If you'd like to test the integration, an example test is given. To run the test, fill out your information in [StubConfiguration.java](https://github.com/Factual/engine-braze-integration-android/tree/master/example/src/androidTest/java/com/factual/engine/braze/StubConfiguration.java).
