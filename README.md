### UiPath RPA Challenge
# Calendar Picker Bot

[![GitHub](https://badgen.net/badge/icon/GitHub?icon=github&color=black&label)](https://github.com/MaxineXiong)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Platform - UiPath RPA](https://img.shields.io/badge/Platform-UiPath_RPA-fa4616)](https://www.uipath.com)

<br/>

This repository hosts an automation solution designed to address the challenge outlined in the requirements below.

### **Objective**

Build a bot which searches for a location in Booking.com, selects the start and end date from the calendar picker.

### **Instructions**

- Open [Booking.com](https://www.booking.com/) manually then use an *Attach Browser* activity and select the browser, tweak the selector to make it reliable and dynamic for any page of the site.
- Use a *Type Into* activity to type "New York" in the location field. Tweak the selector to exclude the id property and rather include the tag and class property. Ensure the typing happens in the background (simulate the typing of the text).
- Use a *Click* activity to open the Calendar popup.
- Drag in two *Assign* activities into the beginning of the workflow and assign two new variables "FromDate" and "ToDate" both of type String. The values must be of this format "d MMMM yyyy" for example, "8 June 2021". You can choose your own start and end dates.
- Add in two *Click* activities to select the before and after dates in the calendar picker respectively. Hint: You will need to fine-tune the selectors to be able to identify the correct day and month. To do this, split the values from the FromDate and ToDate variables and create dynamic selectors.
- Set the bot up so that it clicks the next chevron icon/button on the calendar picker for the following months if the date i.e. selector is not available in the displayed calendar popup. Do this for both the From Date and the To Date. To do this add in a *While* activity and a *Try Catch* into the *While*, then the Click Date activity into the Try. In the Catch, add in a *Click* activity which clicks the next chevron icon/button.

_You can check out the **automation demo video for the solution** below_:


https://github.com/MaxineXiong/Calendar-Picker-Bot-RPA/assets/55864839/0dd53939-90e8-4a98-9968-621b81125c0c










<br/>


## **Installation**

Before installing **UiPath Softwares**, please make sure your system meets the hardware and software requirements outlined in the **[UiPath documentation](https://docs.uipath.com/studio/standalone/2022.10/user-guide/hardware-and-software-requirements)**.

The **Uipath Platform** includes the following tools:

- **UiPath Studio**
- **UiPath Assistant**
- **UiPath Automation Cloud, including UiPath Orchestrator**

<details>  
<summary> To run this project successfully, please follow these steps to install UiPath Studio:
</summary>

***

Step 1 : Visit [uipath.com](https://www.uipath.com/) and click **Try UiPath Free** button.
<p align="center">
<img width="900" src="https://github.com/YenLinWu/RPA_UiPath/blob/master/Installation/README_Images/Install_UiPath_Studio_1.png">
</p>

Step 2: **Sign up** for a personal account.
<p align="center">
<img width="900" src="https://github.com/YenLinWu/RPA_UiPath/blob/master/Installation/README_Images/Install_UiPath_Studio_2.png">
</p>  

Step 3: **Verify** your account in email.
<p align="center">
<img width="900" src="https://github.com/YenLinWu/RPA_UiPath/blob/master/Installation/README_Images/Install_UiPath_Studio_3.png">
</p>  

Step 4: **Log into** the **UiPath Automation Cloud** using your account, and click the **Download Uipath Studio** button.
<p align="center">
<img width="900" src="https://github.com/YenLinWu/RPA_UiPath/blob/master/Installation/README_Images/Install_UiPath_Studio_4.png">
</p>   

Step 5: Click **Sign in**.
<p align="center">
<img width="900" src="https://github.com/YenLinWu/RPA_UiPath/blob/master/Installation/README_Images/Install_UiPath_Studio_5.png">
</p>    

Step 6: Select **UiPath Studio Pro**.
<p align="center">
<img width="900" src="https://github.com/YenLinWu/RPA_UiPath/blob/master/Installation/README_Images/Install_UiPath_Studio_6.png">
</p>  

Step 7: Follow the system instructions to complete the installation of **UiPath Studio Pro**.
<p align="center">
<img width="900" src="https://github.com/YenLinWu/RPA_UiPath/blob/master/Installation/README_Images/Install_UiPath_Studio_7.png">
</p> 

</details> 

<br/>

## **Usage**

To run the RPA workflow on your local machine, follow these steps:

1. Either **download** this repository to your local machine or **clone** it directly within your UiPath Studio.
2. Open the **UiPath Studio** software on your machine.
3. Locate and **open** the **Main.xaml** file from the downloaded repository in **UiPath Studio**.
4. **Run** the **Main.xaml** file to start the RPA process.

<br/>

## **Acknowledgement**

I would like to express my gratitude to the **[UiPath community](https://community.uipath.com/)** for providing resources, tutorials, and a platform for automation enthusiasts to learn and collaborate.

<br/>

## **License**

This project is licensed under the [MIT License](https://choosealicense.com/licenses/mit/), which means you're free to modify, distribute, and use the code in your own projects.
