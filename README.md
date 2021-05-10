# Penetration-testing-practice
In this repository, you will find screenshots and reports of my practice with penetration's testing. 

Instructions:

You've been provided full access to the network and are getting ping responses from the CEO’s workstation.


Perform a service and version scan using Nmap to determine which services are up and running:


Run the Nmap command that performs a service and version scan against the target.

From the previous step, we see that the Icecast service is running. Let's start by attacking that service. Search for any Icecast exploits:


Run the SearchSploit commands to show available Icecast exploits.

Now that we know which exploits are available to us, let's start Metasploit:

Run the command that starts Metasploit:

Search for the Icecast module and load it for use.

Run the command to search for the Icecast module:

                
Note: Instead of copying the entire path to the module, you can use the number in front of it.

Set the RHOST to the target machine.

Run the command that sets the RHOST:

Run the Icecast exploit.

Run the command that runs the Icecast exploit.

Run the command that performs a search for the secretfile.txt on the target.

You should now have a Meterpreter session open.

Run the command to performs a search for the recipe.txt on the target:









