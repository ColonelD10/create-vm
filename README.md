![image](https://github.com/user-attachments/assets/49cc4b7c-c153-42d6-9936-e06cfb69b131)

# Creation of Virtual Machine in Azure
This tutorial outlines the steps necessary to deploy a virtual machine within Microsoft Azure and how to connect to it using Remote Desktop.
# Environments and Technologies Used
- Microsoft Azure (Resource Groups/Virtual Machines)
- Remote Desktop
# Operating Systems Used
- Windows 11
# Process Overview
- Create Resource Group
- Create Virtual Machine in Resource Group
- Obtain Virtual Machine's Public IP Address from Azure
- Connect to it using Remote Desktop
# Create Resource Group
Your first step is to create a resource group for the virtual machine to live in. This will decide the global region that your cloud server will reside in and you can organize it with a name. A resource group is a digital container that holds related resources for a particular Azure solution.

Go to www.portal.azure.com to create a free account, sign in and you will be taken to the Azure home screen/dashboard. Here you'll find common Azure services and a search bar at the top. Click on 'Resource groups' or type it into the search bar to be able to click it.

![Create Resource Group](https://github.com/user-attachments/assets/53f295a2-4c98-4664-b246-cb04bb4437a1)

This will take you to the default directory for resource groups. Now click the blue 'create' button in the center or the 'create' button in the top left of the screen.

![Create Resource Group 2](https://github.com/user-attachments/assets/5b337ae3-763e-4dd7-8fcb-1d9f2aa67500)

Now fill out your resource group's name and select a region.

![Name Group and select region](https://github.com/user-attachments/assets/da0b0c70-ac72-456d-8b40-406fe6568e63)

Skip past the 'Tags' section and you will be taken to the 'Review + create' section. As long as your resource group's name meets criteria you will be able to create it by clicking the 'Create' button in the bottom left of the screen. After doing so Azure will generate your resource group.

![Validation and creation](https://github.com/user-attachments/assets/b7b74afb-359e-4d23-ba4a-5b661f13a1cf)

From the main menu you can click on 'Resource groups' again after you've gotten the notification that it's been created to access the resource group and all the functions associated with it.

![Resource group home page](https://github.com/user-attachments/assets/1387afb5-2de0-4c5f-8a74-5a7a3d152f2a)

# Create Virtual Machine
Now you can create your virtual machine within your resource group. To do this navigate back to the Azure home screen and like with the resource group, click 'Virtual machines' in the row in the middle or search the term in the search bar.

![Create Virtual Machine](https://github.com/user-attachments/assets/0dcea63b-c0da-43bc-b1fd-26302c07a964)

Click the blue 'create' button in the center or the 'create' button in the top left of the screen. After clicking either a drop down menu will appear. Click the first option 'Azure virtual machine'.

![Create Virtual Machine 2](https://github.com/user-attachments/assets/8498a9d3-07f5-4bed-8722-01fc000b71c1)

You will be taken to the 'Create a virtual machine' screen. In the 'Basics' section, the resource group you just created should appear in a drop down menu for the 'Resource group' line. Select it. Then give your virtual machine a name and select the region it will be in. In most basic applications this should be the same region that you selected for your resource group. Leave 'Availability options', 'Zone options', and 'Availability zones' as they are for now and scroll down.

![Create virtual machine 3](https://github.com/user-attachments/assets/1071c850-3ba3-4595-b4ae-925e01ebba86)

Leave 'Security type' as it is. The 'Image' option is where you will select which operating system your virtual machine will use and how many virtual central processing units it will have as well as how much memory it will have. You then must create a username and a password to be able to sign in to the virtual machine. These options will only be available in some zones. If an option is not available in the zone you have selected in the previous section, Azure will notify you, after which you can go back and change the zone your vitual machine will be created in. After filling in these fields scroll down.

![Create virtual machine 4](https://github.com/user-attachments/assets/f55371e3-030d-4bfd-b959-8bb7513fa944)

Leave all the 'Inbound port rules' as they are. Check the box in the 'Licensing' section.

![Create virtual machine 5](https://github.com/user-attachments/assets/13a84c78-645c-4624-9cc2-2e4175611531)

As this is a basic tutorial, we won't bother with any of the other sections aside from 'Basic', so click the blue 'Review + create' button. Azure will validate your selections and if they pass, you will see a green check mark in the top left of the screen. On this screen you will also be able to see all the selections you made, as well as an estimated monthly cost for the virtual machine. Click the blue 'Create' button to deploy your virtual machine.

![Create virtual machine 6](https://github.com/user-attachments/assets/a742c051-4067-4504-ba19-6436bccebc43)
