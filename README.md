# RandomDataGenerator.Net
This is a simple generator to create random data.

## NuGet

[![NuGet Badge](https://buildstats.info/nuget/RandomDataGenerator.Net)](https://www.nuget.org/packages/RandomDataGenerator.Net)

## Supported Random Data 

- Text Patterns
- Lorum Ipsum Text
- Words
- First/Last Names
- Cities
- Countries
- IP-Addresses (V4 and V6)
- MAC Addresses
- Email Addresses
- Guids
- DateTime
- Integers

## Usage

``` csharp
// Generate a random first name
var randomizerFirstName = RandomizerFactory.GetRandomizer(new FieldOptionsFirstName());
string firstName = randomizerFirstName.Generate();

// Generate a random text (no numbers or special characters allowed)
var randomizerText = RandomizerFactory.GetRandomizer(new FieldOptionsText { UseNumber = false, UseSpecial = false });
string text = randomizerText.Generate();
```

## Copyright

### Referenced files
- http://www.cambiaresearch.com/articles/13/csharp-randomprovider-class
- http://www.codeproject.com/Articles/423229/CsharpRandomStringGenerator

### NuGet dependencies
- NLipsum
- NetLegacySupport.ConcurrentDictionary (only for .NET 2.0 & 3.5)
- LinqBridge (only for .NET 2.0)