<h1>Installing-and-Configuring-Sysmon-on-Windows</h1>
I created This repository provides a guide and resources for installing and configuring Sysmon (System Monitor) on Windows systems. Sysmon, part of Microsoft's Sysinternals suite, enhances system monitoring capabilities by logging detailed information about process creations, network connections, and more, aiding in ID and DFIR
<br>Features</br>

    • Process Monitoring: Logs process creation, image loading, and process termination
    • Network Monitoring: Tracks network connections, including destination IPs and ports.
    • File Creation: Monitors file creations and modifications.
    • Registry Activity: Logs changes to Windows registry keys and values.
    • Driver Loading: Tracks driver loads and image executions.
Features

To install Sysmon on your Windows system, follow these steps:

1. Download Sysmon:
   
   ◦ Visit the Sysmon download page on Microsoft's Sysinternals site.
   ![Screenshot from 2024-06-14 20-37-50](https://github.com/Silvan254/Installing-and-Configuring-Sysmon-on-Windows/assets/65334897/b0de3cc8-bfa9-40ca-84f8-e6542ac7201a)

![Screenshot from 2024-06-14 20-38-38](https://github.com/Silvan254/Installing-and-Configuring-Sysmon-on-Windows/assets/65334897/3a72dae0-8516-4edd-b6a3-0fb0069d4941)

   ◦ Download the Sysmon ZIP package.
![Screenshot from 2024-06-14 20-44-18](https://github.com/Silvan254/Installing-and-Configuring-Sysmon-on-Windows/assets/65334897/60d3fc06-54e8-4a7a-b528-e862889fb2ae)


3. Extract Sysmon:
   ◦ Extract the contents of the ZIP package to a directory on your Windows machine.

![Screenshot from 2024-06-14 20-46-02](https://github.com/Silvan254/Installing-and-Configuring-Sysmon-on-Windows/assets/65334897/f37925c9-b416-4272-a6e0-03e8ae43981f)

   
5. Install Sysmon:
   
   ◦ Open a Command Prompt window with administrative privileges.

![Screenshot from 2024-06-14 20-40-05](https://github.com/Silvan254/Installing-and-Configuring-Sysmon-on-Windows/assets/65334897/185e914c-afd0-4978-835f-4800f93c2580)

   
   ◦ Navigate to the directory where you extracted Sysmon.
   
   ◦ Install Sysmon using the following command:
![Screenshot from 2024-06-14 20-46-02](https://github.com/Silvan254/Installing-and-Configuring-Sysmon-on-Windows/assets/65334897/acf505ba-cdeb-482b-ba25-9cf6e8aab4d3)
![Screenshot from 2024-06-14 20-50-17](https://github.com/Silvan254/Installing-and-Configuring-Sysmon-on-Windows/assets/65334897/ccd118af-8d09-43db-8343-37b232a579ba)

   ◦ OPen event viewer and Check sysmon is surrely installed, move to windows > Applications

   ![Screenshot from 2024-06-14 20-55-51](https://github.com/Silvan254/Installing-and-Configuring-Sysmon-on-Windows/assets/65334897/647b7da0-96e2-4687-a305-e67516099dd9)

![Screenshot from 2024-06-14 20-57-28](https://github.com/Silvan254/Installing-and-Configuring-Sysmon-on-Windows/assets/65334897/2c867c11-6ed4-48b2-9082-a0ddf796e470)

   ◦ Now lets perfoam some actions and check if the events will be loged in sysmon, Like whoami and opening calculator
   
   ![Screenshot from 2024-06-14 20-58-29](https://github.com/Silvan254/Installing-and-Configuring-Sysmon-on-Windows/assets/65334897/52a6d75c-1cea-4f60-b7f2-00bff38530bf)
   ![Screenshot from 2024-06-14 21-00-10](https://github.com/Silvan254/Installing-and-Configuring-Sysmon-on-Windows/assets/65334897/1777305b-4c2c-4caa-a13a-467d79b95756)
   
   ◦ Ohh cool, these were logged as below
![Screenshot from 2024-06-14 21-01-37](https://github.com/Silvan254/Installing-and-Configuring-Sysmon-on-Windows/assets/65334897/2f617679-4b06-4fdb-a72d-62e6de110dba)

<h2>OUR NEXT TASK IS TO PUSH THESE LOGS TO WAZUH SIEM(CHECK THIS REPOSITORY)</h2>

