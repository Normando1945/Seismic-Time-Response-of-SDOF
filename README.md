<div align="center">
    <img src="https://github.com/Normando1945/Normando1945.github.io/assets/62081230/1ac0bf1d-67cd-43f6-87b0-141417a606db">
</div>

## Introduction:
This software application is straightforward, designed to compute the time response of underdamped single-degree-of-freedom (1 DOF) systems using the discrete Beta Newmark method. Importantly, this software should not be seen as a replacement for formal classroom instruction but rather as a tool to supplement it. It was developed mainly for underdamped systems subjected to non-periodic and non-harmonic external excitations, like earthquakes. The primary purpose of this tool is to provide students with a visual aid, helping them comprehend how structures behave during actual seismic events. In doing so, users should be aware of the inherent simplifications and approximations in the 1 DOF Beta-Newmark calculation.

Moreover, it is essential for users of this academic software to have sufficient knowledge regarding the step-by-step time-domain response calculation of 1 DOF systems. To familiarize oneself with the mathematical foundation, you can visit the repository **[Brief Summary of Undergraduate Structural Dynamics](https://github.com/Normando1945/Normando1945.github.io)**, where you will find an academic summary on this topic.

### Installation Steps:
* For optimal performance, install **[7-Zip](https://www.7-zip.org/)** (free software).
  
    <div align="center">
        <img src= "https://github.com/Normando1945/TH_SDOF_Carlos_Celi/assets/62081230/301c9c5b-0307-4e11-a5b6-863d3ccf079d">
    </div>
* Using **[7-Zip]**, **[WinRAR]**, or a similar software, unzip the file **<u>"TH_SDOF_CC_setup.7z.001"</u>** to your desired location.
  
    <div align="center">
        <img src= "https://github.com/Normando1945/TH_SDOF_Carlos_Celi/assets/62081230/0fff86ee-f313-4d6f-9778-7e0436596e5a">
    </div>
    
* Note: Ensure all files downloaded from the repository are in the same folder.
* Once unzipped, an executable file named **"TH_SDOF_CC_setup.exe"** will appear. Double-click this file to initiate the installation process. Simply follow the on-screen instructions thereafter.
* Please read and accept the terms and conditions.
  <div align="center">
        <img src= "https://github.com/Normando1945/TH_SDOF_Carlos_Celi/assets/62081230/c63ab5d4-36ba-4c9e-ac93-76d2aa9c1215">
  </div>
* Enter the installation key. Password: **<u>soloparausoacademico<u>**
  <div align="center">
      <img src= "https://github.com/Normando1945/TH_SDOF_Carlos_Celi/assets/62081230/03de11a9-e7a3-4520-ad4b-23f8f865ba2c">
  </div>
* Select your preferred directory.
  <div align="center">
      <img src= "https://github.com/Normando1945/TH_SDOF_Carlos_Celi/assets/62081230/7aea7151-c8e9-42b9-9286-000507fa421a">
  </div>
* If you wish, you can create a shortcut on your desktop.
  <div align="center">
      <img src= "https://github.com/Normando1945/TH_SDOF_Carlos_Celi/assets/62081230/2207bdfa-f8db-4a77-b4b5-72f1d2e08217">
  </div>
  * Proceed with the installation.
  <div align="center">
      <img src= "https://github.com/Normando1945/TH_SDOF_Carlos_Celi/assets/62081230/9ccb5ac5-8350-404c-bcbc-9a384548e0a7">
  </div>

  View of the main screen.
  <div align="center">
      <img src= "https://github.com/Normando1945/TH_SDOF_Carlos_Celi/assets/62081230/80e65558-c1f5-400c-929a-f577c670cddc">
  </div>
  


## User Manual:

El uso es bastante simple. se debe ingresar los parametros requeridos en cada uno de los espacios requieridos.

* **Period of motion [from 0.01 to 4]** : Se debe ingresar el periodo fundamental de vibración del sistema de 1gdl que se requiera conocer su respuesta en el tiempo. El presente software, se limita a calcular rangos de peridos estructurales desde **0.01** segundos hasta **4** segundos. Sin embargo el algoritmo permite calcular la respuesta para cualquier periodo mayor a **0** segundos [Periodos menores a **0.01** segundos o mayores a **4** segundos puede generar resultados de baja confiafiablidad por la inherente convergencia y estabilidad del método de calculo].
  
* **Damping Ratio [from 0.01 to 0.99]** : Se debe ingresar el valor de amoritiguamiento viscoso equivalente del sistema estructural de 1GDL que se desea analizar. Comprendiendo que el algoritmo se basa en una solución discreta paso a paso en el dominio del tiempo de sistemas subamoritiguados, por tal motivo el rango de valores de amortiguamiento va desde **$\zeta$ = 0.01 a 0.99**. potencialmente se puede usar **$\zeta$ = 0** para describir un sistema conservativo. No se puede emplear  **$\zeta$ >= 1** pues se emularía sistemas sobreamortiguados lo cual implica una inestabilidad numerica en la solucuión paso a paso del presente software.

* **Files in the Folder** : Muestra la cantidad de archhivos en format .AT2 que se encuentran en la carpeta donde se instalo el software **"TH_SDOF_CC_setup.exe"**, oficialmente junto con la instalación se añaden 7 registros sísmicos reales, lsitados a continuación:
  - AMT_201604162359_E_100.AT2
  - Artificial.AT2
  - ChiChi_longt.AT2
  - ChiChi_tranv.AT2
  - Friulli.AT2
  - Hollister.AT2
  - Loma_Prieta_1989.AT2

* **Record Selected from the database in the root of the folder, for this data base from 1 to "n"** : Se debe ingresar el **número** del registro sísmico que se desea emplear como exitación externa. para ello se debe observar **"Files in the Folder"**.
* **PLAY** : Boton que inicializa el calculo.
* **Random data** : boton que permite llenar todos los campos necesarios con valores aleatorios dentro de los rangos antes especificados.

### Resultados.
El presente software academico presenta los resultados de forma gráfica en dos pantallas indiviuales interactivas. La primera pantalla contiene el registro sísmico empleado junto con la respuesta estructural en desplazamiento, velocidad y aceleración. La segunda pantalla muestra una animación [no a escala] con la respuesta en aceleración del sistema de 1GDL analizado.

### Ejemplo.
  <div align="center">
      <img src= "https://github.com/Normando1945/TH_SDOF_Carlos_Celi/assets/62081230/52487eec-35a0-4eb0-801e-3ecb2d4d1102">
  </div>
  <div align="center">
      <img src= "https://github.com/Normando1945/TH_SDOF_Carlos_Celi/assets/62081230/82ed8568-5ced-4d3e-a2c1-f492be83ea65">
  </div>

## Importante: 
Cada vez que se desee realizar un nuevo análisis, se debe dar click en **"Close Windows"**
