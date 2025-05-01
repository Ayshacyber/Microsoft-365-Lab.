#  Windows Autopilot Enrollment Lab

This lab shows how to use Windows Autopilot to automatically enroll devices into Intune and apply policies during setup. Screenshots are included after each step for better understanding.

---

##  Steps and Explanations

### 1. Create a Deployment Profile  
**Path:** Devices > Windows > Enrollment > Deployment Profiles

 **Why?**  
The deployment profile tells Autopilot how the device should behave during setup (e.g., skip user steps, auto-join to Azure AD, etc.).

  
![create profile](Windows-Autopilot-Intune-Lab/create profile.png)

---

### 2. Assign the Profile to a Group/User

 **Why?**  
You must link the profile to a user or device group so that Intune knows *which devices* should get this profile.

  
![create profile]Windows-Autopilot-Intune-Lab/create profile.png)

---

### 3. Collect the Hardware ID from the Device (VM or Physical)

 **Why?**  
Autopilot uses the unique hardware ID to recognize and enroll the device. You need to export this as a `.csv` file from the device.

  
![Export Hardware ID](../Screenshots/export-hwid.png)

---

### 4. Upload the CSV File to Intune  
**Path:** Devices > Windows > Enrollment > Devices

 **Why?**  
Uploading the `.csv` file registers the device in Autopilot so that it can get the profile during setup.

  
![Upload Hardware ID CSV](../Screenshots/upload-hwid.png)

---

### 5. Factory Reset the Device (or VM)

 **Why?**  
To trigger Autopilot. When the device reboots, it connects to Autopilot, identifies itself by its hardware ID, and pulls the assigned profile and Intune policies.

  
![Reset Device](../Screenshots/factory-reset.png)

---

##  Summary

Windows Autopilot automates device provisioning. These steps simulate the real-world process in a lab setup, helping you learn how devices get enrolled and managed through Intune from day one.





