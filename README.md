# Proprietary Recipe Data Breach

<h2> Lab </h2>

<h2> Scenario 1 </h2>

In this immersive lab, I will step into the role of a junior cybersecurity administrator at Candy Corp, where a critical breach is unfolding. The R&D division has uncovered alarming signs that a rogue employee is leaking highly classified dessert recipes to rival company Sugar Corp—threatening Candy Corp’s market dominance. My urgent mission: construct a secure forensic evidence repository to catalog, analyze, and correlate digital breadcrumbs (emails, logs, and web activity) that will expose the insider’s actions. This repository will serve as the cornerstone of the investigation, enabling me to methodically trace the breach while adhering to forensic best practices. <br />

<h2> Scenario 2 </h2>

Deep into the active investigation of the suspected intellectual property theft, two employees—Henry (Senior R&D Engineer) and Ruth (Supply Chain Manager)—have been flagged as potential insiders leaking proprietary dessert recipes to rival company Sugar Corp. My manager has covertly extracted digital files from Henry and Ruth’s workstations during a forensic sweep.<br /> These files include: <br />
-  Suspicious documents (e.g., draft recipes, communications)<br />
-  Unreadable data (encrypted/gibberish files, possibly obfuscated)<br />

My Objective is to perform a rapid triage of the files to: <br />

-  Identify readable text data (e.g., logs, emails, plaintext recipes) for immediate analysis. <br />
-  Flag gibberish/binary files that may require advanced tools (hex editors, entropy analysis).<br />
-  Prioritize evidence suggesting ties to Sugar Corp (e.g., filenames, metadata, keywords).<br />

<h2> Scenario 3 </h2>

I’ve uncovered alarming evidence of collusion between employees Henry (R&D) and Ruth (Supply Chain) with competitor Sugar Corp. My manager has just secured additional critical files from their workstations, escalating the urgency to:<br />

-  Analyze new data for ties to recipe leaks. <br />
-  Compile a court-ready evidence dossier for law enforcement within a 72-hour window before Sugar Corp’s product launch.<br />

<h2> Scenario 4 </h2>

My manager has entrusted me with log files from each of the company’s websites, containing records of IP addresses that connected to them on the day of the breach. My task is to systematically analyze these logs to identify patterns and count the number of IP addresses connecting to each website. This analysis will reveal which website endured the heaviest activity, pinpointing the attacker’s main target. By applying forensic methodologies and maintaining meticulous documentation, I will contribute to the investigation, helping Candy Corp mitigate this breach and strengthen its defenses against future threats. <br />

<h2> Step 1: Navigating to secure my workspace </h2>

<b>Purpose: </b>
Before I can begin analyzing evidence, I need to ensure I’m working in a dedicated, isolated directory to prevent accidental contamination of the investigation.<br/>
<b>My Action: </b>
I use <b>cd</b> to enter the ‘take_5’ directory—my designated forensic workspace. This folder acts as a digital crime scene, quarantined to preserve evidence integrity.<br/>
<b>Reflection: </b>
By starting here, I’m setting up a controlled environment—like putting on gloves before handling physical evidence. This discipline is critical for credible forensic analysis.<br/>
<p align="center">
<img src="https://i.imgur.com/tCyvbDh.png" height="80%" width="90%" alt="Navigating into take_5 Directory"/>

<h2>Step 2: Creating a Case-Specific Investigation Folder </h2>
<b>Purpose:</b>
To isolate evidence tied to Employee A, I’ll create a dedicated directory. This ensures no cross-contamination with other cases.<br/>
<b>My Action:</b>
I use <b>mkdir</b> to create the ‘Internal_Investigation_Employee_A’ folder. This naming convention ensures clarity—it’s reserved solely for this suspect’s activities. I run <b>pwd</b> to verify I’m in the correct location. Even a small typo could lead me to accidentally modify live system files, so I double-check! confirm the folder was created successfully. Missing this step risks working in the wrong location later.<br/>
<b>Reflection:</b>
In a real breach, disorganized evidence storage could derail legal proceedings. By scripting this step, I’m practicing forensic discipline.<br/>
<p align="center">
<img src="https://i.imgur.com/9yhbnAI.png" height="80%" width="90%" alt="Creating Internal_Investigation_Employee_A Directory"/>
<img src="https://i.imgur.com/Razgpa2.png" height="80%" width="90%" alt="Navigating into Internal_Investigation_Employee_A Directory"/>

