## Open Source Lecture Week 6 HomeWork

Introduction: This document is a lecture note about Shell command and Git program.  
Please skip this file if this is not your interest.  

---
**1. Systematic Management System (changes)**  
There are two ways of managing version control and collaboration.  
First, **storing data as changes** to the base version.  
It basically save the difference of each version.  
Later, when user open the modified version, the system put the difference it saved to the original version and displayed to the user.  
Therefore, original version kept, and modification plus.  

Second, **storing data as snapshots**
It totally different compared to first way.  
It saved the changed version of system, not adding the changes.  
Each modified system saved just like taking snapshots of entire scene.  

![changes way](https://github.com/kda5337/lecture_note_5-2/assets/144139251/62b402fd-4ff3-4b7a-8a89-aba036931ffc)
  
**2. Systematic Management System (version control)**  
It has total 3 ways. 
First, **Local Version Control**  
Put local database on only user's computer(= local computer)  
Maybe private, but impossible for many people to work together.  

Second, **Centralized Version Control**  
There are central VCS(Version Control Server), and people access to this VCS to work together.  
Possible for collaboration work, but if **VCS Shuted down, it is disaster**.  

Last, **Distributed Version Control**  
This is **Git System**!.  
Each computer has version database for cooperation work (It literally distributed).  
It is the elaborate way for sharing work.  

![version control](https://github.com/kda5337/lecture_note_5-2/assets/144139251/2dc1bd8a-4241-4fd5-a144-543e8fa13e37)  

##Extra: three status of Git    
![three status of git](https://github.com/kda5337/lecture_note_6/assets/144139251/21f05278-5371-4591-a2ba-b5373dd89065)

**3. Git configuration: Three levels**  
1. System level: --system option. have priority(top). Affects all users and repositories on the system, so it need **administrative authority**.
2. Global (user) level: -- global option. Affects all repositories of a current user.
3. Local level: -- local option. Specific to the current repository

**4. Shell command: git int**  
This command initialized empty Git repository by creating new sub-repository.  
This new repository named in this format: .(name)  

**5. Shell command: git status**  
Checking which status does current repository on among three status we mentioned above.  

**6. Shell command: git add [file_name]**  
Use this command if you want to put any repository on staging area.  
**Extra: git add.**  
If you want to put all of directory(manby files, too) into staging area, use this command.  

**7. Shell command: git rm --cached [file_name]**  
It totally constrat with git add command, b/c it unstages a file that will be in [file_name].  
***Caution*** You must put **cached**, b/c without it, it is just command that delete the file.  
### TIPS: Ignore  
It is convenient way to unstage several files at the same time for certain current repository.  
![tips: ignore](https://github.com/kda5337/lecture_note_6/assets/144139251/b8a753b3-cc28-41ec-bdf6-81f9f21f38b8)  
**CAUTION** .gitignore is not command!!  
It creat hidden file and put file names that you do not want to stage or even commit.  


**8. Shell command: git commit -m "commit message"**  
This is final stage, it means snapshot(=save the changes as specific version).  
In "commit message" part, put explanation about what this commit is about.  
**EXTRA: command "git log"**  
You can check all of commit you have done.  

---  

**All of contents and pictures used on this markdown refers to Gachon University educational document**  
**If you want to know more about reference. please contact me**

**THANK YOU FOR READING THIS DOCUMENT**
