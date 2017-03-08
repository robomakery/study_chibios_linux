# study_chibios_linux
   
This is a sibling repository of ["study_chibios"](https://github.com/bus710/study_chibios).  
However, this repo aims Linux users.
  
## Maintainer
  
SJ Kim  
- Profile: [bus710.net](http://bus710.net)  
- Contact: <<bus710@gmail.com>>  
   
## Index

- [Hardware](#Hardware)
- [Installation](#installation)
- [Setting Eclipse](#setting-eclipse)
- [Project importing](#project-importing)
- [Compiling and debugging](#compiling-and-debugging)

## Hardware

Below Hardwares are required.
- A host machine (with linux)
- A target machine (VESC in our case. STM32F4-DISCO is good, too)
- A STLINK-V2 (or a SWD compatible board)
- A Power Supply Unit (Should be able to supply 12V 3A)

## Installation
  
ChibiOS project provides a very convenient tool, which is ChibiStudio for windows users. Linux (and Mac) users need to install Eclipse, Cross tool chain, and OpenOCD by themself though, it is not too complex (Actually we even don't need to compile any tool). Here, I assume that you have a PC with Vanilla **Ubuntu 16.04**.   

### Basic tools

After install Ubuntu, you may follow below commands.

```
$ sudo apt-get update
$ sudo apt-get install build-essential
$ sudo apt-get install eclipse
$ sudo apt-get install openocd
$ sudo apt-get install git
```

### Cross tool chain

In order to get the ARM cross compiler, you may follow below commands.
  
```
$ sudo add-apt-repository ppa:team-gcc-arm-embedded/ppa
$ sudo apt-get update
$ sudo install gcc-arm-embedded
```

### Eclipse Neon and plug-ins
  
Although we already installed Eclipse from the official repository, we will use a newer Eclipse, which is "Neon". (However, by installing Eclipse with command line, we can easily have required tools like JDK for Eclipse.)  
  
In order to get Eclipse Neon, 
- visit this link [>>>](http://www.eclipse.org/downloads/packages/eclipse-ide-cc-developers/neon2).  
- If you click "Download" button on the web page, it might give you a flie **"eclipse-inst-linux64.tar.gz"**. 
- Extract the file (either using gunzip in the terminal or right clicking in the file browser).  
- Go to the directory and run the installer by right clicking "eclipse-inst" in the file browser. 
- Choose **"C/C++"** environment.
- That will automatically install Eclipse Neon but you can update by visiting **"Help > Check for Updates"**.

Once the Eclipse installation is done, 
- You can run Eclipse and navigate to **"Help > Install New Software"**.  
- In the Dialog, you can find a text input **"Work with:"**. 
- Type Neon, then it will give few choice. Click **"Neon - httpL//download.eclipse.org/releases/neon"**.
- Below that, you also can fine a text input **"type text filter"**.
- Type 
  
## Project importing
  
bbb
  
## Compiling and debugging
  
ccc 
  
## References
   
[1] http://www.chibios.org/dokuwiki/doku.php  
[2] http://vedder.se/2015/01/vesc-open-source-esc/  