<h2>Step 3: Initializing Core Evidence Files </h2>
<b>Purpose: </b> To systematically document findings, I’ll create placeholder files for email, log, and web activity evidence tied to Employee A. <br/>
<b>My Action: </b> I enter the dedicated investigation folder to ensure files are created in the correct location. After discovering that web_evidence is irrelevant (Candy Corp has no web logs), I delete it using <b>rm</b>—practicing adaptive investigation tactics. Using <b>ls</b>, I list the directory to confirm all files exist. Missing one could mean overlooked evidence later. <br/>
<b>Reflection: </b> Though these files are empty now, they’ll soon hold hypothetical forensic artifacts—like timestamps of recipe file access or encrypted email attachments. This setup trains me to think ahead, just like preparing evidence labels at a physical crime scene. <br/>
<p align="center">
<img src="https://i.imgur.com/81pJEFD.png" height="80%" width="90%" alt="Creating multiple files within the current directory"/>
<img src="https://i.imgur.com/60GMuZ0.png" height="80%" width="90%" alt="Deleting a file"/>
<img src="https://i.imgur.com/MthrnaO.png" height="80%" width="90%" alt="Listing all files created"/>

<h2>New Details </h2>

My manager at Candy Corp needs me to create an additional directory, as they believe there is a second employee working with Sugar Corp.
I must also copy and move several of the evidence files after creating this new directory. <br />

<h2>Step 4: Creating a Second Investigation Directory  </h2>
<b>Purpose: </b> New intel suggests a second employee may be involved. To maintain forensic integrity, I’ll create a separate directory for Employee B.<br/>
<b>My Action:  </b> I use <b>mkdir</b> to create ‘Internal_Investigation_Employee_B’—this naming convention ensures clarity between suspects.<br/>
<b>Reflection:  </b> In real-world investigations, new suspects often emerge mid-case. By scripting this step, I’m practicing how to scale inquiries dynamically without compromising existing work. <br/>
<p align="center">
<img src="https://i.imgur.com/YfKG30G.png" height="80%" width="90%" alt="Creating additional directory"/>

<h2>Step 5: Reassigning Evidence with Absolute Paths </h2>
<b>Purpose:  </b> After updated intelligence reveals email_evidence does NOT belong to Employee A, I’ll securely transfer it to Employee B’s directory using absolute paths to eliminate ambiguity. <br />
<b>My Action:  </b> Using <b>mv</b> with absolute paths ensures I’m explicitly targeting the correct file and destination, regardless of my current working directory. This avoids accidental misplacement.<br />
<b>Reflection:  </b> By scripting this step, I’m practicing how to adapt investigations dynamically while maintaining an unbroken chain of custody. In court, even minor missteps like misplaced files could invalidate evidence.<br />
<p align="center">
<img src="https://i.imgur.com/aRG0CqE.png" height="80%" width="90%" alt="Moving files to another directory"/>

<h2>Step 6: Copying Shared Log Evidence with Absolute Paths </h2>
<b>Purpose:  </b> Since logs may implicate both employees, I’ll preserve the original file in Employee A’s directory while creating a copy for Employee B’s case—ensuring both investigations have access.<br />
<b>My Action: </b> Using <b>cp</b> with absolute paths guarantees I’m referencing the exact source and destination, avoiding accidental overwrites or misplacements. <br />
<b>Reflection:  </b> By scripting this step, I’m mirroring real forensic practices where evidence often applies to multiple suspects. In court, demonstrating deliberate copying (vs. moving) shows rigorous adherence to protocol.<br />
<p align="center">
<img src="https://i.imgur.com/br004a8.png" height="80%" width="90%" alt="Copying files to another directory"/>

