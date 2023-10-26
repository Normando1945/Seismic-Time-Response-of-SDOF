<div align="center">
    <img src="https://github.com/Normando1945/Normando1945.github.io/assets/62081230/1ac0bf1d-67cd-43f6-87b0-141417a606db">
</div>

>##### Author:                 [Msc. Ing. Carlos Andrés Celi Sánchez](https://www.researchgate.net/profile/Carlos-Celi). & [Phd(c). MSc. Ing. José Poveda](https://www.torrefuerte.com)

>##### Course:                 Structural Dynamics


### **You can find me on**
[![Web Page](https://img.shields.io/badge/Web%20Page-caceli.net-blue)](http:caceli.net)
[![GitHub Carlos Celi](https://img.shields.io/github/followers/Normando1945?label=follow&style=social)](https://github.com/Normando1945)
[![ResearchGate](https://img.shields.io/badge/-ResearchGate-00CCBB?style=social&logo=researchgate)](https://www.researchgate.net/profile/Carlos-Celi)
[![Google Scholar](https://img.shields.io/badge/-Google%20Scholar-4285F4?style=social&logo=google)](https://scholar.google.com.ec/citations?hl=es&user=yR4Gz7kAAAAJ)
<a href="Carlos Celi:normando1945@gmail.com"><img alt="Email" src="https://img.shields.io/badge/Email-normando1945@gmail.com-blue?style=flat&logo=gmail"></a>


## Introduction:
This software application is straightforward, designed to compute the time response of underdamped single-degree-of-freedom **[SDOF](https://en.wikipedia.org/wiki/Vibration)** systems using the discrete Beta Newmark method. Importantly, this software should not be seen as a replacement for formal classroom instruction but rather as a tool to supplement it. It was developed mainly for underdamped systems subjected to non-periodic and non-harmonic external excitations, like earthquakes. The primary purpose of this tool is to provide students with a visual aid, helping them comprehend how structures behave during actual seismic events. In doing so, users should be aware of the inherent simplifications and approximations in the **[SDOF](https://en.wikipedia.org/wiki/Vibration)** Beta-Newmark calculation.

Moreover, it is essential for users of this academic software to have sufficient knowledge regarding the step-by-step time-domain response calculation of 1 DOF systems. To familiarize oneself with the mathematical foundation, you can visit the repository **[Brief Overview of Undergraduate Structural Dynamics for Engineers](https://github.com/Normando1945/Normando1945.github.io)**, where you will find an academic summary on this topic.

### Installation Steps:
* For optimal performance, install **[7-Zip](https://www.7-zip.org/)** (free software).
  
    <div align="center">
        <img src= "https://github.com/Normando1945/Seismic-Time-Response-of-SDOF/assets/62081230/fed842ae-e290-40b7-a082-b557228eff39">
    </div>
* Using **[7-Zip]**, **[WinRAR]**, or a similar software, unzip the file **<u>"TH_SDOF_CC_setup.7z.001"</u>** to your desired location.
  
    <div align="center">
        <img src= "https://github.com/Normando1945/Seismic-Time-Response-of-SDOF/assets/62081230/236e6dd1-6147-4b4a-8061-7f950d0a8b95">
    </div>
    
* Note: Ensure all files downloaded from the repository are in the same folder.
* Once unzipped, an executable file named **"TH_SDOF_CC_setup.exe"** will appear. Double-click this file to initiate the installation process. Simply follow the on-screen instructions thereafter.
* Please read and accept the terms and conditions.
  <div align="center">
        <img src= "https://github.com/Normando1945/Seismic-Time-Response-of-SDOF/assets/62081230/3769f8e5-29c7-4013-9d5b-35564187be68">
  </div>
* Enter the installation key. Password: **<u>soloparausoacademico<u>**
  <div align="center">
      <img src= "https://github.com/Normando1945/Seismic-Time-Response-of-SDOF/assets/62081230/cc18dacd-f6be-4952-8918-c395d16a3af0">
  </div>
* Select your preferred directory.
  <div align="center">
      <img src= "https://github.com/Normando1945/Seismic-Time-Response-of-SDOF/assets/62081230/b781f405-a9f6-41bc-84f6-1c9b95adfc48">
  </div>
* If you wish, you can create a shortcut on your desktop.
  <div align="center">
      <img src= "https://github.com/Normando1945/Seismic-Time-Response-of-SDOF/assets/62081230/a39da2e6-cad3-4b66-a4af-082c1bcacf1b">
  </div>
  * Proceed with the installation.
  <div align="center">
      <img src= "https://github.com/Normando1945/Seismic-Time-Response-of-SDOF/assets/62081230/766c1a02-f343-48f8-8b8c-89958c3d1fb2">
  </div>

  View of the main screen.
  <div align="center">
      <img src= "https://github.com/Normando1945/Seismic-Time-Response-of-SDOF/assets/62081230/ac9b4f1a-82c0-4a9c-8e91-28586ccc906b">
  </div>
  


## User Manual:

The usage is straightforward. Please enter the required parameters into the designated spaces

* **Period of motion [from 0.01 to 4]** : The fundamental vibration period of the **SDOF** system, whose time response you wish to determine, must be input. This software is limited to calculating structural periods ranging from **0.01** seconds to **4** seconds. Nevertheless, the algorithm can determine the response for any period greater than **0** seconds. Periods less than **0.01** seconds or greater than **4** seconds may yield results with diminished reliability due to the inherent convergence and stability of the calculation method.
  
* **Damping Ratio [from 0.01 to 0.99]** : You must input the value of the equivalent viscous damping for the **SDOF** structural system you wish to analyze. It's understood that the algorithm is based on a discrete step-by-step solution in the time domain for underdamped systems. For this reason, the range of damping values is from **$\zeta$ = 0.01 to 0.99**. Potentially, **$\zeta$ = 0** can be used to describe a conservative system. Values of **$\zeta$ >= 1** should not be used as they would emulate overdamped systems, which would result in numerical instability in the step-by-step solution of this software.

* **Files in the Folder** : Displays the number of .AT2 files located in the folder where the software **"TH_SDOF_CC"** was installed. Officially, along with the installation, 7 real seismic records are added, listed below:
  - AMT_201604162359_E_100.AT2
  - Artificial.AT2
  - ChiChi_longt.AT2
  - ChiChi_tranv.AT2
  - Friulli.AT2
  - Hollister.AT2
  - Loma_Prieta_1989.AT2

* **Record Selected from the database in the root of the folder, for this data base from 1 to "n"** : You must enter the **number** of the seismic record you wish to use as external excitation. To do this, please refer to **"Files in the Folder"**..
* **PLAY** : Click the **"PLAY"** button to begin the calculation.
* **Random data** : Clicking this button populates all the necessary fields with random values within the previously specified ranges.

### Results.
This academic software displays the results graphically across two interactive individual screens. The first screen presents the employed seismic record alongside the structural response in displacement, velocity, and acceleration. The second screen showcases an animation [not to scale] of the acceleration response of the analyzed **SDOF** system.

### Example.
  <div align="center">
      <img src= "https://github.com/Normando1945/Seismic-Time-Response-of-SDOF/assets/62081230/8d20e7f9-ddfd-4bf3-8421-5f9ee07d2151">
  </div>
  <div align="center">
      <img src= "https://github.com/Normando1945/Seismic-Time-Response-of-SDOF/assets/62081230/4355650d-9b52-41a8-baf5-60647d3180bc">
  </div>

## Important: 
 - Each time you wish to conduct a new analysis, click on **"Close Windows"** button.
 - If the user wishes to use seismic records other than those pre-loaded in the current software, it can be done in a straightforward manner. To do so, the following steps are recommended:
    - Navigate to the folder where the program was installed.
          <div align="center">
              <img src= "https://github.com/Normando1945/Seismic-Time-Response-of-SDOF/assets/62081230/a7eac18b-80ad-465d-9fef-b0c9bcb10577">
          </div>
   - Create a new text file with the .AT2 extension, in which the data within the file should be organized into 2 columns. **The first column** should contain **the time** in units of **seconds**, with decimals separated by **"."**, for example, **"0.055"**. **The second column** represents **the acceleration** values corresponding to each listed time, with acceleration measured in fractions of **g**, for example, **"1.235"**.
          <div align="center">
              <img src= "https://github.com/Normando1945/Seismic-Time-Response-of-SDOF/assets/62081230/67dcd4cd-e09b-41ff-9d7c-674702b0b17d">
          </div>
