# Windows Server Setup Guide

This guide will walk you through the process of setting up a Windows Server on a Virtual Machine and collecting network logs for intrusion detection.

## Prerequisites

- Virtual Machine software (such as [VirtualBox](https://www.virtualbox.org/) or [VMware](https://www.vmware.com/))
- ISO image of Windows Server (available from the [Microsoft website](https://www.microsoft.com/en-us/evalcenter/evaluate-windows-server-2019))

## Step-by-Step Guide

### Step 1: Install the Virtual Machine Software

Download and install a virtual machine software like VirtualBox or VMware on your computer.

### Step 2: Setup the Windows Server

1. Open your VM software and create a new virtual machine.
2. Choose 'Microsoft Windows' as the operating system and 'Windows Server (64-bit)' as the version.
3. Allocate a portion of your RAM and create a virtual hard disk.
4. Start the virtual machine and choose the ISO image of the Windows Server for booting.
5. Follow the instructions to install the Windows Server.

### Step 3: Configuring the Server

After installation, login to your Windows Server. Install necessary roles and features based on your specific needs. For our project, we focus on generating network traffic.

### Step 4: Install Network Monitoring Tools

1. Download and install a network monitoring tool such as [Wireshark](https://www.wireshark.org/).
2. Run the tool to begin capturing network traffic.

### Step 5: Generate Network Traffic

Start generating network traffic by using the server normally. This could involve web browsing, file downloads, or running network applications.

### Step 6: Collect Network Logs

1. After sufficient network traffic has been generated, stop the network capture on your monitoring tool.
2. Save the logs in a format that can be used for machine learning (like .csv).

That's it! You have successfully set up a Windows Server, generated network traffic, and collected network logs for use in a machine learning project.
