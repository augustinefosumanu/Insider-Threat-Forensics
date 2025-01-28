# Insider Threat Forensics Lab: Investigating Data Breaches at Candy Corp
(Ficticious Organization)

<h2> Lab </h2>
In this lab, I assumed the role of a junior cybersecurity administrator tasked with investigating a critical data breach at Candy Corp. The lab focused on:<br />

-  <b>Forensic Evidence Management</b>: Constructing secure repositories to catalog and analyze logs, emails, and digital artifacts tied to insider threats.<br />
-  <b>Insider Threat Analysis</b>: Identifying collusion between employees leaking proprietary recipes to a competitor, Sugar Corp.<br />
-  <b>Critical Data Recovery</b>: Locating hidden sensitive data, analyzing encrypted files, and isolating evidence tied to stolen intellectual property.<br />
-  <b>Court-Ready Reporting</b>: Compiling a comprehensive evidence dossier to support legal action.<br />

<h2> Step 1: Navigating to secure my workspace </h2>

<b>Purpose: </b>
Before I can begin analyzing evidence, I need to ensure I’m working in a dedicated, isolated directory to prevent accidental contamination of the investigation.<br/>
<b>My Action: </b>
I use <b>cd</b> to enter the ‘take_5’ directory—my designated forensic workspace. This folder acts as a digital crime scene, quarantined to preserve evidence integrity.<br/>
<p align="center">
<img src="https://i.imgur.com/tCyvbDh.png" height="80%" width="90%" alt="Navigating into take_5 Directory"/>

<h2>Step 2: Creating a Case-Specific Investigation Folder </h2>
<b>Purpose:</b>
To isolate evidence tied to Employee A, I’ll create a dedicated directory. This ensures no cross-contamination with other cases.<br/>
<b>My Action:</b>
I use <b>mkdir</b> to create the ‘Internal_Investigation_Employee_A’ folder. This naming convention ensures clarity—it’s reserved solely for this suspect’s activities. I run <b>pwd</b> to verify I’m in the correct location. Even a small typo could lead me to accidentally modify live system files, so I double-check! confirm the folder was created successfully. Missing this step risks working in the wrong location later.<br/>
<p align="center">
<img src="https://i.imgur.com/9yhbnAI.png" height="80%" width="90%" alt="Creating Internal_Investigation_Employee_A Directory"/>
<img src="https://i.imgur.com/Razgpa2.png" height="80%" width="90%" alt="Navigating into Internal_Investigation_Employee_A Directory"/>

<h2>Step 3: Initializing Core Evidence Files </h2>
<b>Purpose: </b> To systematically document findings, I’ll create placeholder files for email, log, and web activity evidence tied to Employee A. <br/>
<b>My Action: </b> I enter the dedicated investigation folder to ensure files are created in the correct location. After discovering that web_evidence is irrelevant (Candy Corp has no web logs), I delete it using <b>rm</b>—practicing adaptive investigation tactics. Using <b>ls</b>, I list the directory to confirm all files exist. Missing one could mean overlooked evidence later. <br/>
<p align="center">
<img src="https://i.imgur.com/81pJEFD.png" height="80%" width="90%" alt="Creating multiple files within the current directory"/>
<img src="https://i.imgur.com/60GMuZ0.png" height="80%" width="90%" alt="Deleting a file"/>
<img src="https://i.imgur.com/MthrnaO.png" height="80%" width="90%" alt="Listing all files created"/>

<h2>Step 4: Creating a Second Investigation Directory  </h2>
<b>Purpose: </b> New intel suggests a second employee may be involved. To maintain forensic integrity, I’ll create a separate directory for Employee B.<br/>
<b>My Action:  </b> I use <b>mkdir</b> to create ‘Internal_Investigation_Employee_B’—this naming convention ensures clarity between suspects.<br/>
<p align="center">
<img src="https://i.imgur.com/YfKG30G.png" height="80%" width="90%" alt="Creating additional directory"/>

<h2>Step 5: Reassigning Evidence with Absolute Paths </h2>
<b>Purpose:  </b> After updated intelligence reveals email_evidence does NOT belong to Employee A, I’ll securely transfer it to Employee B’s directory using absolute paths to eliminate ambiguity. <br />
<b>My Action:  </b> Using <b>mv</b> with absolute paths ensures I’m explicitly targeting the correct file and destination, regardless of my current working directory. This avoids accidental misplacement.<br />
<p align="center">
<img src="https://i.imgur.com/aRG0CqE.png" height="80%" width="90%" alt="Moving files to another directory"/>

