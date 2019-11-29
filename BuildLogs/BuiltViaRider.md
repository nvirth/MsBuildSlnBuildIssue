Build log when building the solution in JetBrains Rider IDE
===========================================================

The log
-------

Build with surface heuristics started at 13:00:11
Use build tool: C:\Program Files (x86)\Microsoft Visual Studio\2019\Professional\MSBuild\Current\Bin\MSBuild.exe
CONSOLE: Microsoft (R) Build Engine version 16.3.1+1def00d3d for .NET Framework
CONSOLE: Copyright (C) Microsoft Corporation. All rights reserved.
CONSOLE: Build started 2019. 11. 29. 13:00:11.
0>------- Started building project: ParentProject
0> === MyCustomTarget ===
0>Skipping target "GenerateTargetFrameworkMonikerAttribute" because all output files are up-to-date with respect to the input files.
0>C:\Program Files (x86)\Microsoft Visual Studio\2019\Professional\MSBuild\Current\Bin\Roslyn\csc.exe /noconfig /nowarn:1701,1702,2008 /nostdlib+ /platform:AnyCPU /errorreport:prompt /warn:4 /define:DEBUG;TRACE /errorendlocation /preferreduilang:en-US /highentropyva+ /reference:"C:\Program Files (x86)\Reference Assemblies\Microsoft\Framework\.NETFramework\v4.8\mscorlib.dll" /reference:"C:\Program Files (x86)\Reference Assemblies\Microsoft\Framework\.NETFramework\v4.8\System.Core.dll" /reference:"C:\Program Files (x86)\Reference Assemblies\Microsoft\Framework\.NETFramework\v4.8\System.Data.dll" /reference:"C:\Program Files (x86)\Reference Assemblies\Microsoft\Framework\.NETFramework\v4.8\System.dll" /reference:"C:\Program Files (x86)\Reference Assemblies\Microsoft\Framework\.NETFramework\v4.8\System.Xml.dll" /debug+ /debug:full /filealign:512 /optimize- /out:obj\Debug\ParentProject.dll /ruleset:"C:\Program Files (x86)\Microsoft Visual Studio\2019\Professional\Team Tools\Static Analysis Tools\\Rule Sets\MinimumRecommendedRules.ruleset" /subsystemversion:6.00 /target:library /utf8output /langversion:7.3 Class1.cs Properties\AssemblyInfo.cs "C:\Users\norbertvirth\AppData\Local\Temp\.NETFramework,Version=v4.8.AssemblyAttributes.cs"
0>Using shared compilation with compiler from directory: C:\Program Files (x86)\Microsoft Visual Studio\2019\Professional\MSBuild\Current\Bin\Roslyn
0>Copying file from "D:\GIT\MsBuildSlnBuildIssue\ParentProject\obj\Debug\ParentProject.dll" to "D:\GIT\MsBuildSlnBuildIssue\ParentProject\bin\Debug\ParentProject.dll".
0>ParentProject -> D:\GIT\MsBuildSlnBuildIssue\ParentProject\bin\Debug\ParentProject.dll
0>Copying file from "D:\GIT\MsBuildSlnBuildIssue\ParentProject\obj\Debug\ParentProject.pdb" to "D:\GIT\MsBuildSlnBuildIssue\ParentProject\bin\Debug\ParentProject.pdb".
0>------- Finished building project: ParentProject. Succeeded: True. Errors: 0. Warnings: 0
1>------- Started building project: ChildProject
1> === MyCustomTarget ===
1>Skipping target "GenerateTargetFrameworkMonikerAttribute" because all output files are up-to-date with respect to the input files.
1>C:\Program Files (x86)\Microsoft Visual Studio\2019\Professional\MSBuild\Current\Bin\Roslyn\csc.exe /noconfig /nowarn:1701,1702,2008 /nostdlib+ /platform:AnyCPU /errorreport:prompt /warn:4 /define:DEBUG;TRACE /errorendlocation /preferreduilang:en-US /highentropyva+ /reference:"C:\Program Files (x86)\Reference Assemblies\Microsoft\Framework\.NETFramework\v4.8\mscorlib.dll" /reference:D:\GIT\MsBuildSlnBuildIssue\ParentProject\bin\Debug\ParentProject.dll /reference:"C:\Program Files (x86)\Reference Assemblies\Microsoft\Framework\.NETFramework\v4.8\System.Core.dll" /reference:"C:\Program Files (x86)\Reference Assemblies\Microsoft\Framework\.NETFramework\v4.8\System.Data.dll" /reference:"C:\Program Files (x86)\Reference Assemblies\Microsoft\Framework\.NETFramework\v4.8\System.dll" /reference:"C:\Program Files (x86)\Reference Assemblies\Microsoft\Framework\.NETFramework\v4.8\System.Xml.dll" /debug+ /debug:full /filealign:512 /optimize- /out:obj\Debug\ChildProject.dll /ruleset:"C:\Program Files (x86)\Microsoft Visual Studio\2019\Professional\Team Tools\Static Analysis Tools\\Rule Sets\MinimumRecommendedRules.ruleset" /subsystemversion:6.00 /target:library /utf8output /langversion:7.3 Class1.cs Properties\AssemblyInfo.cs "C:\Users\norbertvirth\AppData\Local\Temp\.NETFramework,Version=v4.8.AssemblyAttributes.cs"
1>Using shared compilation with compiler from directory: C:\Program Files (x86)\Microsoft Visual Studio\2019\Professional\MSBuild\Current\Bin\Roslyn
1>Copying file from "D:\GIT\MsBuildSlnBuildIssue\ParentProject\bin\Debug\ParentProject.dll" to "D:\GIT\MsBuildSlnBuildIssue\ChildProject\bin\Debug\ParentProject.dll".
1>Copying file from "D:\GIT\MsBuildSlnBuildIssue\ParentProject\bin\Debug\ParentProject.pdb" to "D:\GIT\MsBuildSlnBuildIssue\ChildProject\bin\Debug\ParentProject.pdb".
1>Creating "D:\GIT\MsBuildSlnBuildIssue\ChildProject\obj\Debug\ChildProject.csproj.CopyComplete" because "AlwaysCreate" was specified.
1>Copying file from "D:\GIT\MsBuildSlnBuildIssue\ChildProject\obj\Debug\ChildProject.dll" to "D:\GIT\MsBuildSlnBuildIssue\ChildProject\bin\Debug\ChildProject.dll".
1>ChildProject -> D:\GIT\MsBuildSlnBuildIssue\ChildProject\bin\Debug\ChildProject.dll
1>Copying file from "D:\GIT\MsBuildSlnBuildIssue\ChildProject\obj\Debug\ChildProject.pdb" to "D:\GIT\MsBuildSlnBuildIssue\ChildProject\bin\Debug\ChildProject.pdb".
1>------- Finished building project: ChildProject. Succeeded: True. Errors: 0. Warnings: 0
Build completed in 00:00:01.772
Build succeeded at 13:00:12
