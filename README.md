# WinUIPluginApp
An application that attempts to load plugin assemblies and controls at runtime.

Throws Microsoft.UI.Xaml.Markup.XamlParseException when attempting to instantiate a plugin control.

```
Exception thrown: 'Microsoft.UI.Xaml.Markup.XamlParseException' in WinRT.Runtime.dll
WinRT information: Cannot locate resource from 'ms-appx:///Plugin/PluginRoot.xaml'.
XAML parsing failed.
```

## Build Instructions
1. Configure for x64
2. Build and deploy the Package project
3. Build the Plugin project (this will also copy its output to the AppX folder in a post build step)
