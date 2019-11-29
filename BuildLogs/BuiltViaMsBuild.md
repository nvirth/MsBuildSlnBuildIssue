Build log when building the solution via msbuild.exe
====================================================

Using the following command:

    "C:\Program Files (x86)\Microsoft Visual Studio\2019\Professional\MSBuild\Current\bin\MSBuild.exe" MsBuildSlnBuildIssue.sln /p:TreatWarningsAsErrors="true" /m:16


The log
-------

Microsoft (R) Build Engine version 16.3.1+1def00d3d for .NET Framework
Copyright (C) Microsoft Corporation. All rights reserved.

Build started 2019. 11. 29. 13:03:13.
     1>Project "d:\GIT\MsBuildSlnBuildIssue\MsBuildSlnBuildIssue.sln" on node 1 (default targets).
     1>ValidateSolutionConfiguration:
         Building solution configuration "Debug|Any CPU".
     1>Project "d:\GIT\MsBuildSlnBuildIssue\MsBuildSlnBuildIssue.sln" (1) is building "d:\GIT\MsBuildSlnBuildIssue\ParentProject\ParentProject.csproj" (2) on node 1 (default targets).
     2>MyCustomTarget:
          === MyCustomTarget ===
       GenerateTargetFrameworkMonikerAttribute:
       Skipping target "GenerateTargetFrameworkMonikerAttribute" because all output files are up-to-date with respect to the input files.
       CoreCompile:
       Skipping target "CoreCompile" because all output files are up-to-date with respect to the input files.
       CopyFilesToOutputDirectory:
         ParentProject -> d:\GIT\MsBuildSlnBuildIssue\ParentProject\bin\Debug\ParentProject.dll
     2>Done Building Project "d:\GIT\MsBuildSlnBuildIssue\ParentProject\ParentProject.csproj" (default targets).
     1>Project "d:\GIT\MsBuildSlnBuildIssue\MsBuildSlnBuildIssue.sln" (1) is building "d:\GIT\MsBuildSlnBuildIssue\ChildProject\ChildProject.csproj" (3) on node 2 (default targets).
     3>MyCustomTarget:
          === MyCustomTarget ===
       GenerateTargetFrameworkMonikerAttribute:
       Skipping target "GenerateTargetFrameworkMonikerAttribute" because all output files are up-to-date with respect to the input files.
       CoreCompile:
       Skipping target "CoreCompile" because all output files are up-to-date with respect to the input files.
       _CopyFilesMarkedCopyLocal:
         Touching "d:\GIT\MsBuildSlnBuildIssue\ChildProject\obj\Debug\ChildProject.csproj.CopyComplete".
       CopyFilesToOutputDirectory:
         ChildProject -> d:\GIT\MsBuildSlnBuildIssue\ChildProject\bin\Debug\ChildProject.dll
     3>Done Building Project "d:\GIT\MsBuildSlnBuildIssue\ChildProject\ChildProject.csproj" (default targets).
     1>Done Building Project "d:\GIT\MsBuildSlnBuildIssue\MsBuildSlnBuildIssue.sln" (default targets).

Build succeeded.
    0 Warning(s)
    0 Error(s)

Time Elapsed 00:00:00.69
