# Insider Threat Forensics Lab: Investigating Data Breaches at Candy Corp
(Ficticious Organization)

<h2> Overview </h2>
This lab demonstrates key cybersecurity and forensic investigation tasks performed as a junior cybersecurity administrator, ensuring security, data integrity, and legal preparedness. I investigated a critical data breach at Candy Corp, analyzed insider threats, and managed forensic evidence. I also recovered stolen intellectual property, identified colluding employees, and compiled a court-ready evidence dossier.

<h2>Technical Skills</h2>
✅ Forensic Evidence Management<br />
✅ Insider Threat Analysis<br />
✅ Data Recovery & Encryption Analysis<br />
✅ Incident Response & Investigation<br />
✅ Digital Artifact & Log Analysis<br />
✅ Legal & Compliance Reporting<br />

<h2>  Navigating to secure my workspace </h2>
I navigated into the 'take_5' directory using the <b>cd</b> command, stepping into my designated forensic workspace. This folder functioned as a virtual crime scene—carefully quarantined to preserve the integrity of the evidence within.<br />
<br />
<p align="center">
<img src="https://i.imgur.com/tCyvbDh.png" height="80%" width="90%" alt="Navigating into take_5 Directory"/>

<h2> Creating a Case-Specific Investigation Folder </h2>
I used the <b>mkdir</b> command to create the 'Internal_Investigation_Employee_A' folder, following a clear and precise naming convention to ensure it was dedicated exclusively to this suspect's activities. To confirm I was in the correct directory, I ran <b>pwd</b>. This verification step was critical— even a minor typo could have led to unintended modifications of live system files. By double-checking, I also ensured the folder was created successfully, preventing potential errors from working in the wrong location later on.<br />
<br />
<p align="center">
<img src="https://i.imgur.com/9yhbnAI.png" height="80%" width="90%" alt="Creating Internal_Investigation_Employee_A Directory"/>
<img src="https://i.imgur.com/Razgpa2.png" height="80%" width="90%" alt="Navigating into Internal_Investigation_Employee_A Directory"/>

<h2> Initializing Core Evidence Files </h2>
I navigated into the dedicated investigation folder to ensure all files were created in the correct location. Upon discovering that 'web_evidence' was irrelevant (as Candy Corp had no web logs), I deleted it using the <b>rm</b> command, adapting my investigation approach as new information emerged. I then used <b>ls</b> to list the directory and verify that all necessary files were present. Missing a file at this stage could have led to overlooked evidence later in the process.<br />
<br />
<p align="center">
<img src="https://i.imgur.com/81pJEFD.png" height="80%" width="90%" alt="Creating multiple files within the current directory"/>
<img src="https://i.imgur.com/60GMuZ0.png" height="80%" width="90%" alt="Deleting a file"/>
<img src="https://i.imgur.com/MthrnaO.png" height="80%" width="90%" alt="Listing all files created"/>

<h2> Creating a Second Investigation Directory  </h2>
I used the <b>mkdir</b> command to create the 'Internal_Investigation_Employee_B' folder. This naming convention maintained clarity by distinctly separating the investigation data for each suspect.<br />
<br />
<p align="center">
<img src="https://i.imgur.com/YfKG30G.png" height="80%" width="90%" alt="Creating additional directory"/>

<h2> Reassigning Evidence with Absolute Paths </h2>
By using <b>mv</b> with absolute paths, I ensured that I was explicitly targeting the correct file and destination, regardless of my current working directory. This approach prevented accidental misplacement of files during the process.<br />
<br />
<p align="center">
<img src="https://i.imgur.com/aRG0CqE.png" height="80%" width="90%" alt="Moving files to another directory"/>

<h2> Copying Shared Log Evidence with Absolute Paths </h2>
Using <b>cp</b> with absolute paths ensured I was referencing the precise source and destination, preventing accidental overwrites or misplacements.<br />
<br />
<p align="center">
<img src="https://i.imgur.com/br004a8.png" height="80%" width="90%" alt="Copying files to another directory"/>

