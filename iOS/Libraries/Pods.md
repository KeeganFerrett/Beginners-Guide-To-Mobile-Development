# Cocoapods

## Setting up a Podfile
Change to your project directory and run the following command

```bash
  pod init
```

This will produce a new Podefile similar to this:

```Ruby
# Uncomment the next line to define a global platform for your project
# platform :ios, '9.0'

target '<project>' do
  # Comment the next line if you're not using Swift and don't want to use dynamic frameworks
  use_frameworks!

  # Pods for <project>
  # pod '<pod name>'

end
```

Since Pods are just ruby gems, Podfiles are written in ruby.

Uncomment the second line `# platform :ios, '9.0'` as instructed. This defines a
global 'variable' which is used when retrieving pods

## Finding Pods

Pods can be searched for and viewed [here](https://cocoapods.org). Once the desired
pod is found, it can be added to the Podfile to be installed

## Installing Pods

To install you selected pods, simpily run
```bash
  pod install
```
This will install all pods in the the `Pods/` folder. Note that this command
installs all Pods all over again.

## Updating Pods

Simply run
`pod install` or `pod update` to update all saved pods

## Using pods

You will notice that a new file `<project>.xcworkspace` has been created. In order
to use your Pods, you will need to open all projects using this file. After that
it is as simple as importing the library.

```Swift
  import <Pod>
```
