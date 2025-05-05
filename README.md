# Spencer-s-Gits
Repository for development in alignment with CYB333 assignments.


Purpose:
-This is a repository for security automation scripts in alignment with a final project for National University.
-This project consists of three scripts which (respectively) achieve device open port and traffic scanning, event/log viewing and summary, and recommended actions for device hardening.

Prerequisites:
-Have these modules installed on your device, and the path made available in your environment variables:
	-Current version of Python with modules:
		-Nmap
		-win32evtlog

Setup:
-To run "Spencer's Scan.txt", the only edit that needs to be made is the top IP address and subnet function. Change this information to the IP information of your local network or the devices you would like to scan.
-BE AWARE that these scripts will output JSON files in the same directory that you run them from. If you want to review them, remember that they will be located in the same folder as the save location when you pull these scripts down to your device.

Execute:
-After downloading the scripts and making the above configurations, run the scripts in this order:
	1) "Spencer's Scan.txt"
	2) "Spencer's Auditor.txt"
	3) "Spencer's FixIt.txt"

Outcome:
-By executing in this order, you will receive two JSON files. One will summarize the open ports and type of traffic being allowed over the network parameters that you input into "Spencer's Scan.txt". The second script, "Spencer's Auditor", will summarize the most recent 200 events recorded in Event Viewer, categorize them by severity, and output them to another JSON file. The final script will call on these two output JSON files and give you recommendations for review so that you can harden and/or learn more about your system environment.

Good luck!