<h2> Auditing Directories to Verify Evidence Integrity </h2>
Employee A’s folder now contains only 'log_evidence' and 'web_evidence,' as the 'email_evidence' file was moved to Employee B’s directory, based on updated information linking the email leaks to B. Employee B’s folder now holds both 'email_evidence' (moved from A) and 'log_evidence' (copied from A). This ensures that shared logs are preserved for cross-analysis, while isolating the email-specific evidence to Employee B's investigation.<br />
<br />
<p align="center">
<img src="https://i.imgur.com/7piYWdD.png" height="80%" width="90%" alt="Checking files in Internal_Investigation_Employee_A directory"/>
<img src="https://i.imgur.com/JDgdtVE.png" height="80%" width="90%" alt="Checking files in Internal_Investigation_Employee_B directory"/>
<br />

<h2> Navigating to the Forensic Workspace </h2>
I used <b>cd</b> to navigate to the centralized forensic workspace, a directory pre-configured by my manager to store all evidence related to the insider threat investigation.<br />
<br />
<p align="center">
<img src="https://i.imgur.com/06e9glR.png" height="80%" width="90%" alt="Navigating to oh_henry directory"/>
  
<h2> Inspecting Henry’s Files </h2>
I moved into the 'Henry' subdirectory using <b>cd</b>, which contains all files extracted from Henry’s workstation. Then, I used <b>ls</b> to list all files within the directory for review.<br />
<br />
<p align="center">
<img src="https://i.imgur.com/n1wygxp.png" height="80%" width="90%" alt="Navigating into Henry directory"/>

<h2> Previewing Henry’s Files </h2>
By using <b>head</b> with the <b>-n</b> option, I previewed the contents of the files to determine which ones were readable and which were obfuscated.<br />
<br />
<p align="center">
<img src="https://i.imgur.com/mMCKPr7.png" height="80%" width="90%" alt="Previewing files"/>
<img src="https://i.imgur.com/PQZ5ndF.png" height="80%" width="90%" alt="Previewing files"/>

<h2> Removing Non-Readable Files </h2>
I used <b>rm</b> to remove all non-readable files from the directory, ensuring that only relevant and accessible evidence remained for analysis.<br />
<br />
<p align="center">
<img src="https://i.imgur.com/4KzlGbH.png" height="80%" width="90%" alt="Removing files"/>

<h2> Switching Focus to Ruth’s Directory </h2>
I used <b>cd</b> ../Ruth to move up one level to the parent folder and then navigated into Ruth’s dedicated directory. Once there, I used <b>ls</b> to list all files within the directory for review.<br />
<br />
<p align="center">
<img src="https://i.imgur.com/5qaLebd.png" height="80%" width="90%" alt="Navigating into Ruth directory"/>

<h2> Previewing Ruth’s Files </h2>
Using <b>head</b> with the <b>-n</b> option allowed me to preview the files, helping to identify which ones were readable and which were obfuscated.<br />
<br />
<p align="center">
<img src="https://i.imgur.com/2PhppWX.png" height="80%" width="90%" alt="Previewing files"/>
<img src="https://i.imgur.com/N4lwWWG.png" height="80%" width="90%" alt="Previewing files"/>
<img src="https://i.imgur.com/rjt8yv9.png" height="80%" width="90%" alt="Previewing files"/>

<h2> Removing Non-Readable Files </h2>
I used <b>rm</b> to remove all non-readable files from the directory, ensuring that only relevant, accessible files remained for further analysis.<br />
<br />
<p align="center">
<img src="https://i.imgur.com/NllbfJA.png" height="80%" width="90%" alt="Removing files"/>

<h2> Navigating to the Central Evidence Directory </h2>
I used <b>cd</b> to navigate to the dedicated investigation directory, a pre-configured folder designed to securely house all evidence and prevent any accidental interaction with live systems.<br />
<br />
<p align="center">
<img src="https://i.imgur.com/32lO3Yc.png" height="80%" width="90%" alt="Navigate into working directory"/>