<h2>Step 6: Copying Shared Log Evidence with Absolute Paths </h2>
<b>Purpose:  </b> Since logs may implicate both employees, I’ll preserve the original file in Employee A’s directory while creating a copy for Employee B’s case—ensuring both investigations have access.<br />
<b>My Action: </b> Using <b>cp</b> with absolute paths guarantees I’m referencing the exact source and destination, avoiding accidental overwrites or misplacements. <br />
<p align="center">
<img src="https://i.imgur.com/br004a8.png" height="80%" width="90%" alt="Copying files to another directory"/>

<h2>Step 7: Auditing Directories to Verify Evidence Integrity </h2>
<b>Purpose:  </b> To ensure no misplacement or accidental deletion, I’ll rigorously audit all directories using absolute paths. <br />
<b>My Action:  </b> Employee A’s folder now only contains log_evidence and web_evidence. The email_evidence file was moved to Employee B’s directory, aligning with the updated intel that email leaks are tied to B. Employee B’s folder also holds email_evidence (moved from A) and log_evidence (copied from A). This confirms shared logs are preserved for cross-analysis while isolating email-specific evidence to B. <br />
<p align="center">
<img src="https://i.imgur.com/7piYWdD.png" height="80%" width="90%" alt="Checking files in Internal_Investigation_Employee_A directory"/>
<img src="https://i.imgur.com/JDgdtVE.png" height="80%" width="90%" alt="Checking files in Internal_Investigation_Employee_B directory"/>
<br />

<h2>Step 8: Navigating to the Forensic Workspace </h2>
<b>Purpose:  </b> To begin analyzing the files from Henry and Ruth, I first ensure I’m working in the secure directory where the extracted evidence is stored.<br />
<b>My Action:  </b> I use <b>cd</b> to navigate to the centralized forensic workspace. This directory was pre-configured by my manager to house all evidence related to the insider threat investigation.<br />
<p align="center">
<img src="https://i.imgur.com/06e9glR.png" height="80%" width="90%" alt="Navigating to oh_henry directory"/>
  
<h2>Step 9: Inspecting Henry’s Files </h2>
<b>Purpose:  </b> I’ll isolate Henry’s files to focus on his potential involvement with Sugar Corp, ensuring no cross-contamination with Ruth’s evidence.<br />
<b>My Action:  </b> I move into the ‘Henry’ subdirectory using <b>cd</b>—this folder contains all files extracted from Henry’s workstation then using <b>ls</b>, I list all files within the directory.<br />
<p align="center">
<img src="https://i.imgur.com/n1wygxp.png" height="80%" width="90%" alt="Navigating into Henry directory"/>

<h2>Step 10: Previewing Henry’s Files </h2>
<b>Purpose:  </b> I’ll now inspect Henry’s files to identify readable text, hidden clues, or ties to Sugar Corp.<br />
<b>My Action:  </b> By using <b>head</b> with option <b>-n</b>, I am able to preview the files to show which ones are readable and which ones are obfuscated.<br />
<p align="center">
<img src="https://i.imgur.com/mMCKPr7.png" height="80%" width="90%" alt="Previewing files"/>
<img src="https://i.imgur.com/PQZ5ndF.png" height="80%" width="90%" alt="Previewing files"/>

<h2>Step 11: Removing Non-Readable Files </h2>
<b>Purpose:  </b> To declutter the workspace, I’ll remove unreadable (binary/gibberish) files, retaining only actionable text evidence.<br />
<b>My Action:  </b> Using <b>rm</b>, I will remove all non-readable files within the directory.<br />
<p align="center">
<img src="https://i.imgur.com/4KzlGbH.png" height="80%" width="90%" alt="Removing files"/>

<h2>Step 12: Switching Focus to Ruth’s Directory </h2>
<b>Purpose:  </b> With Henry’s files triaged, I’ll now investigate Ruth’s directory to uncover potential supply chain leaks to Sugar Corp.<br />
<b>My Action:  </b> I use <b>cd</b> ../Ruth to move up one level (to the parent folder) and then into Ruth’s dedicated directory. Then using <b>ls</b>, I list all files within the directory.<br />
<p align="center">
<img src="https://i.imgur.com/5qaLebd.png" height="80%" width="90%" alt="Navigating into Ruth directory"/>


