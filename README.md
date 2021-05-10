# Penetration-testing-practice
In this repository, you will find screenshots and reports of my practice with penetration testing. 

Instructions:

You've been provided full access to the network and are getting ping responses from the CEO’s workstation.


Perform a service and version scan using Nmap to determine which services are up and running:


Run the Nmap command that performs a service and version scan against the target.

![screenshot 1](https://user-images.githubusercontent.com/81331968/117705753-ab72de80-b189-11eb-8daa-bc66c6d6e712.png)

From the previous step, we see that the Icecast service is running. Let's start by attacking that service. Search for any Icecast exploits:


Run the SearchSploit commands to show available Icecast exploits.

command: searchsploit icecast

![searchsploit](https://user-images.githubusercontent.com/81331968/117707965-761bc000-b18c-11eb-8ee1-3269e14076ff.png)


Now that we know which exploits are available to us, let's start Metasploit:

Run the command that starts Metasploit:

command: msfconsole



![msf5](https://user-images.githubusercontent.com/81331968/117707983-7b790a80-b18c-11eb-90f7-06fd6ffe00f9.png)



Search for the Icecast module and load it for use.

Run the command to search for the Icecast module:
![screenshot 6 msf5](https://user-images.githubusercontent.com/81331968/117706186-37850600-b18a-11eb-848c-dd5ac11d8d86.png)

                
Note: Instead of copying the entire path to the module, you can use the number in front of it.

Set the RHOST to the target machine.

Run the command that sets the RHOST:

Command: set rhosts 192.168.0.20



![set rhots](https://user-images.githubusercontent.com/81331968/117710271-2985b400-b18f-11eb-98e2-22edd46cd2f4.png)


Run the Icecast exploit.

Run the command that runs the Icecast exploit.

command: exploit

Run the command that performs a search for the secretfile.txt on the target.

command: search -f secretfile*.txt

![secret file](https://user-images.githubusercontent.com/81331968/117710360-43bf9200-b18f-11eb-9fc7-ee5432f876cb.png)


Download drinks.recipe.txt

![screenshot 3](https://user-images.githubusercontent.com/81331968/117707604-f8f04b00-b18b-11eb-8315-68e2fb3260ca.png)



You should now have a Meterpreter session open.

Run the command to performs a search for the recipe.txt on the target:


![screenshot 2 meterpreter](https://user-images.githubusercontent.com/81331968/117706919-1f61b680-b18b-11eb-8853-12bf9a25a4a4.png)

You can also use Meterpreter's local exploit suggester to find possible exploits.
Note: The exploit suggester is just that: a suggestion. Keep in mind that the listed suggestions may not include all available exploits.

![meterpreter](https://user-images.githubusercontent.com/81331968/117710528-736e9a00-b18f-11eb-864c-fe81197283e0.png)