<h2>Step 7: Auditing Directories to Verify Evidence Integrity </h2>
<b>Purpose:  </b> To ensure no misplacement or accidental deletion, I’ll rigorously audit all directories using absolute paths. <br />
<b>My Action:  </b> Employee A’s folder now only contains log_evidence and web_evidence. The email_evidence file was moved to Employee B’s directory, aligning with the updated intel that email leaks are tied to B. Employee B’s folder also holds email_evidence (moved from A) and log_evidence (copied from A). This confirms shared logs are preserved for cross-analysis while isolating email-specific evidence to B. <br />
<b>Reflection:  </b> By scripting these checks, I’m practicing forensic due diligence. In a real investigation, skipping this step could lead to missed evidence or legal challenges.<br />
<p align="center">
<img src="https://i.imgur.com/7piYWdD.png" height="80%" width="90%" alt="Checking files in Internal_Investigation_Employee_A directory"/>
<img src="https://i.imgur.com/JDgdtVE.png" height="80%" width="90%" alt="Checking files in Internal_Investigation_Employee_B directory"/>
<br />

<h2>Step 8: Navigating to the Forensic Workspace </h2>
<b>Purpose:  </b> To begin analyzing the files from Henry and Ruth, I first ensure I’m working in the secure directory where the extracted evidence is stored.<br />
<b>My Action:  </b> I use <b>cd</b> to navigate to the centralized forensic workspace. This directory was pre-configured by my manager to house all evidence related to the insider threat investigation.<br />
<b>Reflection:  </b> By starting here, I’m setting up a controlled environment—like putting on gloves before handling physical evidence. This discipline is critical for credible forensic analysis.<br />
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
<b>Reflection:  </b> By scripting these commands, I’m simulating real-world insider threat hunting—where seconds matter and buried clues can unravel entire schemes.<br />
<p align="center">
<img src="https://i.imgur.com/mMCKPr7.png" height="80%" width="90%" alt="Previewing files"/>
<img src="https://i.imgur.com/PQZ5ndF.png" height="80%" width="90%" alt="Previewing files"/>

<h2>Step 11: Removing Non-Readable Files </h2>
<b>Purpose:  </b> To declutter the workspace, I’ll remove unreadable (binary/gibberish) files, retaining only actionable text evidence.<br />
<b>My Action:  </b> Using <b>rm</b>, I will remove all non-readable files within the directory.<br />
<b>Reflection:  </b>In real investigations, binaries are archived (not deleted) for advanced analysis. This simulation prioritizes simplicity.<br />
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
<b>Reflection:  </b> By scripting these commands, I’m mirroring real-world forensic workflows where hidden threats lurk in plain sight—and only meticulous analysis uncovers them.”
<p align="center">
<img src="https://i.imgur.com/2PhppWX.png" height="80%" width="90%" alt="Previewing files"/>
<img src="https://i.imgur.com/N4lwWWG.png" height="80%" width="90%" alt="Previewing files"/>
<img src="https://i.imgur.com/rjt8yv9.png" height="80%" width="90%" alt="Previewing files"/>

<h2>Step 14: Removing Non-Readable Files </h2>
<b>Purpose:  </b> To declutter the workspace, I’ll remove unreadable (binary/gibberish) files, retaining only actionable text evidence.<br />
<b>My Action:  </b> Using <b>rm</b>, I will remove all non-readable files within the directory.<br />
<b>Reflection:  </b>In real investigations, binaries are archived (not deleted) for advanced analysis. This simulation prioritizes simplicity.<br />
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
<b>Reflection:  </b> Missteps in directory navigation can lead to missing critical evidence or unintentionally modifying files, which could compromise the investigation. By following a methodical approach and validating each step, I uphold the integrity of the forensic process and ensure the evidence remains admissible in legal proceedings.<br />
<p align="center">
<img src="https://i.imgur.com/qoOE7BV.png" height="80%" width="90%" alt="Gathering evidence"/>