<h2>Step 13: Previewing Ruth’s Files </h2>
<b>Purpose:  </b> I’ll now inspect Ruth’s files to identify readable evidence of collaboration with Sugar Corp, focusing on communications and financial anomalies.
<b>My Action:  </b> By using <b>head</b> with option <b>-n</b>, I am able to preview the files to show which ones are readable and which ones are obfuscated.<br />
<p align="center">
<img src="https://i.imgur.com/2PhppWX.png" height="80%" width="90%" alt="Previewing files"/>
<img src="https://i.imgur.com/N4lwWWG.png" height="80%" width="90%" alt="Previewing files"/>
<img src="https://i.imgur.com/rjt8yv9.png" height="80%" width="90%" alt="Previewing files"/>

<h2>Step 14: Removing Non-Readable Files </h2>
<b>Purpose:  </b> To declutter the workspace, I’ll remove unreadable (binary/gibberish) files, retaining only actionable text evidence.<br />
<b>My Action:  </b> Using <b>rm</b>, I will remove all non-readable files within the directory.<br />
<p align="center">
<img src="https://i.imgur.com/NllbfJA.png" height="80%" width="90%" alt="Removing files"/>

<h2>Step 15: Navigating to the Central Evidence Directory </h2>
<b>Purpose:  </b> To begin analyzing the new files provided by my manager, I first ensure I’m in the secure, centralized workspace where all evidence is stored. <br />
<b>My Action:  </b>  I use <b>cd</b> to navigate to the dedicated investigation directory. This folder was pre-configured to house all evidence, ensuring no accidental interaction with live systems.<br />
<p align="center">
<img src="https://i.imgur.com/32lO3Yc.png" height="80%" width="90%" alt="Navigate into working directory"/>

<h2>Step 16: Creating a Dedicated Directory for Combined Evidence </h2>
<b>Purpose:  </b> To organize the new files from Henry and Ruth into a consolidated workspace, I’ll create a directory to centralize critical findings for the authorities.<br />
<b>My Action:  </b> I use <b>mkdir</b> to create Evidence for authorities directory . The <b>ls</b> command confirms Evidence for Authorities directory now exists alongside Henry and Ruth’s directories.<br />
<p align="center">
<img src="https://i.imgur.com/nAgPFK1.png" height="80%" width="90%" alt="Creating a new directory"/>

<h2>Step 17: Navigating through directories to gather potential evidence </h2>
<b>Purpose:  </b> To locate and organize possible evidence, I need to traverse the relevant directories systematically. This ensures that I only collect data pertinent to the investigation and maintain a clear audit trail.<br />
<b>My Action:  </b> I use the <b>cd</b> command to navigate into the suspected directories. Along the way, I employ ls to list the contents and confirm I’m in the correct location.<br />
<p align="center">
<img src="https://i.imgur.com/qoOE7BV.png" height="80%" width="90%" alt="Gathering evidence"/>

<h2>Step 18: Copying files into the ‘Evidence_for_authorities’ directory </h2>
<b>Purpose:  </b> To secure the identified evidence, I’ll copy the relevant files into a dedicated directory, ensuring they’re preserved and easily accessible for review by authorities. This step minimizes the risk of accidental tampering or loss.<br />
<b>My Action:  </b> I use the <b>cp</b> command to copy the identified files into the ‘Evidence_for_authorities’ directory along with absolute path to ensure that the files are safely copied into the right directory. Before executing the command, I preview the text documents using <b>less</b> to confirm that the texts are readable. To maintain a clear record, I ensure the filenames remain unchanged during the copy process. Afterward, I run ls within the directory to verify the files were successfully copied.<br />
<p align="center">
<img src="https://i.imgur.com/QBAx96T.png" height="80%" width="90%" alt="Copying evidence"/>
<img src="https://i.imgur.com/5qEnpVH.png" height="80%" width="90%" alt="Copying evidence"/>

<h2>Step 19: Concatenating all potential evidence into a single file </h2>
<b>Purpose:  </b> To streamline the review process for authorities, I’ll merge all the potential evidence files within the ‘Evidence_for_Authorities’ directory into a single file. This ensures that all data is consolidated while preserving the original files.<br />
<b>My Action:  </b> I use the <b>cat</b> command to concatenate all the evidence files into a single file named Candy-Evidence.txt within the ‘Evidence_for_authorities’ directory. I also check the contents of the file using <b>head</b> to ensure the data merged correctly without errors.<br />
<p align="center">
<img src="https://i.imgur.com/dNemsV4.png" height="80%" width="90%" alt="Candy-evidence file"/>

