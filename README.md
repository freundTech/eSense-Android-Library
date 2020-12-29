![GitHub Workflow Status](https://img.shields.io/github/workflow/status/freundTech/eSense-Android-Library/Java%20CI) ![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/freundTech/eSense-Android-Library) ![JitPack](https://img.shields.io/jitpack/v/github/freundTech/eSense-Android-Library) ![GitHub](https://img.shields.io/github/license/freundTech/eSense-Android-Library)
# eSense Android Library
Android Studio project containing a light-weight Android library to build mobile apps with [eSense](https://esense.io).

## Requirements
Android 6.0 (API 23) or later.

## Documentation
Find the library documentation at [this link](https://www.esense.io/share/eSense-Android-Library.pdf).

## Builds
Binaries are provided using the Github Package Registry (requires authentication with Github) and [jitpack](https://jitpack.io/#freundTech/eSense-Android-Library) (allows anonymous access)

### JitPack
Add the following to the `repositories` section of your build.gradle:
```groovy
maven { url 'https://jitpack.io' }
```

Then add the following to your dependencies section:
```groovy
implementation 'com.github.freundTech:eSense-Android-Library:1.0.3'
```
### Github Package Registry
Add the following to the `repositories` section of your build.gradle:
```groovy
maven {
    url 'https://maven.pkg.github.com/freundTech/eSense-Android-Library'
    credentials {
        username = "<username>"
        password = "<token>"
    }
}
```
Replace `<username>` with your GitHub username and `<token>` with a private access token you can generate in the GitHub Developer Settings.
If you use GitHub Actions to build your project you can use the values of the `GITHUB_ACTOR` and `GITHUB_TOKEN` secrets instead.

Then add the following to your dependencies section:
```groovy
implementation 'io.esense.esenselib:esenselib:1.0.3'
```


## Credits
Pervasive Systems team at Nokia Bell Labs Cambridge maintains the upstream of this project voluntarily as a community service. Please [get in touch](mailto:info@esense.io) with us to contribute to this effort in advancing the earable computing research.

Forked by Adrian Freund to provide automated builds and small improvements.

CREDITS : [Alessandro Montanari](https://www.cl.cam.ac.uk/~am2266/), [Chulhong Min](https://chulhongmin.com/), [Akhil Mathur](https://akhilmathurs.github.io/), [Fahim Kawsar](https://www.fahim-kawsar.net/), [Adrian Freund](https://adrian.freund.io)
