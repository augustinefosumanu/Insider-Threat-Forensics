# Proprietary Recipe Breach

<h2> Lab </h2>

In this immersive lab, I will step into the role of a junior cybersecurity administrator at Candy Corp, where a critical breach is unfolding. The R&D division has uncovered alarming signs that a rogue employee is leaking highly classified dessert recipes to rival company Sugar Corp—threatening Candy Corp’s market dominance. My urgent mission: construct a secure forensic evidence repository to catalog, analyze, and correlate digital breadcrumbs (emails, logs, and web activity) that will expose the insider’s actions. This repository will serve as the cornerstone of the investigation, enabling me to methodically trace the breach while adhering to forensic best practices. <br />


<h2> Step 1: Navigating to secure my workspace </h2>

<b>Purpose:</b>
Before I can begin analyzing evidence, I need to ensure I’m working in a dedicated, isolated directory to prevent accidental contamination of the investigation.<br/>
<b>My Action:</b>
I use 'cd' to enter the ‘take_5’ directory—my designated forensic workspace. This folder acts as a digital crime scene, quarantined to preserve evidence integrity.<br/>
<b>Reflection:</b>
By starting here, I’m setting up a controlled environment—like putting on gloves before handling physical evidence. This discipline is critical for credible forensic analysis.<br/>
<p align="center">
<img src="https://i.imgur.com/tCyvbDh.png" height="80%" width="80%" alt="Navigating into take_5 Directory"/>

<h2>Step 2: Creating a Case-Specific Investigation Folder </h2>
<b>Purpose:</b>
To isolate evidence tied to Employee A, I’ll create a dedicated directory. This ensures no cross-contamination with other cases.<br/>
<b>My Action:</b>
I use 'mkdir' to create the ‘Internal_Investigation_Employee_A’ folder. This naming convention ensures clarity—it’s reserved solely for this suspect’s activities. I run 'pwd' to verify I’m in the correct location. Even a small typo could lead me to accidentally modify live system files, so I double-check! confirm the folder was created successfully. Missing this step risks working in the wrong location later.<br/>
<b>Reflection:</b>
In a real breach, disorganized evidence storage could derail legal proceedings. By scripting this step, I’m practicing forensic discipline.<br/>
<p align="center">
<img src="https://i.imgur.com/9yhbnAI.png" height="80%" width="80%" alt="Creating Internal_Investigation_Employee_A Directory"/>
<img src="https://i.imgur.com/Razgpa2.png" height="80%" width="80%" alt="Navigating into Internal_Investigation_Employee_A Directory"/>

<h2>Step 3: Initializing Core Evidence Files </h2>
<b>Purpose: </b> To systematically document findings, I’ll create placeholder files for email, log, and web activity evidence tied to Employee A. <br/>
<b>My Action: </b> I enter the dedicated investigation folder to ensure files are created in the correct location. After discovering that web_evidence is irrelevant (Candy Corp has no web logs), I delete it—practicing adaptive investigation tactics. I list the directory to confirm all files exist. Missing one could mean overlooked evidence later. <br/>
<b>Reflection: </b> Though these files are empty now, they’ll soon hold hypothetical forensic artifacts—like timestamps of recipe file access or encrypted email attachments. This setup trains me to think ahead, just like preparing evidence labels at a physical crime scene. <br/>
<p align="center">
<img src="https://i.imgur.com/81pJEFD.png" height="80%" width="80%" alt="Creating multiple files within the current directory"/>
<img src="https://i.imgur.com/60GMuZ0.png" height="80%" width="80%" alt="Deleting a file"/>
<img src="https://i.imgur.com/MthrnaO.png" height="80%" width="80%" alt="Listing all files created"/>

<h2>Step :  </h2>
<b>Purpose:  </b>
<b>My Action:  </b>
<b>Reflection:  </b>

<h2>Step :  </h2>
<b>Purpose:  </b>
<b>My Action:  </b>
<b>Reflection:  </b>


<h2>Description</h2>

Your manager at Candy Corp needs you to create an additional directory, as they believe there is a second employee working with Sugar Corp.
You must also copy and move several of the evidence files after creating this new directory. <br />

<h2>Walk-through</h2>

<p align="center">
Navigate back into working Directory: <br/>
<img src="https://i.imgur.com/eID7cPD.png" height="80%" width="80%" alt="Navigate into take_5 Directory"/>
<br />
<br />
<p align="center">
Create an additional folder called Internal_Investigation_Employee_B.: <br/>
<img src="https://i.imgur.com/YfKG30G.png" height="80%" width="80%" alt="Creating additional directory"/>
<br />
<br />
<p align="center">
Using absolute paths, move the file email_evidence from Internal_Investigation_Employee_A to Internal_Investigation_Employee_B because you have been told there won’t be email evidence for the first employee: <br/>
<img src="https://i.imgur.com/aRG0CqE.png" height="80%" width="80%" alt="Moving files to another directory"/>
<br />
<br />
<p align="center">
Using absolute paths, copy the file log_evidence from Internal_Investigation_Employee_A to Internal_Investigation_Employee_B, as you have been told there will likely be log evidence from both employees: <br/>
<img src="https://i.imgur.com/br004a8.png" height="80%" width="80%" alt="Copying files to another directory"/>
<br />
<br />
<p align="center">
Check your directories to confirm the files are all in the correct locations: <br/>
<img src="https://i.imgur.com/7piYWdD.png" height="80%" width="80%" alt="Checking files in Internal_Investigation_Employee_A directory"/>
<br />
<br />
<p align="center">
Check your directories to confirm the files are all in the correct locations: <br/>
<img src="https://i.imgur.com/JDgdtVE.png" height="80%" width="80%" alt="Checking files in Internal_Investigation_Employee_B directory"/>
<br />
<br />
