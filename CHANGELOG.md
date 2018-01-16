## Version 4.19.0 (December 15, 2017)
- Bug fixes.
- The MoPub Unity Plugin is now compatible with version 4.19.0 of the MoPub Android SDK and version 4.19.0 of the MoPub iOS SDK.

## Version 4.18.0 (November 3, 2017)
- Improved documentation for third-party SDKs.
- Added ability to change log level for iOS (Android already logs everything). See [`MoPubBinding.setSDKLogLevel(MoPubLogLevel)`](https://github.com/mopub/mopub-unity-sdk/blob/79e34235386b751054eeb70dfda2feda84f1762d/unity/MoPubUnityPlugin/Assets/MoPub/Internal/MoPubBinding.cs#L76)
- Several third-party networks were upgraded.
- Cleaned up errors for non-mobile platforms.
- The MoPub Unity Plugin is now compatible with version 4.18.0 of the MoPub Android SDK and version 4.18.0 of the MoPub iOS SDK.

## Version 4.17.0 (September 28, 2017)
- Rewarded Ads can now send up optional custom data through the server completion url. See [`MoPub.showRewardedVideo (string, string)`](https://github.com/mopub/mopub-unity-sdk/blob/e0697d2f03c972de70d94aac39d5990bb30389af/unity/MoPubUnityPlugin/Assets/MoPub/MoPub.cs#L348).
- Several improvements to the Sample Scene, including better layout, error cleanup, more details on failures, and showing the versions of the running Plugin and SDK.
- The MoPub Unity Plugin is now compatible with version 4.17.0 of the MoPub Android SDK and version 4.17.0 of the MoPub iOS SDK.

## Version 4.16.1 (September 8, 2017)
- The MoPub Unity Plugin is now fully open source! Please see the [readme](https://github.com/mopub/mopub-unity-sdk/blob/master/README.md) for details and building instructions.
- This release does not change the SDK compatibility; the Plugin is still compatible with version 4.16.1 of the MoPub Android SDK and version 4.16.0 of the MoPub iOS SDK.

## Version 4.16.0 (August 30, 2017)
- The MoPub Unity Plugin is now compatible with version 4.16.1 of the MoPub Android SDK and version 4.16.0 of the MoPub iOS SDK.
- Rewarded Videos have a new init method. See [`MoPub.initializeRewardedVideo(MoPubRewardedNetwork[])`](https://github.com/mopub/mopub-unity-sdk/blob/e0697d2f03c972de70d94aac39d5990bb30389af/unity/MoPubUnityPlugin/Assets/MoPub/MoPub.cs#L306). Pass in a list of networks to initialize, and MoPub will initialize those networks with the settings from the previous ad request, persisted across app close.

## Version 4.15.0 (June 29, 2017)
- The MoPub Unity Plugin is now compatible with version 4.15.0 of the MoPub SDK.
- The MoPub Unity Plugin is now available on GitHub.

## Version 4.14.0
- The MoPub Unity Plugin is now compatible with version 4.14.0 of the MoPub SDK.

## Version 4.13.0
- The MoPub Unity Plugin is now compatible with version 4.13.0 of the MoPub SDK.

## Version 4.12.0
- The MoPub Unity Plugin is now compatible with version 4.12.0 of the MoPub SDK.

## Version 4.11.0
- Minor bug fixes

## Version 4.10.0
#### The Mopub Unity Plugin 4.10.0 introduces Modularized SDK for Android
Starting in the 4.10.0 release, we want to bring the modular SDK support to Android, so you choose to include specific ad formats and decrease overall SDK footprint in your app. For instance, if a publisher only wishes to integrate with MoPub’s interstitials and rewarded videos, you no longer need to include the banner SDK module to your project. For taking advantage of the new modular features, download the Android Unity package 4.10.0 from the "Getting Started" section and choose the modules of your choice from [`Assets/Plugins/Android/mopub/libs/`](https://github.com/mopub/mopub-unity-sdk/tree/master/unity/MoPubUnityPlugin/Assets/Plugins/Android/mopub/libs) directory:

- mopub-unity-plugins.jar: Unity plugins supporting banner, interstitial, and/or rewarded video (required)
- mopub-sdk-base.jar: base module for MoPub Android SDK (required)
- mopub-sdk-banner.jar: banner SDK module (optional)
- mopub-sdk-interstitial.jar: interstitial SDK module (optional, but required for rewarded video)
- mopub-sdk-rewardedvideo.jar: rewarded video SDK module (optional)

Note: interstitials is a prerequisite for rewarded videos, so one cannot integrate with rewarded videos without the interstitials SDK module.

## Version 4.9.0
- Support of multiple plugins for multiple banners, interstitials, and rewarded videos: one plugin per adunit
- Compatibility with MoPub's SDK 4.9.0 (modular SDK)
- Please note that there is no backward compatibility with SDK versions earlier than 4.9.0. For earlier versions, please check our reference documentation.
