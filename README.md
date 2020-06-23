# KITTO365Tool
KITT - An Open Source PowerShell O365 Business Email Compromise Investigation Tool


Welcome to KITT - This is a tool designed to make working O365 Business Email Compromise investigations easier and more efficient for DFIR and SOC analysts by pairing the power of PowerShell cmdlets with the ease of use of a GUI.
KITT was built using Sapien's PowerShell Studio. Dates are set to UTC. 

Powershell Cmdlet limitations limit the pulling of AzureAD SignIn Logs to 30 days, and Message Trace Logs to 10 days. By default, the timepickers are set to those values. 

---------------------------------------------------------------------------	
BEFORE YOU BEGIN:
1. You'll need to install the following PS modules in order to run this:
	1. AzureADPreview
	2. ExchangeOnlineManagement
	3. MSOnline
		
2. Please search for "CHANGE_ME" to find two values you will need to change. These are: 
	1. You'll need to add your email address after Connect-ExchangeOnline -UserPrincipalName.  
	2. You'll need to change the variable $script:DomainName to be your domain. That will allow the script to get the password policy for your domain to calculate the password expiration date for a user. 
	
---------------------------------------------------------------------------
Feedback can be left on my Github or sent to the following contact details: 
1. @IntrepidTechie on Twitter
2. intrepidtechie@gmail.com
---------------------------------------------------------------------------
Please feel free to contribute to this tool by fixing bugs or providing feedback. I'm not a developer by trade, and would gladly accept feedback from seasoned devs/PowerShell Gurus.
Special thanks to my wonderful wife Kait for constantly supporting me. 
Dedicated to @HumanMalware. RIP bro, you are gone too soon. 
