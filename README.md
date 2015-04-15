#NFC-WISP Hardware
---
### Version
1.0

#Resource
---
###Tutorial & Discussion: 
See NFC-WISP wiki: http://nfc-wisp.wikispaces.com/

Please send your questions and suggestions to the [**discussion board**](http://nfc-wisp.wikispaces.com/wiki/messages) in wiki!!!	    

###Firmware repository:
https://github.com/wisp/nfc-wisp-fw.git

###Andriod App repository
Use cell-phone to updates E-ink display when loading **nfc-eink-img-update-demo** firmware 

https://github.com/wisp/nfc-reader-app.git		

#Introduction
---
1. This version of NFC-WISP is the first released hardware version. It is a software-defined NFC-Wireless-Identification-Sensing-Platform with other enhanced feature. (The older pre-release design file is taged as **"pre-release"**)

2. Feature:
  *  Communication carrier frequency: 13.56Mhz 
  *  Protocol: 
            Hardware demoudulator can support ISO 14443-Type A/B and ISO 15693 NFC protocol, however, our [latestest firmware](https://github.com/wisp/nfc-wisp-fw.git) only implements  and fully tests ISO 14443-Type B protocol, the ISO 15693 is particially implemented but not fully implemented yet.

  *  Mode: NFC-WISP hardware can be configured in 3 different mode: 
  	- **Passive** (battery-free) --- disconnect battery or remove Rz0
  	- **Semi-passive** (battery-assistant) -- connect battery and keep Rz0. The battery may not need to be charged, it only used for storage wireless power during communication **with** NFC reader and offer power later for high-power application.

  	- **Active** (battery-powered) -- connect battery and keep Rz0. Charge the battery for running tasks **without** NFC reader.

        **Note**: For semi-passive/active mode, a rechargable li-ion thin film battery will be connected to NFC-WISP, it can be directlly charged by **NFC reader** or **NFC-enabled cell-phone (may need custermized app to send more power)** and **13.56Mhz wireless charging system**  (see paper: Enabling Seamless Wireless Power Delivery in Dynamic Environment,Sample, A.P., Waters, B.H. ; Wisdom, S.T. ; Smith, J.R.).




