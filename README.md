# Black Duck Polaris - Upload & Scan Lab (Lab #1)

The goal of this lab is to provide hands on experience with uploading your source to Polaris and viewing the results. There are multiple ways you can scan with Polaris, and uploading your source is one of them. In subsequent labs, we will show additional ways you can scan your applications.

As part of this lab, we will:
- ensure access to the Polaris platform
- upload our sample application to Polaris for analysis
- review the results identified in the Polaris UI

This repository contains everything you need to complete the lab except for the prerequisite listed below. If you have not yet recieved an inviation to the platform contact your Black Duck Sales Engineer.

## $\textsf{\color{#800080}{Prerequisites}}$

1. A Polaris user account with entitlements for SAST and SCA

## UPLOAD & SCAN WITH POLARIS
![](https://img.shields.io/badge/steps-blueviolet?style=for-the-badge)
1. Download the zip file from this [GitHub repository](https://github.com/itsnotjason/polaris-upload-lab-java) onto your local computer
> [!WARNING]  
> Some browsers auto unzip. You can typically recover the zip from your trash, or you may need to re-zip the files.   
2. Log in to Polaris
3. From the Polaris UI, create a new application assigning a name such as First Initial Last Initial-hellojava (ie. FL-hellojava) and assign SAST and SCA subscriptions from the drop downs prior to clicking Create Application.
4. Now that your application is created you can add projects. Click, Create + New Project and give it a name and save.
5. To begin testing, click the 3 dotted menu on the far right and choose "New Test"
6. Fill in the details, select both SAST and SCA, and upload the zip source file you previously downloaded
7. Once your scan has completed, review your results within the Polaris UI

> [!NOTE]  
> Included in this lab is a coverity.yaml file. This is used in the event your application needs to build and lets Polaris know your build commands, and any other scan overides you'd like to configure.
> 


# Congratulations

You have now configured a Polaris workflow using the upload method and should be able to review found issues in the UI. :clap: :trophy:


## ![](https://img.shields.io/badge/optional-CTF-blueviolet?style=for-the-badge)
Once you upload the scan, you will find a "Use of Hard-coded Credentials" finding. Locate the secret, and decrypt it. Use this to assemble a sentence in the proper order. 
