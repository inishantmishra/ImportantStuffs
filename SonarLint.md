This page provides some additional information about SonarLint and how it can be used.


Description
SonarLint is an IDE extension that helps you detect and fix quality issues as you write code. Like a spell checker, SonarLint squiggles flaws so that they can be fixed before committing code. HBB source control will be integrated with SonarQube on the server side in the near future. This will start to provide feedback on code quality and style as code is committed and scanned. As well as improving the code quality as we develop, SonarLint will reduce the amount of issues detected by SonarQube. Subsequently SonarLint in the IDE can be integrated with SonarQube to scan for the specific rules defined by SonarQube, enabling us to proactively resolve any issues as opposed to waiting from feedback from SonarQube.



Installation
This section provides some information on how to install SonarLint. Installation of SonarLint is through the Visual Studio Marketplace. The steps required are as follows:

1. Open the Visual Studio Marketplace by going to Extensions → Manage Extensions on the main menu.

2. Search for SonarLint in the Marketplace.





3. Click the download button to install SonarLint. (You might need to restart Visual Studio at this point to complete the install.)

4. On restarting Visual Studio SonarLint should now be installed.

Scan Scope
You can change the scope of the scanning performed by analysis tools by doing the following:

1. On the Main Menu, go to Tools → Options

2. Select Text Editor → C# → Advanced

3. Select required scope from Background analysis scope section.





Usage
Initially any code modified as part of a deployment should be reviewed for findings from SonarLint and those findings addressed within the code. Over time we should be able to cover a significant amount of the existing HBB codebase. Issues should be addressed on a priority basis, those that are deemed important should be addressed as soon as possible and those with a lower rating should be addressed over time. In some cases the SonarLint findings will overlap with findings from other analysers so resolving the issue might resolve more than one finding.

