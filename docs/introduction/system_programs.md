---
layout: default
---
## System Programs  
System programs are server and GUI programs that provide various services in Innova. There are two types of system programs:
 
1. Service programs that run as background processes on the Innova server or other computers in the Innova system.  
2. WinUI programs that run the user interfaces on IPCs, PDAs or other devices.

The base Innova configuration includes five system programs.

### Program Manager  
Progman.exe manages the execution of background programs on the Innova server and on other servers and PCs in the Innova system.
 
The system has one program manager for every server to manage the execution of programs.

### Base Services 
**Mp5services.exe** provides the four system-wide services described below. There can only be one mp5services program installed in each Innova system. 
 
* Message service - Used to route SSI packets between programs.  
* Licensing service - Provides support functions for the Innova licensing system.  
* Device configuration service - Allows users to configure device parameters.  
* Installation service - Supports the client software installation and distribution framework.

### Device Router  
**Mp5router.exe** provides device communication services. Instead of connecting directly to each device, a program can connect to the device through this program. This provides two main benefits:
 
1. It allows multiple programs to interact with devices with limited connection capabilities. For example, M2200 devices only support one incoming socket connection per port.  
2. It allows you to easily monitor and log device communications.

### GUI Services  
**Mp5guiservices.exe** provides services needed for the different graphical user interfaces to run. The following services are installed by default:
 
* Authentication session factory - Creates authentication sessions that are used to authenticate users when they log on through a GUI client.  
* Authorizer service - Used to determine the user's access level to different applications. Other services use this service to restrict access and filter information.  
* Data factory - Creates DataSource objects that are used in client programs to present data to end users.  
* Document manager - The backbone of the document system. Its function is to provide and store documents.  
* Persistent storage service - Stores and restores user preferences, including window locations, and visible grid columns.  
* UI Configuration service - Creates the menu tree shown in the GUI client based on the user's acceess level.   
* Base GUI actions service - A compilation of different actions that are activated through a client but need to run on the server side.  * Process GUI actions service - Process counterparts to the Base GUI actions service.

### Process Manager  
**Procman.exe** provides the following process system services: 
 
* Unit operation service - A data processing service. Allows remote clients to execute unit operations over .NET remoting. 
* Site service - Allows clients to interact with sites over .NET remoting. This service can be used to change production day parameters at runtime.  
* Process unit service - Allows clients to interact with process units over .NET remoting.  Use this service to change the activity or PO on a process unit or to get notified when the activity or PO changes.  
* Export-import service - Exports and imports data records, such as pack records, to and from Innova.
