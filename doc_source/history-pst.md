# Document History<a name="history-pst"></a>

This topic describes significant changes to the documentation for the AWS Tools for PowerShell\.

 *Last documentation update: September 17, 2018* 

We also update the documentation periodically in response to customer feedback\. To send feedback about a topic, use the feedback buttons next to "Did this page help you?" located at the bottom of each page\.

For additional information about changes and updates to the Tools for Windows PowerShell, see the [release notes](https://aws.amazon.com/releasenotes/PowerShell)\.

## AWS Tools for PowerShell 3\.3\.343\.0<a name="pstools-release-v3-3-343-0"></a>

 *Release Date:* 2018\-09\-11

 *Summary of Changes* 
+ Added information to the [Using the AWS Tools for PowerShell](https://docs.aws.amazon.com/powershell/latest/userguide/pstools-using.html) section introducing the AWS Lambda Tools for PowerShell for PowerShell Core developers to build AWS Lambda functions\.

## AWS Tools for Windows PowerShell 3\.1\.31\.0<a name="twplong-3-1-31-0"></a>

 *Release Date:* 2015\-12\-01

 *Summary of Changes* 
+ Added information to the [Getting Started](https://docs.aws.amazon.com/powershell/latest/userguide/pstools-getting-started.html) section about new cmdlets that use Security Assertion Markup Language \(SAML\) to support configuring federated identity for users\.

## AWS Tools for Windows PowerShell 2\.3\.19<a name="pstools-release-v2-3-19"></a>

 *Release Date:* 2015\-02\-05

 *Summary of Changes* 
+ Added information to the [Cmdlets Discovery and Aliases](https://docs.aws.amazon.com/powershell/latest/userguide/pstools-discovery-aliases.html) section about the new `Get-AWSCmdletName` cmdlet that can help users more easily find their desired AWS cmdlets\.

## AWS Tools for Windows PowerShell 1\.1\.1\.0<a name="pstools-release-v1-1-1-0"></a>

 *Release Date:* 2013\-05\-15

 *Summary of Changes* 
+ Collection output from cmdlets is always enumerated to the PowerShell pipeline
+ Automatic support for pageable service calls
+ New $AWSHistory shell variable collects service responses and optionally service requests
+ AWSRegion instances use Region field instead of SystemName to aid pipelining
+ Remove\-S3Bucket supports a \-DeleteObjects switch option
+ Fixed usability issue with Set\-AWSCredentials
+ Initialize\-AWSDefaults reports from where it obtained credentials and region data
+ Stop\-EC2Instance accepts Amazon\.EC2\.Model\.Reservation instances as input
+ Generic List<T> parameter types replaced with array types \(T\[\]\)
+ Cmdlets that delete or terminate resources prompt for confirmation prior to deletion
+ Write\-S3Object supports in\-line text content to upload to Amazon S3

## AWS Tools for Windows PowerShell 1\.0\.1\.0<a name="pstools-release-v1-0-1-0"></a>

 *Release Date:* 2012\-12\-21

The install location of the Tools for Windows PowerShell module has changed so that environments using Windows PowerShell version 3 can take advantage of auto\-loading\.
+ The module and supporting files are now installed to an *AWSPowerShell* subfolder beneath *AWS ToolsPowerShell*\. Files from previous versions that exist in the *AWS ToolsPowerShell* folder are automatically removed by the installer\.
+ The `PSModulePath` for Windows PowerShell \(all versions\) is updated in this release to contain the parent folder of the module \(*AWS ToolsPowerShell*\)\.
+ For systems with Windows PowerShell version 2, the Start Menu shortcut **Amazon Web ServicesWindows PowerShell for AWS** is updated to import the module from the new location and then run `Initialize-AWSDefaults`\.
+ For systems with Windows PowerShell version 3, the Start Menu shortcut **Amazon Web ServicesWindows PowerShell for AWS** is updated to remove the `Import-Module` command, leaving just `Initialize-AWSDefaults`\.
+ If you edited your PowerShell profile to perform an `Import-Module` of the `AWSPowerShell.psd1` file, you will need to update it to point to the file's new location \(or, if using PowerShell version 3, remove the `Import-Module` statement as it is no longer needed\)\.

As a result of these changes, the Tools for Windows PowerShell module is now listed as an available module when executing `Get-Module -ListAvailable`\. In addition, for users of Windows PowerShell version 3, the execution of any cmdlet exported by the module will automatically load the module in the current PowerShell shell without needing to use `Import-Module` first\. This enables interactive use of the cmdlets on a system with an execution policy that disallows script execution\.

## AWS Tools for Windows PowerShell 1\.0\.0\.0<a name="pstools-release-v1-0-0-0"></a>

 *Release Date:* 2012\-12\-06

Initial release