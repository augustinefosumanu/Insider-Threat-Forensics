# Proprietary Recipe Breach

<h2> Lab </h2>

In this immersive lab, I will step into the role of a junior cybersecurity administrator at Candy Corp, where a critical breach is unfolding. The R&D division has uncovered alarming signs that a rogue employee is leaking highly classified dessert recipes to rival company Sugar Corp—threatening Candy Corp’s market dominance. My urgent mission: construct a secure forensic evidence repository to catalog, analyze, and correlate digital breadcrumbs (emails, logs, and web activity) that will expose the insider’s actions. This repository will serve as the cornerstone of the investigation, enabling me to methodically trace the breach while adhering to forensic best practices. <br />


<h2> Step 1: Navigating to secure my workspace </h2>

<b>Purpose: </b>
Before I can begin analyzing evidence, I need to ensure I’m working in a dedicated, isolated directory to prevent accidental contamination of the investigation.<br/>
<b>My Action: </b>
I use <b>cd</b> to enter the ‘take_5’ directory—my designated forensic workspace. This folder acts as a digital crime scene, quarantined to preserve evidence integrity.<br/>
<b>Reflection: </b>
By starting here, I’m setting up a controlled environment—like putting on gloves before handling physical evidence. This discipline is critical for credible forensic analysis.<br/>
<p align="center">
<img src="https://i.imgur.com/tCyvbDh.png" height="80%" width="80%" alt="Navigating into take_5 Directory"/>

<h2>Step 2: Creating a Case-Specific Investigation Folder </h2>
<b>Purpose:</b>
To isolate evidence tied to Employee A, I’ll create a dedicated directory. This ensures no cross-contamination with other cases.<br/>
<b>My Action:</b>
I use <b>mkdir</b> to create the ‘Internal_Investigation_Employee_A’ folder. This naming convention ensures clarity—it’s reserved solely for this suspect’s activities. I run <b>pwd</b> to verify I’m in the correct location. Even a small typo could lead me to accidentally modify live system files, so I double-check! confirm the folder was created successfully. Missing this step risks working in the wrong location later.<br/>
<b>Reflection:</b>
In a real breach, disorganized evidence storage could derail legal proceedings. By scripting this step, I’m practicing forensic discipline.<br/>
<p align="center">
<img src="https://i.imgur.com/9yhbnAI.png" height="80%" width="80%" alt="Creating Internal_Investigation_Employee_A Directory"/>
<img src="https://i.imgur.com/Razgpa2.png" height="80%" width="80%" alt="Navigating into Internal_Investigation_Employee_A Directory"/>

<h2>Step 3: Initializing Core Evidence Files </h2>
<b>Purpose: </b> To systematically document findings, I’ll create placeholder files for email, log, and web activity evidence tied to Employee A. <br/>
<b>My Action: </b> I enter the dedicated investigation folder to ensure files are created in the correct location. After discovering that web_evidence is irrelevant (Candy Corp has no web logs), I delete it using <b>rm</b>—practicing adaptive investigation tactics. Using <b>ls</b>, I list the directory to confirm all files exist. Missing one could mean overlooked evidence later. <br/>
<b>Reflection: </b> Though these files are empty now, they’ll soon hold hypothetical forensic artifacts—like timestamps of recipe file access or encrypted email attachments. This setup trains me to think ahead, just like preparing evidence labels at a physical crime scene. <br/>
<p align="center">
<img src="https://i.imgur.com/81pJEFD.png" height="80%" width="80%" alt="Creating multiple files within the current directory"/>
<img src="https://i.imgur.com/60GMuZ0.png" height="80%" width="80%" alt="Deleting a file"/>
<img src="https://i.imgur.com/MthrnaO.png" height="80%" width="80%" alt="Listing all files created"/>

<h2>New Details </h2>

My manager at Candy Corp needs me to create an additional directory, as they believe there is a second employee working with Sugar Corp.
I must also copy and move several of the evidence files after creating this new directory. <br />

<h2>Step 4: Creating a Second Investigation Directory  </h2>
<b>Purpose: </b> New intel suggests a second employee may be involved. To maintain forensic integrity, I’ll create a separate directory for Employee B.<br/>
<b>My Action:  </b> I use <b>mkdir</b> to create ‘Internal_Investigation_Employee_B’—this naming convention ensures clarity between suspects.<br/>
<b>Reflection:  </b> In real-world investigations, new suspects often emerge mid-case. By scripting this step, I’m practicing how to scale inquiries dynamically without compromising existing work. <br/>
<p align="center">
<img src="https://i.imgur.com/YfKG30G.png" height="80%" width="80%" alt="Creating additional directory"/>

<h2>Step 5: Reassigning Evidence with Absolute Paths </h2>
<b>Purpose:  </b> After updated intelligence reveals email_evidence does NOT belong to Employee A, I’ll securely transfer it to Employee B’s directory using absolute paths to eliminate ambiguity. <br />
<b>My Action:  </b> Using <b>mv</b> with absolute paths ensures I’m explicitly targeting the correct file and destination, regardless of my current working directory. This avoids accidental misplacement.<br />
<b>Reflection:  </b> By scripting this step, I’m practicing how to adapt investigations dynamically while maintaining an unbroken chain of custody. In court, even minor missteps like misplaced files could invalidate evidence.<br />
<p align="center">
<img src="https://i.imgur.com/aRG0CqE.png" height="80%" width="80%" alt="Moving files to another directory"/>


<h2>Step 6: Copying Shared Log Evidence with Absolute Paths </h2>
<b>Purpose:  </b> Since logs may implicate both employees, I’ll preserve the original file in Employee A’s directory while creating a copy for Employee B’s case—ensuring both investigations have access.<br />
<b>My Action: </b> Using <b>cp</b> with absolute paths guarantees I’m referencing the exact source and destination, avoiding accidental overwrites or misplacements. <br />
<b>Reflection:  </b> By scripting this step, I’m mirroring real forensic practices where evidence often applies to multiple suspects. In court, demonstrating deliberate copying (vs. moving) shows rigorous adherence to protocol.<br />
<p align="center">
<img src="https://i.imgur.com/br004a8.png" height="80%" width="80%" alt="Copying files to another directory"/>

<h2>Step 7: Auditing Directories to Verify Evidence Integrity </h2>
<b>Purpose:  </b> To ensure no misplacement or accidental deletion, I’ll rigorously audit all directories using absolute paths. <br />
<b>My Action:  </b> Employee A’s folder now only contains log_evidence and web_evidence. The email_evidence file was moved to Employee B’s directory, aligning with the updated intel that email leaks are tied to B. Employee B’s folder also holds email_evidence (moved from A) and log_evidence (copied from A). This confirms shared logs are preserved for cross-analysis while isolating email-specific evidence to B. <br />
<b>Reflection:  </b> By scripting these checks, I’m practicing forensic due diligence. In a real investigation, skipping this step could lead to missed evidence or legal challenges.<br />
<p align="center">
<img src="https://i.imgur.com/7piYWdD.png" height="80%" width="80%" alt="Checking files in Internal_Investigation_Employee_A directory"/>
<img src="https://i.imgur.com/JDgdtVE.png" height="80%" width="80%" alt="Checking files in Internal_Investigation_Employee_B directory"/>
<br />

<h2>Step :  </h2>
<b>Purpose:  </b>
<b>My Action:  </b>
<b>Reflection:  </b>
