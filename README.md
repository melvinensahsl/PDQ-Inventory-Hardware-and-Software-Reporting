<h1>Overview : Lab 11 PDQ Inventory: Hardware and Software Reporting</h1>

This repository documents my home lab focused on **PDQ Inventory: Hardware and Software Reporting** using **VirtualBox**. The lab aims to explore PDQ Inventory's capabilities for gathering detailed reports on hardware and software configurations across a network of virtual machines. The project will include setting up PDQ Inventory, creating custom reports, and automating hardware/software data collection for system management and network monitoring.

<h2>Objectives</h2>

- **Learn PDQ Inventory:** Explore how to set up PDQ Inventory and configure it for comprehensive hardware and software reporting.
- **Create Custom Reports:** Learn how to build and customize reports to track hardware specifications, software installations, and system configurations.



<h2>Documentation</h2>

In this home lab, I will showcase the installation and uses of **PDQ Inventory**. To start, open **File Explorer** and navigate to the **SimoTech** folder. Inside, you should find the **PDQ Inventory** application.






1. <p align="center">
   <img src="https://i.imgur.com/aVTqfoM.png" height="80%" width="80%" alt="Disk Sanitization Steps 1"/>
   <br />
   <br />
</p>

We can double click on the application to start the installation then continue it to install to finish. Launch the application once finish. 

2. <p align="center">
   <img src="https://i.imgur.com/lv9hlxL.png" height="80%" width="80%" alt="Disk Sanitization Steps 2"/>
   <br />
   <br />
</p>

Lets add Desktop2 to PDQ Inventory, to do that select “Computers” on top → “Add computers” then “Active Directory - Browse by Name” then select “Desktop2.SimoTech.com” as the target to add then select “OK”.

3. <p align="center">
   <img src="https://i.imgur.com/1m4gB68.png" height="80%" width="80%" alt="Disk Sanitization Steps 3"/>
   <br />
   <br />
</p>

**PDQ Inventory** is a powerful IT asset management tool that helps track and manage hardware and software across a network. It provides real-time insights, automates reporting, and integrates seamlessly with tools like **PDQ Deploy** for efficient software updates and policy compliance.

Here are some of the features we can use in **PDQ Inventory**: Right-click on **Desktop2**, then select **Run Report** → **Share Folders** to generate a report on the shared folders available on that machine.

4. <p align="center">
   <img src="https://i.imgur.com/laDMEG7.png" height="80%" width="80%" alt="Disk Sanitization Steps 4"/>
   <br />
   <br />
</p>

This show us all the folders that are mapped on it. Lets double click on “ADMIN$”

5. <p align="center">
   <img src="https://i.imgur.com/SuSndJy.png" height="80%" width="80%" alt="Disk Sanitization Steps 5"/>
   <br />
   <br />
</p>

It will give us all the details and specifications that are on that computer, such as who is logged in currently, what the domain controller is, the host name, what operating system it is, and what version of Windows it is using.


6. <p align="center">
   <img src="https://i.imgur.com/bNlYnPT.png" height="80%" width="80%" alt="Disk Sanitization Steps 6"/>
   <br />
   <br />
</p>

On the left-hand side, we can see all the items we can explore on Desktop2. Let's take a look at the Applications by clicking on it. This is a great way to check what applications are installed on the computer. If something is missing, we can use this feature to identify the missing software and download it accordingly.

7. <p align="center">
   <img src="https://i.imgur.com/Bujt4R7.png" height="80%" width="80%" alt="Disk Sanitization Steps 7"/>
   <br />
   <br />
</p>

To verify if we have these applications downloaded, let's go to our Desktop2 VM and open Control Panel → Uninstall a Program. This will display the list of applications installed on Desktop2 under Bob's account.

8. <p align="center">
   <img src="https://i.imgur.com/dvox4rY.png" height="80%" width="80%" alt="Disk Sanitization Steps 8"/>
   <br />
   <br />
</p>

We can also navigate to the CPU section on the left to see how many CPU cores are available on Desktop2. It will also provide information about the processors being used on the system.

9. <p align="center">
   <img src="https://i.imgur.com/3huXb17.png" height="80%" width="80%" alt="Disk Sanitization Steps 9"/>
   <br />
   <br />
</p>

The Environment tab on the left shows us the path directories configured on Desktop2 as well.

10. <p align="center">
    <img src="https://i.imgur.com/StwnqcS.png" height="80%" width="80%" alt="Disk Sanitization Steps 10"/>
    <br />
    <br />
</p>

We can look into Printers and see which printer machines are installed on Desktop2 as well.

11. <p align="center">
    <img src="https://i.imgur.com/SXQjW4O.png" height="80%" width="80%" alt="Disk Sanitization Steps 11"/>
    <br />
    <br />
</p>

On the **Shares** tab, we can see our shared drives.

12. <p align="center">
    <img src="https://i.imgur.com/kQ7k19W.png" height="80%" width="80%" alt="Disk Sanitization Steps 12"/>
    <br />
    <br />
</p>

If we wanted to remote admin into Desktop2 then double click on “ADMIIN$”, here we can see things on a system level. 

13. <p align="center">
    <img src="https://i.imgur.com/HAO88iZ.png" height="80%" width="80%" alt="Disk Sanitization Steps 13"/>
    <br />
    <br />
</p>

If we wanted to add a specific file to Desktop2, we can double click on “C$” then add anything in there.


