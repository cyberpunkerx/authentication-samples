#spark-auth-sample-android

Calls to Spark APIs require an access token in the authorization header. This simple Android app demonstrates getting an access token.  Use it to get started with the Spark APIs.

<b>Spark APIs are current in beta: [Request access](https://spark.autodesk.com/developers/).</b>

##Prerequisites for running this app

* The Android Studio development environment.
* The [Spark Android SDK](https://github.com/spark3dp/spark-android-SDK) installed in Android Studio.
* To use the Spark Android SDK you must first <i>add an app</i> on the [Spark Developer’s Portal](https://spark.autodesk.com/developers/myApps) and save the app key and app secret Spark generates. For more information see [the tutorial](https://spark.autodesk.com/developers/reference/introduction/tutorials/register-an-app).

##Running the app

1) Download the sample apps from https://github.com/spark3dp/authentication-samples.<br>
2) In the Android Studio <i>Quick Start</i> menu, select <i>Open an existing Android Studio project</i>. <br>
3) Locate the downloaded authentication samples and select the Android folder. <br>In the Android/SparkSample/src/main/java/com/autodesk/spark/sdk/example/SelectionActivity.java file, go to line 39:  
```Java
Spark.init(this,key,secret,Constants.SPARK_ENV_TYPE_SANDBOX);
```
Replace "key" and "secret" with the app key and app secret allocated when you registered your app.<br>
To run the sample in production (not in the Sandbox) change the SPARK_ENV_TYPE_SANDBOX to SPARK_ENV_TYPE_PRODUCTION.<br>
4) In the Android/SparkSample/src/main/res/values/strings.xml file set the <b>SPARK_API_KEY</b> and <b>SPARK_API_SECRET</b> strings to the value of the API key and secret you were allocated when you registered your app.<br>
5) Click the <b>Run</b> button on Android Studio.<br>

For more information about authentication see our [Authentication API](https://spark.autodesk.com/developers/reference/authentication).
