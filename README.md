# Test.Integration.Oldest.MsBuild.VbNet

This repository contains the integration tests for the nBuildKit.MsBuild, testing the oldest supported version of the configuration scripts against a VB.NET Visual Studio solution


## Building

In order to start the build execute the following commandline:

    msbuild entrypoint.msbuild /t:build /p:NBuildKitMinimumVersion=<MIN_VERSION> /p:NBuildKitMaximumVersion=<MAX_VERSION> /p:LocalNuGetRepository=<LOCAL_REPO>

In this commandline the provide:

* **<MIN_VERSION>** The minimum version of nBuildKit against which the test should run
* **<MAX_VERSION>** The maximum version of nBuildKIT against which the test should run.
* **<LOCAL_REPO>** The NuGet feed for a local NuGet repository. It is expected that the version of nBuildKit which should be tested is in this repository.
