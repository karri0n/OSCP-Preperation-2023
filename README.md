# OSCP-Preperation-2023

> **_Important NOTE:_**
 follow the subreddit ([/oscp](https://www.reddit.com/r/oscp/)) and read about other people experiences, it will help... a lot!! i will link some peoples experiences below.

***My Own Experience***

https://www.reddit.com/r/oscp/comments/16h0n4l/passed_with_110_points_in_1st_attempt/ - I wrote my journey and everything I did from scratch to pass the OSCP!

# Active Directory

- To master active directory for OSCP I recommend taking the [Active directory Enumerationg & Attacks](https://academy.hackthebox.com/course/preview/active-directory-enumeration--attacks) module from HTB academy. I also recommend HTB academy for other topics, It is such a great learning resource and preparation for OSCP.
- TCM Security PEH is also a great resource for AD attacks [PracticalEthicalHacking](https://academy.tcm-sec.com/p/practical-ethical-hacking-the-complete-course).

### Mind Maps

```bash
https://whimsical.com/active-directory-YJFeAhW9GMtmLX4SWxKCCM
https://tajdini.net/blog/penetration/active-directory-penetration-mind-map/
https://i.ibb.co/TKYNCNP/Pentest-ad.png
https://xmind.app/m/vQuTSG/#
https://orange-cyberdefense.github.io/ocd-mindmaps/img/pentest_ad_dark_2022_11.svg  #Covers everything in the world :)
```

### Cheat Sheets

```bash
https://cheatsheet.haax.fr/ #One of my favorites
https://github.com/Kitsun3Sec/Pentest-Cheat-Sheets
https://kashz.gitbook.io/kashz-jewels/
https://github.com/shreyaschavhan/oscp-pre-preparation-plan-and-notes
https://wadcoms.github.io/ #interactive cheat sheet
https://github.com/Tib3rius/Active-Directory-Exploitation-Cheat-Sheet
https://github.com/infosecn1nja/AD-Attack-Defense
https://powersploit.readthedocs.io/en/stable/README/ #PowerSploit Wiki (Known for PowerView, PowerUp a nd many other insanely good tools)
https://github.com/S1ckB0y1337/Active-Directory-Exploitation-Cheat-Sheet
https://github.com/Integration-IT/Active-Directory-Exploitation-Cheat-Sheet

https://casvancooten.com/posts/2020/11/windows-active-directory-exploitation-cheat-sheet-and-command-reference/ #Covers a lot more than OSCP.. great resource
https://book.hacktricks.xyz/windows-hardening/basic-powershell-for-pentesters/powerview #PowerView / Sharpview cmdlet.. this is must to know
https://adsecurity.org/ #Everything about AD attacks, tools and news
https://www.youtube.com/watch?v=-vjF3kgvWVg #AD Enumeration
https://www.thehacker.recipes/ #Great resource
https://www.ired.team/ #One of the best resources for red teaming, its like hacktricks but goes deep into red teaming and AD stuff
https://github.com/geeksniper/active-directory-pentest
https://drive.google.com/file/d/1sLxTSGQImCxE8KbPi063OuH461ADzCR3/view
https://www.youtube.com/watch?v=Bm3mihQNGI4&list=PLDrNMcTNhhYqZj7WZt2GfNhBDqBnhW6AT #Great explaination for some of the attacks and tools.. a must follow youtube channel
```

### Build an AD lab

```bash
https://ad-lab.gitbook.io/building-a-windows-ad-lab/
https://redteamtechniques.github.io/Windows%20&%20AD%20Hacking/
https://github.com/Orange-Cyberdefense/GOAD
```

### Top ActiveDirectory tools `(must to know and be comfortable with)`

- CrackMapExec - You need to be very comfortable with this tool. 
- Evil-WinRM.
- PowerView.ps1.
- BloodHound.
- Mimikatz - Along with the other mimi-sisters like Invoke-Mimikatz, PypyKatz, SafetyKat etc..
- Rubeus.
- PowerUpSql.ps1 - Used to enumerate SQL servers.
- adPEAS.ps1 - It is like winPEAS and linPEAS - automatic enumeration of AD environement.
- ldapsearch - Used to perform LDAP queries and enumerate a DC.
- kerbrute - used to enumerate & bruteforce passwords and usernames.

### Pivoting and Tunneling

- For pivoting in OSCP, you only need `ligolo-ng`, master it and you will be 100% fine:
[Ligolo-ng](https://www.youtube.com/watch?v=DM1B8S80EvQ)
- For port forwarding you can also use ligolo but i prefer chisel (you need to know both windows and linux versions):
[Chisel](https://github.com/jpillora/chisel/releases)
- Chisel can be also used for pivoting but there is not point for not using ligolo-ng, it is just too good.

# Privilege Escalation
***Linux***

*Most common tools (MUST USE):*
  
- [pspy64](https://github.com/DominicBreuker/pspy) - Used to enumerate cronjobs in real time (live). Seriously always use this if you are stuck. 
- [LinPeas](https://github.com/carlospolop/PEASS-ng/tree/master/linPEAS).
- [LinEnum](https://github.com/rebootuser/LinEnum).
- [Linux-Exploit-Suggester](https://github.com/The-Z-Labs/linux-exploit-suggester) 
- [Linux-Exploit-Suggester2](https://github.com/jondonas/linux-exploit-suggester-2)
- [LiinuxPrivChecker](https://github.com/sleventyeleven/linuxprivchecker)

*Advise*: Always start with manual enumeration like enumerating listening ports, enumerate all machine directories, look for hidden files and creds etc.. always do th at first then use automatic tools. This also applies for windows priv esc.

```bash
https://book.hacktricks.xyz/linux-hardening/privilege-escalation #Covers everything in the world
https://academy.hackthebox.com/module/details/51 #All you need is here - It is paid and part of the HTB academy
https://tryhackme.com/room/linprivesc
https://sirensecurity.io/blog/linux-privilege-escalation-resources/
https://www.udemy.com/course/linux-privilege-escalation/?kw=privilege+esc&src=sac #Paid 
https://academy.tcm-sec.com/p/linux-privilege-escalation #Paid
https://github.com/swisskyrepo/PayloadsAllTheThings/blob/master/Methodology%20and%20Resources/Linux%20-%20Privilege%20Escalation.md
```

***Windows***

*Most common tools (MUST USE):*

- [PowerUp.ps1](https://github.com/PowerShellMafia/PowerSploit/blob/master/Privesc/PowerUp.ps1) - Always and Always use this tool first before anything else.
- [winPEAS](https://github.com/carlospolop/PEASS-ng/tree/master/winPEAS)
- [PrivEsc.ps1](https://github.com/enjoiz/Privesc/blob/master/privesc.ps1)
- [Watson.exe](https://github.com/rasta-mouse/Watson) - Used for windows kernel exploits `( I have the tool compiled I can share if needed )`.
- [Sherlock.ps1](https://github.com/rasta-mouse/Sherlock/tree/master) - Used for windows kernel exploits.
- [lazagne.exe](https://github.com/AlessandroZ/LaZagne/releases/) - One of my favorite and best tools.
- [lazagne.py](https://github.com/AlessandroZ/LaZagne/tree/master/Linux) - Python version of Lazagne.exe for linux.
- [Windows-Exploit-Suggester](https://github.com/AonCyberLabs/Windows-Exploit-Suggester)
- [Ghostpack-CompipledBinaries](https://github.com/r3motecontrol/Ghostpack-CompiledBinaries) - Very usedful binaries pre-compiled.
- [PowerSharpPack](https://github.com/S3cur3Th1sSh1t/PowerSharpPack) - PowerShell version of almost every tool used for windows and AD priv esc.
- [SharpGPOAbuse](https://github.com/FSecureLABS/SharpGPOAbuse)
- [JuicyPotato](https://github.com/ohpe/juicy-potato) - Used to abuse `SeImpersonatePrivilege`
- [PrintSpoofer](https://github.com/itm4n/PrintSpoofer) - Used to abuse `SeImpersonatePrivilege`
- [GodPotato](https://github.com/BeichenDream/GodPotato) - Used to abuse `SeImpersonatePrivilege`
- [RoguePotato](https://github.com/antonioCoco/RoguePotato) - Used to abuse `SeImpersonatePrivilege`
- [Churrasco.exe](https://github.com/Re4son/Churrasco/raw/master/churrasco.exe) - Used to abuse `SeImpersonatePrivilege`
- [SharpEfsPotato](https://github.com/bugch3ck/SharpEfsPotato) - Used to abuse `SeImpersonatePrivilege`, this is my favorite one and I always use it and it works all the time. I have the binary compiled if needed.


```bash
https://book.hacktricks.xyz/windows-hardening/windows-local-privilege-escalation
https://academy.hackthebox.com/module/details/67 #Great
https://tryhackme.com/jr/windowsprivesc20
https://www.youtube.com/channel/UCcU4a3acOkH43EjNfpprIEw/videos #Great videos
```
# Web Application Attacks

- HTB Academy has great modules which covers all server side attacks needed for OSCP (You only need server side attacks for OSCP).
- Port Swigger has great free material whicih covers everything you need for server side attacks https://portswigger.net/web-security/all-topics.
- Be Very comfortable with manual testing and exploitation especially for SQL injection.

# Payloads & shells

- [Revshells](https://www.revshells.com/)

- [RevShellGenerator](https://github.com/cwinfosec/revshellgen) - A python script to generate custom reverse shells - This is must to use.

- [HackTools](https://addons.mozilla.org/en-US/firefox/addon/hacktools/) - Browser extension to create custom reverse shells.

# All in all 
```bash
https://book.hacktricks.xyz/welcome/readme #The best website ever.
https://github.com/swisskyrepo/PayloadsAllTheThings #Really great resource for everything
https://github.com/rodolfomarianocy/OSCP-Tricks-2023
```

# Practice machines/boxes

```bash
https://docs.google.com/spreadsheets/d/1i36FP2DZA6pxMcZlCVJBqnjTvFrdVAAYGoQmUk-JlZM/edit#gid=0 #TJNulls list

https://docs.google.com/spreadsheets/d/1PVH3athOru-rHirsy30R1r8692R6J44W7uuHTrquqnk/edit#gid=1638926857

https://docs.google.com/spreadsheets/d/1dwSMIAPIam0PuRBkCiDI88pU3yzrqqHkDtBngUHNCw8/edit#gid=665299979

https://docs.google.com/spreadsheets/d/1dzvaGlT_0xnT-PGO27Z_4prHgA8PHIpErmoWdlUrSoA/htmlview

https://htbmachines.github.io/

https://www.offsec.com/labs/ #PG Practice labs is must to solve.
```
# Report Taking

- You can use the template provided by OffSec - https://help.offsec.com/hc/en-us/articles/360046787731-PEN-200-Reporting-Requirements#pwk-report-templates
- I personally used Markdown - https://github.com/noraj/OSCP-Exam-Report-Template-Markdown


# People experiences

```bash
https://www.netsecfocus.com/oscp/2021/05/06/The_Journey_to_Try_Harder-_TJnull-s_Preparation_Guide_for_PEN-200_PWK_OSCP_2.0.html #TJnulls blog

https://thatonesecguy.medium.com/hacking-hilarity-unleashed-how-i-survived-the-oscp-2023-certification-exam-and-lived-to-tell-the-254744b36c72

https://perdomo.org/2023/01/02/my-path-to-oscp/

https://medium.com/@0xP/oscp-2022-tips-to-help-you-pass-dddd3563967e

https://benheater.com/journey-to-oscp/#what-is-the-oscp

https://medium.com/@FortunateBot/oscp-passed-90-100-2022-september-7881f8c48d8f

https://dw3113r.com/2022/07/20/how-to-pass-your-oscp-exam/

https://thexssrat.medium.com/nail-your-oscp-exam-in-2023-92fc0f253035

https://www.youtube.com/watch?v=aZsysS4BaTs
```

`And lastly I wish you all the best, do not make it hard on yourself and be well prepared, it is just an exam! :>`


