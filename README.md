# Atomic Android SDK

The Atomic Android SDK is distributed as an AAR, allowing you to integrate an Atomic stream container or single card view into your Android app and present action cards to your end users.

The SDK supports Android API 21 and above.

## Installation

The SDK can be installed as a Gradle dependency or by manually downloading the AAR file.

### Gradle

The SDK is hosted on our public Maven repository. You'll need to add the following repository to your root `build.gradle` file:

```java
allprojects {
    repositories {
      ...
      maven {
        url  "https://downloads.atomic.io/android-sdk/maven"
      }
    }
}
```

Then, add the following to your app’s `build.gradle`

```java
dependencies {
    implementation 'io.atomic.actioncards:aacsdk:<versionNumber>'
}
```

To view a list of available version numbers, see the [`Packages` section](https://github.com/atomic-app/action-cards-android-sdk-releases/packages).

### Manual Installation

If you prefer to manually download and integrate the Atomic SDK into your app, you can download the AAR and POM files from the [`Packages` section](https://github.com/atomic-app/action-cards-android-sdk-releases/packages).

See [our documentation](https://documentation.atomic.io/install/android) for more information.