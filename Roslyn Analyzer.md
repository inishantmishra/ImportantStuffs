
This page provides some additional information about the Rosalyn Analyzers, how to enable them and usage.

Description
Roslyn analyzers analyze your code for style, quality and maintainability, design and other issues. The documentation for Roslyn Analyzers can be found at docs.microsoft.com/visualstudio/code-quality/roslyn-analyzers-overview.

Microsoft created a set of analyzers called Microsoft.CodeAnalysis.FxCopAnalyzers that contains the most important "FxCop" rules from static code analysis, converted to Roslyn analyzers. These analyzers check your code for security, performance, and design issues, among others. The documentation for FxCop analyzers in Visual Studio can be found at docs.microsoft.com/visualstudio/code-quality/install-fxcop-analyzers.

Installation
Visual Studio includes a core set of .NET Compiler Platform (Roslyn) analyzers. These analyzers are always on. You can install additional analyzers either as NuGet packages, or as Visual Studio extensions in VSIX files. At the very least you should install the following Analyzer:

Microsoft.CodeAnalysis.FxCopAnalyzers


The Microsoft.CodeAnalysis.FxCopAnalyzers ca be installed as a NuGet package if necessary.

Usage
There is some overlap between the Roslyn Analyzers and SonarLint so resolving issues highlighted might resolve issues highlighted by another analyser. Similar to SonarLint, initially any code modified as part of a deployment should be reviewed for findings from the Roslyn Analysers and those findings addressed within the code. Over time we should be able to cover a significant amount of the existing HBB codebase. Issues should be addressed on a priority basis, those that are deemed important should be addressed as soon as possible and those with a lower rating should be addressed over time.
