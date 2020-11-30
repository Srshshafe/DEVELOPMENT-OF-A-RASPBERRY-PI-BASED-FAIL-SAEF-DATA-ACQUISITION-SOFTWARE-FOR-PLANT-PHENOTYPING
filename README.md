# DEVELOPMENT-OF-A-RASPBERRY-PI-BASED-FAIL-SAEF-DATA-ACQUISITION-SOFTWARE-FOR-PLANT-PHENOTYPING


The code is a part of my master project, for further details and instructions, please contact me at als123@usask.ca

Abstract
Modern plant phenotyping is a trending topic in plant breeding science which often uses non-destructive and digital technologies to gather data about a plant’s environmental conditions as well as its interaction with the ever-changing environment in which it is growing. Understanding this process helps identify key factors that lead to better crop management and breeding.
Plant phenotyping usually requires monitoring many variables in a large-scale field and collecting data on sensors and modules in use such as different kind of cameras, GPS module.
Some of the most common data acquisition methods used in plant phenotyping is unmanned aerial vehicles (UVAs) or drone, satellite, phenomobile and handheld devices. 
One of the main challenges in plant phenotyping is a reliable data management and data storage software, due to the increasingly amount of data being collected on farm fields. Using computers with high processing power and fast storage hard drives for data collection is considered normal and usually little effort is allocated towards improving the agility of software.
Developing an efficient, reliable and fail-safe data acquisition software for plant phenotyping, in addition to  validating its performance and consistency under various conditions is the main goal of this project.
Hardware components consist of a low-cost credit-card sized Raspberry pi computer, two Full HD webcams, a GPS module, a display, a mouse and keyboard. A python script is developed as the data acquisition and data visualization software which runs on the Raspberry Pi computer to collect data on GPS module and webcams at user-defined time intervals.
Plant phenotyping often requires a high throughput data collection platform where data on several sensors and modules need to be collected at the same time. For instance, in order to accurately geo-tag images with corresponding GPS data in every time interval, GPS and webcams data need to be collected with least possible delay.
Hard drive memories are much cheaper than random access memories (RAMs) and have relatively much larger storage capacity. However, saving data on a hard drive is relatively much slower than RAM, causing conflicts for geo-tagging captured images with corresponding GPS data. 
RAM is much faster than a hard drive, however, it is suitable for storing data on a short-term basis. Some plant phenotyping data acquisition methods rely on RAM for data collection and only transfer data to hard drive at the end of data collection. Data storage on RAM  has some limitations such as total loss of data in case any errors happen within the operating system, defects in the software itself, or any accident leading to computer power loss.
the possihility of losing data during data collection ought to be eliminated, as there are sometimes a narrow window of time to collect data during data collection.
To safely save data on a hard drive and without delay, a data cache layer may be designed to improve performance by buffering data from cameras and sensors. The method of buffering data  allows data to be stored on RAM while data is being processed and written on hard drive in the background. This method which is used in most modern DSLR cameras is often expensive and difficult to implement.
In our presented method an optimized code is developed that takes up a small memory and stores the collected data on GPS module and cameras on RAM and then transfer the collected data from RAM to a hard drive memory while data collection is in progress. The write speed of the hardware does not have to be known as the algorithm will measure the execution time in every loop and keep the loop delay as defined by user.

Alireza Shafe
