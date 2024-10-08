## Taking the Shortcuts

1. Clone this project in git bash terminal with:

	```
	git clone --recurse-submodules https://github.com/siler23/wca4z-pilot-shortcut.git
	```

2. Open a command prompt and create and build clientCobol ADDI project using the following command:  

	```
	C:\Users\Administrator\wca4z-pilot-shortcut\clientCobol.bat
	```

3. Setup Refactoring assistant

	1. Login to TechZone on the Windows machine
	2. Get private IPs for refactoring assistant (3 out of 3) and windows instance (2 out of 3)
	3. Download the ssh key for your refactoring assistant instance (3 of 3)
	4. Open git bash terminal and type (replacing the xs with your actual ips):

		```
		windows_private_ip=xxx.xxx.xxx.xxx refactoring_private_ip=xxx.xxx.xx.xx "${HOME}/wca4z-pilot-shortcut/IpSetup.sh"
		```

	5. Wait for the refactoring assistant started message in an opened PUTTY windows once the script finishes

4. Open the clientCobol project and all files from z/os Cobol and cobol includes folders and then build the project

5. Setup cloud watsonx instances following instructions in lab guide

6. Configure db2cli by opening git terminal and typing in credentials you've obtained for db2 in the form

	```
	host=db2hostname port=db2port user=db2user password=db2password "${HOME}/wca4z-pilot-shortcut/db2cli.sh"
	```

7. Copy and paste the outputted command in the command prompt

8. Follow lab guide instructions for creating `refactorCobol` ADDI project

9. Add Watsonx API key to vscode

System is now prepared for student use starting with refactoring assistant for lab student