# Black Duck Polaris - Upload & Scan Lab (Lab #1)

The goal of this lab is to provide hands on experience with uploading your source to Polaris and viewing the results. As part of the lab, we will:
- execute a full SAST and SCA scan, viewing the results in the Polaris UI

This repository contains everything you need to complete the lab except for the prerequisite listed below.

# Prerequisites

1. A Polaris user account with entitlements for SAST and SCA

# Download repository

1. Download the zip file from this repository onto your local computer

# Polaris workflow

1. Log in to Polaris
2. From the Polaris UI, create a new application and assign SAST and SCA subscriptions if not already created
3. Create or use an existing project. If creating new, do not use "New Project with SCM" at this time.
4. To begin testing, click the 3 dotted menu on the far right and choose "New Test"
5. Fill in the details, and upload the zip source file you previously downloaded

# Options

1. Unzip the files and create a coverity.yaml to the project repository (typically added to the application root folder where your build occurs).

   An example file can be seen below and is specific to your application and the build commands it needs. Polaris can scan many languages without this file, however, the more Polaris understands about your application and how it works, provides better visibility into your risk. For more information regarding support, goto https://polaris.blackduck.com/developer/default/polaris-documentation/r_support-matrix.

```
capture:
  build:
    clean-command: mvn -B clean
    build-command: mvn -B -DskipTests package
analyze:
  checkers:
    webapp-security:
      enabled: true
```

# Congratulations

You have now configured a Polaris workflow using the upload method and should be able to review found issues in the UI. :clap: :trophy:

# CTF (Optional)

Capture the value from the secret and assemble a 3 part sentance in order. 
