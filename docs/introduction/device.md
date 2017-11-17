---
layout: default
---
### Device
A machine or piece of equipment that is connected to Innova so that it can be configured, controlled and monitored. Innova collects data from devices and generates reports to monitor yield, throughput, quality, capacity and labor efficiency.
 
* A device can be a physical device, like a scale, grader, PDA, scanner, or printer.  
* It can also be software, like a Windows printer driver.

For devices, it is important to note that some devices may be part of a line.  
```xml
<DataRoot>
	<Marel.Mp5.Process.Services.Process.ProcessUnitService.Configuration>
		<!--List of process units for which to reset the productnum counter when a new process period starts.-->
		<ResetProductNumOnPrperiodPrunits />
		<!--List of process units for which to reset the processnum counter when a new process period starts.-->
		<ResetProcessNumOnPrperiodPrunits />
		<!--List of process units for which to start new process period when PO changes.-->
		<NewPrperiodOnPOChangePrunits />
	</Marel.Mp5.Process.Services.Process.ProcessUnitService.Configuration>
	<ConfigSections>
		<Section name="Marel.Mp5.Process.Services.Process.ProcessUnitService.Configuration" type="Marel.Mp5.Process.Services.Process.ProcessUnitService+Configuration, Marel.Mp5.Process.Services" serializer="Marel.Common.Serialization.XmlDataSerializer, Marel.Common" />
	</ConfigSections>
</DataRoot>
```