<h2> Creating a Dedicated Directory for Combined Evidence </h2>
I used <b>mkdir</b> to create the 'Evidence_for_Authorities' directory. Then, using the <b>ls</b> command, I confirmed that the 'Evidence_for_Authorities' directory now existed alongside Henry's and Ruth's directories.<br />
<br />
<p align="center">
<img src="https://i.imgur.com/nAgPFK1.png" height="80%" width="90%" alt="Creating a new directory"/>

<h2> Navigating through directories to gather potential evidence </h2>
I used the <b>cd</b> command to navigate into the suspected directories, using <b>ls</b> along the way to list the contents and confirm that I was in the correct location.<br />
<br />
<p align="center">
<img src="https://i.imgur.com/qoOE7BV.png" height="80%" width="90%" alt="Gathering evidence"/>

<h2> Copying files into the ‘Evidence_for_authorities’ directory </h2>
I used the <b>cp</b> command with an absolute path to copy the identified files into the 'Evidence_for_Authorities' directory, ensuring they were safely placed in the correct location. Before executing the command, I previewed the text documents using <b>less</b> to confirm that the content was readable. To maintain a clear record, I made sure the filenames remained unchanged during the copy process. Afterward, I ran <b>ls</b> within the directory to verify that the files were successfully copied.<br />
<br />
<p align="center">
<img src="https://i.imgur.com/QBAx96T.png" height="80%" width="90%" alt="Copying evidence"/>
<img src="https://i.imgur.com/5qEnpVH.png" height="80%" width="90%" alt="Copying evidence"/>

<h2> Concatenating all potential evidence into a single file </h2>
I used the <b>cat</b> command to concatenate all the evidence files into a single file named 'Candy-Evidence.txt' within the 'Evidence_for_Authorities' directory. Afterward, I used <b>head</b> to check the contents of the file, ensuring that the data had merged correctly without any errors.<br />
<br />
<p align="center">
<img src="https://i.imgur.com/dNemsV4.png" height="80%" width="90%" alt="Candy-evidence file"/>

<h2> Navigating into the working directory </h2>
I used the <b>cd</b> command to enter the designated working directory for this investigation. Then, I used <b>ls</b> to confirm that the expected log files were present before proceeding.<br />
<br />
<p align="center">
<img src="https://i.imgur.com/mUVOapR.png" height="80%" width="90%" alt="Navigating into working directory"/>

<h2> Counting the number of connections to IP address </h2>
I used the <b>wc -w</b> command to count the number of words in each log file, with each word corresponding to an IP address. This command outputted the total word count for each file, indicating the number of IP connections per website.<br />
<br />
<p align="center">
<img src="https://i.imgur.com/1GwWsHh.png" height="80%" width="90%" alt="Number of connections"/>

<h2> Navigating into the working directory </h2>
Using the <b>cd</b> command, I navigated to the designated working directory where the investigation would be conducted.<br />
<br />
<p align="center">
<img src="https://i.imgur.com/ixQz8b8.png" height="80%" width="90%" alt="Naviagting into PeanutButtery.net directory"/>

<h2> Searching for directories with the word “secret” </h2>
I used the <b>find</b> command to search for directories with 'secret' in their names. This command searched recursively within the specified path, identifying all directories (denoted by <b>-type d</b>) containing 'secret' in their name, regardless of case (using <b>-iname</b>).<br />
<br />
<p align="center">
<img src="https://i.imgur.com/57vy0a6.png" height="80%" width="90%" alt="Secret directories"/>

<h2> Searching for all files with the word “recipe” </h2>
I used the <b>find</b> command to search for files with 'recipe' in their names. This command searched recursively within the specified directory for files (<b>-type f</b>) that contained 'recipe' in their name, ignoring case sensitivity (<b>-iname</b>).<br />
<br />
<p align="center">
<img src="https://i.imgur.com/rdmLOOv.png" height="80%" width="90%" alt="Recipe files"/>