<h2>Step 20: Navigating into the working directory </h2>
<b>Purpose:  </b> To ensure all investigative activities are organized and executed within the correct environment, I’ll navigate into the designated working directory. This establishes a clear and focused space for handling evidence related to the incident.<br />
<b>My Action:  </b> I use the <b>cd</b>  command to enter the working directory specified for this investigation. I also use <b>ls</b> to ensure the expected log files are present before proceeding.<br />
<p align="center">
<img src="https://i.imgur.com/mUVOapR.png" height="80%" width="90%" alt="Navigating into working directory"/>

<h2>Step 21: Counting the number of connections to IP address </h2>
<b>Purpose:  </b> To identify the main target of the attack, I’ll analyze the log files by counting the number of words (IP addresses) in each file. This approach allows me to determine which website experienced the highest volume of connections during the attack.<br />
<b>My Action:  </b> I use the <b>wc -w</b> command to count the number of words in each log file, as each word corresponds to an IP address. This command outputs the total word count for each file, which represents the number of IP connections per website.<br />
<p align="center">
<img src="https://i.imgur.com/1GwWsHh.png" height="80%" width="90%" alt="Number of connections"/>

<h2>Step 22: Navigating into the working directory </h2>
<b>Purpose:  </b> To begin the investigation, I need to ensure I am operating within the correct working directory on the PeanutButtery.net server. This step is critical to avoid unintentionally accessing or modifying unrelated files outside the scope of the investigation. <br />
<b>My Action:  </b> Using the <b>cd</b> command, I navigate to the designated working directory where the investigation will take place.  <br />
<p align="center">
<img src="https://i.imgur.com/ixQz8b8.png" height="80%" width="80%" alt="Naviagting into PeanutButtery.net directory"/>

<h2>Step 23: Searching for directories with the word “secret” </h2>
<b>Purpose:  </b> To locate potential evidence, I need to identify any directories containing the word “secret” within their names. This is critical because such directories may house the hidden recipes or other sensitive files tied to the investigation. <br />
<b>My Action:  </b> I use the <b>find</b> command to search for directories with “secret” in their names. This command searches recursively within the specified path, identifying all directories (denoted by <b>- type d</b>) with “secret” in their name, regardless of case (using <b>- iname</b>). <br />
<p align="center">
<img src="https://i.imgur.com/57vy0a6.png" height="80%" width="80%" alt="Secret directories"/>

<h2>Step 24: Searching for all files with the word “recipe” </h2>
<b>Purpose:  </b> To uncover files potentially containing Henry’s hidden recipes, I need to locate any files with the word “recipe” in their names. This targeted search allows me to focus on evidence directly tied to the investigation. <br />
<b>My Action:  </b> I use the <b>find</b> command to search for files with “recipe” in their names. This command searches recursively within the specified directory for files (<b>- type f</b>) with “recipe” in their name, ignoring case sensitivity (<b>- iname</b>). <br />
<p align="center">
<img src="https://i.imgur.com/rdmLOOv.png" height="80%" width="80%" alt="Recipe files"/>

<h2>Step 25: Navigating into the working directory </h2>
<b>Purpose:  </b> To begin the investigation, I need to ensure I’m operating within the correct directory where all the required files and tools for this task are located. This step is crucial for maintaining organization and avoiding errors. <br />
<b>My Action:  </b> I use the <b>cd</b> command to navigate into the designated working directory. Additionally, I execute <b>ls</b> to verify the expected files and folders are present. <br />
<p align="center">
<img src="https://i.imgur.com/zxFgl4J.png" height="80%" width="80%" alt="Navigating into working directories"/>

<h2>Step 26: Finding all recipes with guavaberries </h2>
<b>Purpose:  </b> To identify which secret recipes include guavaberries as an ingredient, I’ll search the recipe files systematically. This step is crucial in assessing which proprietary formulas depend on Candy Corp’s exclusive guavaberry supply, ensuring a focused and efficient investigation. <br />
<b>My Action:  </b> I use the <b>grep -i</b> command to search for the keyword “guavaberry” across all recipe files in the working directory. This command scans all text files for case-insensitive matches. <br />
<p align="center">
<img src="https://i.imgur.com/goYEI9Z.png" height="80%" width="80%" alt="Search for guavaberries"/>

