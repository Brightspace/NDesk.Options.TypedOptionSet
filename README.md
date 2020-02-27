# NDesk.Options.TypedOptionSet

[![Build status](https://ci.appveyor.com/api/projects/status/l8gaf93jwf78te9c/branch/master?svg=true)](https://ci.appveyor.com/project/Brightspace/ndesk-options-typedoptionset/branch/master)

Some helpers for NDesk.Options

## Releasing

To release a new version of this library, bump the version numbers in [appveyor.yml](appveyor.yml):

```diff
- version: 1.0.0-{branch}-{build}
+ version: 1.0.1-{branch}-{build}
  image: Visual Studio 2017

  environment:
-   ASSEMBLY_FILE_VERSION: 1.0.0
+   ASSEMBLY_FILE_VERSION: 1.0.1

...
```

Make sure to get both spots! Get this change into the `master` branch.

After this, create a [new release](https://github.com/Brightspace/NDesk.Options.TypedOptionSet/releases/new) with the tag name `v1.0.1`. _Don't forget the leading `v`!_

Your package will be published to our AppVeyor account feed and automatically pulled down to [nuget.build.d2l](http://nuget.build.d2l)
