# Atomic Android SDK

Android integration with the Atomic Platform is available as an installable SDK that you can embed in your existing Android apps. The SDK supports Android API 21 and above.

The SDK is hosted privately in this Github repository. To consume the SDK, add the following repository to your root `build.gradle`:

**Note:** The password in your Gradle file is your Github personal access token, rather than your login password. To obtain a personal access token, [follow these instructions](https://docs.github.com/en/packages/learn-github-packages/about-github-packages#authenticating-to-github-packages).

```
allprojects {
    repositories {
      ...
      maven {
        url  "https://maven.pkg.github.com/atomic-app/action-cards-android-sdk-releases"
        credentials {
           username '<USERNAME>'
           password '<PERSONAL_ACCESS_TOKEN>'
        }
      }
    }
}
```

Then, add the following to your app’s `build.gradle`:

```java
dependencies {
    implementation 'io.atomic.actioncards:aacsdk:<versionNumber>'
}
```

To view a list of available version numbers, see the [`Packages` section](https://github.com/atomic-app/action-cards-android-sdk-releases/packages).

If you prefer to manually download and integrate the Atomic SDK into your app, you can download the AAR and POM files for our SDK releases from the [`Packages` section](https://github.com/atomic-app/action-cards-android-sdk-releases/packages).