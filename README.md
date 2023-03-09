# Xamarin.AndroidX.AppCompat.AppCompatResources

## Workaround for https://github.com/xamarin/Xamarin.Forms/issues/15668


- compile this project in Release
- download package version 1.6.0.1 from https://www.nuget.org/packages/Xamarin.AndroidX.AppCompat.AppCompatResources
- extract package
- replace version descriptions for this package from 1.6.0.1 to 1.6.0.2 in .nuspec file
- replace dlls in folder \lib\monoandroid12.0 with output from this project
- zip everything into archive nammed xamarin.androidx.appcompat.appcompatresources.1.6.0.2.nupkg
- store this nuget into your local nuget source
- update target project

Linking and AOT should again work in target project.