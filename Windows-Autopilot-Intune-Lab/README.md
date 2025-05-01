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
 ---
   
Errors I Faced & How I Fixed Them

Intune Enrollment Issue
**Error:** `Something went wrong. Your account wasn't created.`  
**Fix:** Ensure the user has the correct MDM license assigned and that Android for Work is bound in Intune admin center.

![Error Screenshot](Screenshots/intune-error-account.png)


Google Workspace Binding Issue  
**Error:** Stuck during redirection from Intune to Google  
**Fix:** Sign in with a managed organization account, not a personal Gmail.

![Screenshot](Screenshots/google-binding-error.png)


More Screenshots

All screenshots are stored in the `Screenshots/` folder and referenced in this README.

Resources Used

- [Microsoft Docs - Intune](https://learn.microsoft.com/en-us/mem/intune/)
- [Windows Autopilot](https://learn.microsoft.com/en-us/mem/autopilot/)
- [Defender for Endpoint](https://learn.microsoft.com/en-us/microsoft-365/security/defender-endpoint/)


Screenshots:
- Autopilot profile in Intune
- Device showing as enrolled
- Policies being applied

> (Screenshots will be uploaded in the folder)
---

My Goal

To demonstrate my learning in endpoint management and security as I transition into the cybersecurity domain.


What I learned:
- How to enroll a device into Intune using Autopilot.
- How compliance and configuration policies get applied.
- How real companies manage devices without touching them physically.

Feel free to explore and use this as a reference if you're starting your own Intune lab journey!

---

Thanks for checking out my project!  
👩‍💻Aysha – Future Cybersecurity Professional
