# Voximplant iOS SDK Swift PM

This repository provides the access to the Voximplant iOS SDK for Swift Package Manager. 

Voximplant iOS SDK is distributed as a binary packages (XCFramework) since 2.38.0.

Supported architectures:
- iphoneos: armv7, arm64
- iphonesimulator: i386, x86_64, arm64


## Add Voximplant to your app in Xcode

1. Open the project in Xcode
2. Go to Files > Swift Packages > Add Package Dependency
3. Add this github repository ( .... )
4. Select the SDK version 

More information can be found in [Apple Developer documentation](https://developer.apple.com/documentation/swift_packages/adding_package_dependencies_to_your_app)

## Add Voximplant to your package

To add Voximplant iOS SDK as a dependency of your package, declare it in `dependencies` section of your `Package.swift`

```swift
dependencies: [
    .package(url: "https://github.com/voximplant/ios-sdk-releases.git", .upToNextMinor(from: "2.38.0"))
]
```

## Version notice
Voximplant iOS SDK version does not fully conform to [semantic versioning](https://www.semver.org/). 

The backward compatibility is only garanteed for the patch version. Minor version change may include the API changes or a dependency update.

Check the Voximplant iOS SDK [changelog](https://voximplant.com/docs/references/iossdk/changelog) before selecting a version requirement. It is recommended to use `exact` or `upToNextMinor` requirements.
