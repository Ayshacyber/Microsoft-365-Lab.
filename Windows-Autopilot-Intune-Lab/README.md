Windows Autopilot + Intune Lab

What is this lab about?

This lab shows how I used **Windows Autopilot** and **Microsoft Intune** to set up a Windows 11 device automatically — like how companies give laptops that are ready to use on first login.

Why is this important?

In real jobs, companies don’t manually install software on every laptop. Instead, they use tools like **Autopilot and Intune** to:
- Save time
- Improve security
- Apply company settings automatically

This lab helped me learn how to set that up myself.

What I used:
- Microsoft 365 account
- Microsoft Intune (Endpoint Manager)
- Entra ID (Azure AD)
- Windows 11 in VirtualBox
- PowerShell

What I did (Steps):
1. Created a Windows 11 VM.
2. Collected the device info (hardware hash) using PowerShell.
3. Uploaded the info to Intune.
4. Created an Autopilot profile in Intune.
5. Assigned that profile to a group.
6. Restarted the VM and watched it auto-configure.

Screenshots:
- Autopilot profile in Intune
- Device showing as enrolled
- Policies being applied

> (Screenshots will be uploaded in the folder)

What I learned:
- How to enroll a device into Intune using Autopilot.
- How compliance and configuration policies get applied.
- How real companies manage devices without touching them physically.

---

Thanks for checking out my project!  
👩‍💻Aysha – Future Cybersecurity Professional