<h2>Step 27: Navigating into the working directory </h2>
<b>Purpose:  </b> To begin the investigation, I need to ensure I’m in the correct working directory where the relevant files are stored. This step is crucial to avoid any missteps, such as accessing or altering unrelated data. <br />
<b>My Action:  </b> I use the <b>cd</b> command to navigate into the designated working directory. <br />
<p align="center">
<img src="https://i.imgur.com/Bbx5vaB.png" height="80%" width="80%" alt="Navigating into directory"/>

<h2>Step 28: Creating the ‘Sugar_Evidence’ directory </h2>
<b>Purpose:  </b> To securely store all evidence related to Sugar Corp’s suspected cybercrime, I’ll create a dedicated directory. This ensures that all data collected is organized and isolated from other investigations. <br />
<b>My Action:  </b> I use the <b>mkdir</b> command to create a new directory named Sugar_Evidence. After creating the directory, I verify its existence by running <b>ls</b> in the parent directory <br />
<p align="center">
<img src="https://i.imgur.com/1Vb3scV.png" height="80%" width="80%" alt="Creating a new directory"/>

<h2>Step 29: Searching for emails referencing "sugar" </h2>
<b>Purpose:  </b> To identify any communications that reference Sugar Corp, I’ll search through email files to locate potential evidence. This step is essential for uncovering any correspondence that could link Sugar Corp to the suspected data theft. <br />
<b>My Action:  </b> I use the <b>grep -i</b> command to search for the term "sugar" within the email files. This command performs a case-insensitive search across all email files in the directory and redirects the results (including filenames and matching lines) into a file named sugar_email_evidence. I also count the number of occurrences by piping the <b>grep</b> command with <b>wc</b> command. <br />
<p align="center">
<img src="https://i.imgur.com/dhFI5Aw.png" height="80%" width="80%" alt="List and number of emails"/>

<h2>Step 30: Searching for weblogs referencing Sugar Corp's IP address </h2>
<b>Purpose:  </b> To strengthen the evidence against Sugar Corp, I will search weblog files for mentions of their suspected IP address. This step is critical in identifying communications that could directly implicate Sugar Corp in the data theft. <br />
<b>My Action:  </b> I use the <b>grep -i</b> command to search for the specific IP address associated with Sugar Corp across all weblog files. This command captures all occurrences of the IP address, including the filenames and matching lines, and saves the output to a file named web_evidence. <br />
<p align="center">
<img src="https://i.imgur.com/ATCL1Ec.png" height="80%" width="80%" alt="List and number of IPs"/>


<h2>Step 31: Moving the Sugar web evidence file to the ‘Sugar_evidence’ directory </h2>
<b>Purpose:  </b> To securely organize and preserve the web evidence file for review, I will move it to the dedicated ‘Sugar_evidence’ directory. This ensures all evidence is centralized and ready for submission. <br />
<b>My Action:  </b> I use the <b>mv</b> command along with absolute path to move the identified Sugar web evidence file into the ‘Sugar_evidence’ directory.  <br />
<p align="center">
<img src="https://i.imgur.com/79uqE8M.png" height="80%" width="80%" alt="Moving a file"/>


<h2>Step 32: Moving the Sugar email evidence file to the ‘Sugar_evidence’ directory </h2>
<b>Purpose:  </b> To ensure the email evidence is properly stored and ready for submission to the authorities, I will move the file into the ‘Sugar_evidence’ directory. This keeps all relevant evidence centralized and organized for the investigation. <br />
<b>My Action:  </b> I use the <b>mv</b> command along with absolute path to move the Sugar email evidence file into the ‘Sugar_evidence’ directory. <br />
<p align="center">
<img src="https://i.imgur.com/BGiptco.png" height="80%" width="80%" alt="Moving a file"/>


<h2>Step 33: Combining both the Sugar email evidence file and the Sugar web evidence file </h2>
<b>Purpose:  </b> To create a consolidated record of all relevant evidence related to Sugar Corp, I’ll merge the email evidence and web evidence files into a single file. This will provide a unified view of the data for easier review and submission to the authorities. <br />
<b>My Action:  </b> I use the <b>cat</b> command to concatenate both files into a single consolidated file named Sugar_evidence_for_authorities. Afterward, I use <b>cat</b> to confirm the contents of the new file created in the ‘Sugar_evidence’ directory. <br />
<p align="center">
<img src="https://i.imgur.com/OPWtZyh.png" height="80%" width="80%" alt="Combining files"/>
<br />
<br />
