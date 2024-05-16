# GIM Chat Android SDK Releases

This repository hosts the release artifacts and changelogs for the GIM Chat Android SDK.

## Access

This repository is intended for internal use or access by authorized partners only.  
The SDK is **not open source** and may not be redistributed or modified.

If you are a partner or developer integrating with GIM Chat, please refer to the official partner documentation provided separately.

---

## Introduce

The GIM Chat Android SDK provides the tools necessary to integrate chat functionalities into your Android applications. This repository contains only the release binaries and changelogs for version tracking and distribution.

---

## Quick Start

### Root Gradle Configuration

#### Gradle 6.8 or higher

Add the following to your `settings.gradle` file:
```
dependencyResolutionManagement {
    repositories {
        ...
        maven {
            url = uri("https://maven.pkg.github.com/gamania-beanfun/gim-chat-sdk-android")
            credentials {
                username = "your GitHub username"
                password = "your GitHub token"
            }
        }
    }
}
```

#### Gradle 6.7 or lower

Add the following to your root `build.gradle` file:
```
allprojects {
    repositories {
        ...
        maven {
            url = uri("https://maven.pkg.github.com/gamania-beanfun/gim-chat-sdk-android")
            credentials {
                username = "your GitHub username"
                password = "your GitHub token"
            }
        }
    }
}
```

### Install the SDK

Add the following to your module's build.gradle.kts or build.gradle:

```
dependencies {
    implementation("com.gamania.gim:gim-chat:<latest-version>")
}
```