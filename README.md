# Black Duck Polaris - Upload & Scan Lab (Lab #1)

The goal of this lab is to provide hands on experience with uploading your source to Polaris and viewing the results. As part of the lab, we will:
- execute a full SAST and SCA scan, viewing the results in the Polaris UI

This repository contains everything you need to complete the lab except for the prerequisite listed below.

## $\textsf{\color{#800080}{Prerequisites}}$

1. A Polaris user account with entitlements for SAST and SCA

## UPLOAD & SCAN WITH POLARIS
![](https://img.shields.io/badge/steps-blueviolet?style=for-the-badge)
1. Download the zip file from this [GitHub repository](https://github.com/itsnotjason/polaris-upload-lab-java) onto your local computer
2. Log in to Polaris
3. From the Polaris UI, create a new application and assign SAST and SCA subscriptions if not already created
4. Create or use an existing project. If creating new, do not use "New Project with SCM" at this time.
5. To begin testing, click the 3 dotted menu on the far right and choose "New Test"
6. Fill in the details, and upload the zip source file you previously downloaded

> [!NOTE]  
> 1. Included in this lab is a coverity.yaml file. This is used in the event your application needs to build and lets Polaris know your build commands, and any other scan overides you'd like to configure.

# Congratulations

You have now configured a Polaris workflow using the upload method and should be able to review found issues in the UI. :clap: :trophy:

## ![](https://img.shields.io/badge/optional-CTF-blueviolet?style=for-the-badge)
Once you upload the scan, you will find a "Use of Hard-coded Credentials" finding. Locate the secret, and decrypt it. Use this to assemble a sentance in the proper order. 