14. <p align="center">
    <img src="https://i.imgur.com/6bvtR44.png" height="80%" width="80%" alt="Disk Sanitization Steps 14"/>
    <br />
    <br />
</p>

Lets copy the text document “results” then go into “Users” → into “Bob” → then “Desktop”.

15. <p align="center">
    <img src="https://i.imgur.com/YWO78cG.png" height="80%" width="80%" alt="Disk Sanitization Steps 15"/>
    <br />
    <br />
</p>

Paste the copied "results" file onto the Desktop, and we can see that the file was successfully transferred to our Desktop2 VM from our Windows Server 2022 VM using PDQ Inventory.

16. <p align="center">
    <img src="https://i.imgur.com/2K9XLFc.png" height="80%" width="80%" alt="Disk Sanitization Steps 16"/>
    <br />
    <br />
</p>

Some additional features in PDQ Inventory include Manage with MMC, which allows us to manage Computer Management on the Desktop2 VM directly from PDQ Inventory. To use this, select Tools at the top, then choose Manage with MMC.

17. <p align="center">
    <img src="https://i.imgur.com/cAE4kPX.png" height="80%" width="80%" alt="Disk Sanitization Steps 17"/>
    <br />
    <br />
</p>

We can create a new user on Desktop2 if we wanted to by using this feature. 

18. <p align="center">
    <img src="https://i.imgur.com/8J9OPlj.png" height="80%" width="80%" alt="Disk Sanitization Steps 18"/>
    <br />
    <br />
</p>

Another tool we can use is “Remote Desktop” if we want to remote into Desktop2 from PDQ Inventory. 

19. <p align="center">
    <img src="https://i.imgur.com/cBMl5cV.png" height="80%" width="80%" alt="Disk Sanitization Steps 19"/>
    <br />
    <br />
</p>

s

20. <p align="center">
    <img src="https://i.imgur.com/4OcMfH2.png" height="80%" width="80%" alt="Disk Sanitization Steps 20"/>
    <br />
    <br />
</p>

Another powerful feature we can use is remotely rebooting Desktop2. To do this, select Tools, then choose Reboot/Shutdown.


21. <p align="center">
    <img src="https://i.imgur.com/aWlZ8Kh.png" height="80%" width="80%" alt="Disk Sanitization Steps 21"/>
    <br />
    <br />
</p>

s

22. <p align="center">
    <img src="https://i.imgur.com/xFQVlog.png" height="80%" width="80%" alt="Disk Sanitization Steps 22"/>
    <br />
    <br />
</p>

Now, let's print a report on Desktop2. Return to the home page in All Computers, right-click on Desktop2, and select Print Preview. This feature is useful if, for example, a manager requests a report on a specific user's computer.

23. <p align="center">
    <img src="https://i.imgur.com/kiRk8vA.png" height="80%" width="80%" alt="Disk Sanitization Steps 23"/>
    <br />
    <br />
</p>

Now, let's print a report on the hardware devices on Desktop2. Right-click on Desktop2, then select Run Report → Hardware Devices. This will generate a report of all the hardware devices installed on Desktop2.

24. <p align="center">
    <img src="https://i.imgur.com/FVWvsfR.png" height="80%" width="80%" alt="Disk Sanitization Steps 24"/>
    <br />
    <br />
</p>

Select the printer icon on the top left to preview the report. This will display a list of all the hardware devices associated with Desktop2.

25. <p align="center">
    <img src="https://i.imgur.com/W46F0kZ.png" height="80%" width="80%" alt="Disk Sanitization Steps 25"/>
    <br />
    <br />
</p>

Lastly, we can launch PDQ Deploy for Desktop2 through PDQ Inventory. In All Computers, right-click on Desktop2, select Tools, and then choose Run PDQ Deploy.


26. <p align="center">
    <img src="https://i.imgur.com/mhHBfp1.png" height="80%" width="80%" alt="Disk Sanitization Steps 26"/>
    <br />
    <br />
</p>

From here, we can deploy applications or software packages onto Desktop2 using this feature. Let's select the Mozilla Firefox package that we previously installed on our Windows Server 2022 VM, then click OK to deploy it onto the Desktop2 VM.


27. <p align="center">
    <img src="https://i.imgur.com/PVeEPKM.png" height="80%" width="80%" alt="Disk Sanitization Steps 27"/>
    <br />
    <br />
</p>

Notice on the left that Desktop2.SimoTech.com is the target for the Firefox application deployment. Now, select Deploy Now to begin the deployment process.


28. <p align="center">
    <img src="https://i.imgur.com/rpr7ihk.png" height="80%" width="80%" alt="Disk Sanitization Steps 28"/>
    <br />
    <br />
</p>

Now, we can see that Firefox has been successfully installed on our Desktop2 VM through the PDQ Deploy deployment process.


29. <p align="center">
    <img src="https://i.imgur.com/8IWjtmv.png" height="80%" width="80%" alt="Disk Sanitization Steps 29"/>
    <br />
    <br />
</p>


Congratulations! We have successfully completed **Home Lab 10** on **PDQ Deploy** and **Inventory**!

This project focused on using **PDQ Inventory** within a **VirtualBox** environment to track and manage hardware and software across virtual machines. We explored creating and analyzing reports, gaining insights into user resources, and generating reports for managers or supervisors.

 👉 [Next Lab 12 : Printer Setup on Server 2022, NTFS Permissions](https://github.com/melvinensahsl/Printer-Setup-on-Server-2022-NTFS-Permissions/tree/main)
