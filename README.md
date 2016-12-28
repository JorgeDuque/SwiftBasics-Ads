# SwiftBasics: Ads
Ads basic functionalities

##Features
- Google Ad Banner
- Fullscreen Ad

##How to use it?
###Step 1. Set up Firebase
- Create a new project on Firebase
- Select iOS and paste our App's bundle identifier
- GoogleService-info-plist file will be downloaded. Add this file to our project in XCode.

###Step 2. Terminal
- Go to our project's directory
- Initialize pod in terminal:
```
pod init
```
- Open recently created podfile in XCode
- Edit pod file to look like this:
```
platform :ios, '9.0'

target 'Admob' do
  # Comment the next line if you're not using Swift and don't want to use dynamic frameworks
  use_frameworks!

pod 'Firebase/Core'
pod 'Firebase/AdMob'

end
```
- Save pod file changes
- Install pods using terminal:
```
pod install
```
###Step 3. App Delegate
- import Firebase and GoogleMobileAds in our project's Appdelegate file 
```
import Firebase
import GoogleMobileAds
```
- in didFinishLaunchingWithOptions method, add the following line:
```
FIRApp.configure()
```
