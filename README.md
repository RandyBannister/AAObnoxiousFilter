# Table of Contents

##Description


AAObnoxiousFilter is a profanity filter for images written in CoreML and Swift. Its a lightweight framework that can detect the inappropriation in UIImage with a single line of code.


<div id='section-id-16'/>

##Demonstration



To run the example project, clone the repo, and run `pod install` from the Example directory first.


<div id='section-id-26'/>

##Requirements

- iOS 11.0+
- Xcode 10.0+
- Swift 4.2+

<div id='section-id-32'/>

# Installation

`AAObnoxiousFilter` can be installed using CocoaPods, Carthage, or manually.


<div id='section-id-37'/>

##CocoaPods

`AAObnoxiousFilter` is available through [CocoaPods](http://cocoapods.org). To install CocoaPods, run:

`$ gem install cocoapods`

Then create a Podfile with the following contents:

```
source 'https://github.com/CocoaPods/Specs.git'
platform :ios, '11.0'
use_frameworks!

target '<Your Target Name>' do
pod 'AAObnoxiousFilter'
end

```

Finally, run the following command to install it:
```
$ pod install
```



<div id='section-id-63'/>

##Carthage

To install Carthage, run (using Homebrew):
```
$ brew update
$ brew install carthage
```
Then add the following line to your Cartfile:

```
github "EngrAhsanAli/AAObnoxiousFilter" "master"
```

Then import the library in all files where you use it:
```swift
import AAObnoxiousFilter
```


<div id='section-id-82'/>

##Manual Installation

If you prefer not to use either of the above mentioned dependency managers, you can integrate `AAObnoxiousFilter` into your project manually by adding the files contained in the Classes folder to your project.


<div id='section-id-87'/>

#Getting Started
----------

<div id='section-id-90'/>

##Detect the Image

```swift
if let prediction = image.predictImage() {
    // prediction if greater than 0.5, the image will have inappropriate look
}
else {
    // Exception in any other case if the Image is not valid to predict
}
```

<div id='section-id-156'/>

#Contributions & License


Pull requests are welcome! The best contributions will consist of substitutions or configurations for classes/methods known to block the main thread during a typical app lifecycle.

I would love to know if you are using `AAObnoxiousFilter` in your app, send an email to [Engr. Ahsan Ali](mailto:michael.b.albanese@gmail.com)
