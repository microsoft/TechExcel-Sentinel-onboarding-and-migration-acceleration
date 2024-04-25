---
title: Introduction
layout: home
nav_order: 1
---

# TechExcel: Sentinel onboarding and migration acceleration (level 300 / CSU) lab

**The estimated time to complete this lab is 90 minutes.**

Humongous IT, a global data infrastructure provider, manages a complex network of private and public clouds, along with on-premises data centers. Recognizing the need to streamline operations and enhance security, the company's board of directors approved a cloud modernization initiative, with a focus on adopting Microsoft Sentinel.

Elisabeth Eriksson, an experienced Azure admin at Humongous IT, has been put in charge of ramping up Microsoft Sentinel. She will be executing the deployment plan and ensuring that Sentinel's integration aligns with the company's IT framework and security requirements.​

**The goal of this lab is to practice configuring an environment for managing Windows and Linux security events in Azure Sentinel.**

Prior to you starting the journey, the Humongous IT environment will have programmatically deployed Windows and Linux virtual machines (VMs) with internet access. The Linux virtual machine will have a single modification to the template that adds events into its syslog. The Windows machine will have an event triggered during the lab exercises. 

These events will later be sent to Sentinel, and Sentinel will be configured to interpret these events as a potential risk and you will identify the risk created.   

To successfully complete this lab, you need to perform the following tasks:

- **Set up and configure Sentinel:** Establish a Sentinel environment with log analytics workspace and set up data connectors for Windows and Linux VMs. Configure Azure monitoring agents and define data retention strategies. 
- **Develop detection systems:** Import and verify Splunk data, create and enable Sentinel analytics rules for threat detection.
- **Simulate threats and create detections:** Review and simulate various attack types using different methods, and develop detections with Log Analytics KQL. 
- **Investigate and respond:** Analyze incidents and alerts in Sentinel, and deploy ASIM parsers for targeted registry events in Windows.  

## Exercises

This lab has exercises on:

- Configuring the Azure environment for Microsoft Sentinel
- Standing up Microsoft Sentinel with Windows and Linux data connectors
- Data Operations
- Importing Splunk data into Microsoft Sentinel
- Verifying the Splunk migration
- Importing a Splunk data export file into Microsoft Sentinel
- Verifying the migration of Splunk data rules
- Enabling migrated Splunk rules within Microsoft Sentinel
- Simulating various types of security attacks and developing detection strategies
- Creating and implementing analytics rules using Log Analytics KQL
- Investigating and responding to incidents and alerts within Microsoft Sentinel
- Deploying Advanced Security Information Management (ASIM) parsers for specific event monitoring

## Disclaimer

This presentation, demonstration, and demonstration model are for informational purposes only and (1) are not subject to SOC 1 and SOC 2 compliance audits, and (2) are not designed, intended or made available as a medical device(s) or as a substitute for professional medical advice, diagnosis, treatment or judgment. Microsoft makes no warranties, express or implied, in this presentation, demonstration, and demonstration model. Nothing in this presentation, demonstration, or demonstration model modifies any of the terms and conditions of Microsoft’s written and signed agreements. This is not an offer and applicable terms and the information provided are subject to revision and may be changed at any time by Microsoft.

This presentation, demonstration, and demonstration model do not give you or your organization any license to any patents, trademarks, copyrights, or other intellectual property covering the subject matter in this presentation, demonstration, and demonstration model.

The information contained in this presentation, demonstration and demonstration model represents the current view of Microsoft on the issues discussed as of the date of presentation and/or demonstration, for the duration of your access to the demonstration model. Because Microsoft must respond to changing market conditions, it should not be interpreted to be a commitment on the part of Microsoft, and Microsoft cannot guarantee the accuracy of any information presented after the date of presentation and/or demonstration and for the duration of your access to the demonstration model.

No Microsoft technology, nor any of its component technologies, including the demonstration model, is intended or made available as a substitute for the professional advice, opinion, or judgment of (1) a certified financial services professional, or (2) a certified medical professional. Partners or customers are responsible for ensuring the regulatory compliance of any solution they build using Microsoft technologies.

## Copyright

© 2024 Microsoft Corporation. All rights reserved. 

By using this demo/lab, you agree to the following terms:

The technology/functionality described in this demo/lab is provided by Microsoft Corporation for purposes of obtaining your feedback and to provide you with a learning experience. You may only use the demo/lab to evaluate such technology features and functionality and provide feedback to Microsoft. You may not use it for any other purpose. You may not modify, copy, distribute, transmit, display, perform, reproduce, publish, license, create derivative works from, transfer, or sell this demo/lab or any portion thereof.

COPYING OR REPRODUCTION OF THE DEMO/LAB (OR ANY PORTION OF IT) TO ANY OTHER SERVER OR LOCATION FOR FURTHER REPRODUCTION OR REDISTRIBUTION IS EXPRESSLY PROHIBITED.

THIS DEMO/LAB PROVIDES CERTAIN SOFTWARE TECHNOLOGY/PRODUCT FEATURES AND FUNCTIONALITY, INCLUDING POTENTIAL NEW FEATURES AND CONCEPTS, IN A SIMULATED ENVIRONMENT WITHOUT COMPLEX SET-UP OR INSTALLATION FOR THE PURPOSE DESCRIBED ABOVE. THE TECHNOLOGY/CONCEPTS REPRESENTED IN THIS DEMO/LAB MAY NOT REPRESENT FULL FEATURE FUNCTIONALITY AND MAY NOT WORK THE WAY A FINAL VERSION MAY WORK. WE ALSO MAY NOT RELEASE A FINAL VERSION OF SUCH FEATURES OR CONCEPTS. YOUR EXPERIENCE WITH USING SUCH FEATURES AND FUNCITONALITY IN A PHYSICAL ENVIRONMENT MAY ALSO BE DIFFERENT.