<h2>Step 18: Copying files into the ‘Evidence_for_authorities’ directory </h2>
<b>Purpose:  </b> To secure the identified evidence, I’ll copy the relevant files into a dedicated directory, ensuring they’re preserved and easily accessible for review by authorities. This step minimizes the risk of accidental tampering or loss.<br />
<b>My Action:  </b> I use the <b>cp</b> command to copy the identified files into the ‘Evidence_for_authorities’ directory along with absolute path to ensure that the files are safely copied into the right directory. Before executing the command, I preview the text documents using <b>less</b> to confirm that the texts are readable. To maintain a clear record, I ensure the filenames remain unchanged during the copy process. Afterward, I run ls within the directory to verify the files were successfully copied.<br />
<b>Reflection:  </b> Properly securing evidence is vital in forensic investigations. Mishandling this step—such as copying files into the wrong directory or failing to verify their integrity—can jeopardize the chain of custody. By being meticulous, I uphold best practices and ensure the evidence remains reliable for legal use. <br />
<p align="center">
<img src="https://i.imgur.com/QBAx96T.png" height="80%" width="90%" alt="Copying evidence"/>
<img src="https://i.imgur.com/5qEnpVH.png" height="80%" width="90%" alt="Copying evidence"/>

<h2>Step 19: Concatenating all potential evidence into a single file </h2>
<b>Purpose:  </b> To streamline the review process for authorities, I’ll merge all the potential evidence files within the ‘Evidence_for_Authorities’ directory into a single file. This ensures that all data is consolidated while preserving the original files.<br />
<b>My Action:  </b> I use the <b>cat</b> command to concatenate all the evidence files into a single file named Candy-Evidence.txt within the ‘Evidence_for_authorities’ directory. I also check the contents of the file using <b>head</b> to ensure the data merged correctly without errors.<br />
<b>Reflection:  </b> Combining evidence into a single file saves time during reviews but requires precision to avoid data loss or corruption. By validating each step, I ensure the final file is accurate and complete, maintaining the chain of custody and forensic integrity.<br />
<p align="center">
<img src="https://i.imgur.com/dNemsV4.png" height="80%" width="90%" alt="Candy-evidence file"/>

<h2>Step 20: Navigating into the working directory </h2>
<b>Purpose:  </b> To ensure all investigative activities are organized and executed within the correct environment, I’ll navigate into the designated working directory. This establishes a clear and focused space for handling evidence related to the incident.<br />
<b>My Action:  </b> I use the <b>cd</b>  command to enter the working directory specified for this investigation. I also use <b>ls</b> to ensure the expected log files are present before proceeding.<br />
<b>Reflection:  </b> Starting in the wrong directory could lead to disorganized work or accidental modifications to unrelated files. By double-checking my location and verifying the presence of necessary files, I establish a disciplined workflow critical to forensic investigations.<br />
<p align="center">
<img src="https://i.imgur.com/mUVOapR.png" height="80%" width="90%" alt="Navigating into working directory"/>

<h2>Step 21: Counting the number of connections to IP address </h2>
<b>Purpose:  </b> To identify the main target of the attack, I’ll analyze the log files by counting the number of words (IP addresses) in each file. This approach allows me to determine which website experienced the highest volume of connections during the attack.<br />
<b>My Action:  </b> I use the <b>wc -w</b> command to count the number of words in each log file, as each word corresponds to an IP address. This command outputs the total word count for each file, which represents the number of IP connections per website.<br />
<b>Reflection:  </b> Using wc -w ensures precise counting of IP addresses in each log file, which is crucial for identifying the attack’s main target. Careful execution and verification of this step help maintain the integrity of my findings and support a thorough investigation.<br />
<p align="center">
<img src="https://i.imgur.com/1GwWsHh.png" height="80%" width="90%" alt="Number of connections"/>
<br />
<br />
