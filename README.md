# Penetration-testing-practice
In this repository, you will find screenshots and reports of my practice with penetration's testing. 

Instructions:

You've been provided full access to the network and are getting ping responses from the CEO’s workstation.


Perform a service and version scan using Nmap to determine which services are up and running:


Run the Nmap command that performs a service and version scan against the target.

![screenshot 1](https://user-images.githubusercontent.com/81331968/117705753-ab72de80-b189-11eb-8daa-bc66c6d6e712.png)

From the previous step, we see that the Icecast service is running. Let's start by attacking that service. Search for any Icecast exploits:


Run the SearchSploit commands to show available Icecast exploits.

command: searchsploit icecast

Now that we know which exploits are available to us, let's start Metasploit:

Run the command that starts Metasploit:

command: msfconsole


Search for the Icecast module and load it for use.

Run the command to search for the Icecast module:
![screenshot 6 msf5](https://user-images.githubusercontent.com/81331968/117706186-37850600-b18a-11eb-848c-dd5ac11d8d86.png)

                
Note: Instead of copying the entire path to the module, you can use the number in front of it.

Set the RHOST to the target machine.

Run the command that sets the RHOST:

Command: set rhosts 192.168.0.20

Run the Icecast exploit.

Run the command that runs the Icecast exploit.

command: exploit

Run the command that performs a search for the secretfile.txt on the target.

command: search -f secretfile*.txt

Download drinks.recipe.txt

![screenshot 3](https://user-images.githubusercontent.com/81331968/117707604-f8f04b00-b18b-11eb-8315-68e2fb3260ca.png)



You should now have a Meterpreter session open.

Run the command to performs a search for the recipe.txt on the target:


![screenshot 2 meterpreter](https://user-images.githubusercontent.com/81331968/117706919-1f61b680-b18b-11eb-8853-12bf9a25a4a4.png)


![screenshot 4](https://user-images.githubusercontent.com/81331968/117707011-3dc7b200-b18b-11eb-966e-f4f72834c368.png)