<h2> Navigating into the working directory </h2>
I used the <b>cd</b> command to navigate into the designated working directory. Additionally, I ran <b>ls</b> to verify that the expected files and folders were present before proceeding.<br />
<br />
<p align="center">
<img src="https://i.imgur.com/zxFgl4J.png" height="80%" width="90%" alt="Navigating into working directories"/>

<h2> Finding all recipes with guavaberries </h2>
I used the <b>grep -i</b> command to search for the keyword 'guavaberry' across all recipe files in the working directory. This command scanned all text files for case-insensitive matches, ensuring that all relevant instances were identified.<br />
<br />
<p align="center">
<img src="https://i.imgur.com/goYEI9Z.png" height="80%" width="90%" alt="Search for guavaberries"/>

<h2> Navigating into the working directory </h2>
I used the <b>cd</b> command to navigate into the designated working directory, ensuring I was in the correct location to carry out the investigation.<br />
<br />
<p align="center">
<img src="https://i.imgur.com/Bbx5vaB.png" height="80%" width="90%" alt="Navigating into directory"/>

<h2> Creating the ‘Sugar_Evidence’ directory </h2>
I used the <b>mkdir</b> command to create a new directory named 'Sugar_Evidence.' After creating the directory, I verified its existence by running <b>ls</b> in the parent directory to ensure it had been created successfully.<br />
<br />
<p align="center">
<img src="https://i.imgur.com/1Vb3scV.png" height="80%" width="90%" alt="Creating a new directory"/>

<h2> Searching for emails referencing "sugar" </h2>
I used the <b>grep -i</b> command to search for the term 'sugar' within the email files. This performed a case-insensitive search across all email files in the directory and redirected the results, including filenames and matching lines, into a file named 'sugar_email_evidence.' To quantify the occurrences, I piped the output of the <b>grep</b> command to the <b>wc</b> command to count the number of matches.<br />
<br />
<p align="center">
<img src="https://i.imgur.com/dhFI5Aw.png" height="80%" width="90%" alt="List and number of emails"/>

<h2> Searching for weblogs referencing Sugar Corp's IP address </h2>
I used the <b>grep -i</b> command to search for the specific IP address associated with Sugar Corp across all weblog files. This command captured all occurrences of the IP address, including the filenames and matching lines, and saved the output to a file named 'web_evidence' for further analysis.<br />
<br />
<p align="center">
<img src="https://i.imgur.com/ATCL1Ec.png" height="80%" width="90%" alt="List and number of IPs"/>

<h2> Moving the Sugar web evidence file to the ‘Sugar_evidence’ directory </h2>
I used the <b>mv</b> command with an absolute path to move the identified Sugar web evidence file into the 'Sugar_evidence' directory, ensuring proper organization and secure placement of the file.<br />
<br />
<p align="center">
<img src="https://i.imgur.com/79uqE8M.png" height="80%" width="90%" alt="Moving a file"/>


<h2> Moving the Sugar email evidence file to the ‘Sugar_evidence’ directory </h2>
I used the <b>mv</b> command with an absolute path to move the Sugar email evidence file into the 'Sugar_evidence' directory, ensuring precise relocation to the correct folder.<br />
<br />
<p align="center">
<img src="https://i.imgur.com/BGiptco.png" height="80%" width="90%" alt="Moving a file"/>


<h2> Combining both the Sugar email evidence file and the Sugar web evidence file </h2>
I used the <b>cat</b> command to concatenate both files into a single, consolidated file named 'Sugar_evidence_for_authorities.' Afterward, I used <b>cat</b> again to verify the contents of the newly created file in the 'Sugar_evidence' directory, ensuring accuracy and completeness.<br />
<br />
<p align="center">
<img src="https://i.imgur.com/OPWtZyh.png" height="80%" width="90%" alt="Combining files"/>
<br />
<br />
