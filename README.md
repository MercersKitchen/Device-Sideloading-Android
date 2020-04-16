# Device Sideloading Android
Final Project in CS10

---

# Developing in Android: Resources, Exemplars, and Examples

Website: http://ketai.org/

Teacher Only Files: <a href="https://drive.google.com/drive/folders/1BE18BxXR0JU8w9lnIFvAqntXuChsK2Jo">See Mr. Mercer</a>

---

# To Include

Progressions
- Hello World: focused on network connections, OS configurations, and drivers
- Simple Touch Screen Interaction: Click counter with random colours including possible game with timer
  - Simple way to put text on screen
  - Color by numbers: line art generation, preloaded pictures
  - Side stroller
- CS10: Drawing program with background changes
- CS10: Music Player
- CS20: Weather Program
- CS20: Tic Tac Toe
- CS30: Pong
- Pure Java, messaging program
- Android-specific like Android Studio
- Google Play Account

---

# Java: Processing-Java, Processing-Android, and Pure Java
CAUTION: this installation has a few steps and should be done last
- used on all machines
Note: JDK Version from Oracle should be already installed or verified, reference above

Program Installation Overview
- Processing: processing-3.5.4-windows64.zip, https://processing.org/download/, 20200416

Optional Installation (Note Necessary for Processing Right Now, 20200416)
- Android Studio (Uses Pure Java, CS30), https://developer.android.com/studio/
  - NOTE: Android Studio's SDK GUI Manager made Processing Installation easier, not necessary as of 20180614
  - When installing SDK, update JDK and Manager for KitKat, Android 4.4 (most legacy that is tested to work)
    - Installing all OS Options will use a lot of Hard Drive Space (>200Gb), be careful about your overall hard drive size
  - Note: when choosing an Android OS, choose the one on your device, search your device to locate what is installed and updated

Processing Installation
- Download ZIP File, extract with 7-Zip (already installed above)
- Move folder to Program files (C:\Program Files)
- Create shortcut to processing.exe in the Start Menu
  - https://www.howtogeek.com/howto/6463/stupid-geek-tricks-how-to-open-the-start-menu-folder-in-windows-7/

Customize Processing Java & Android (Download Packages using Contribution Manager)
- Menu: Sketch / Import Library / Add Library
- Libraries to Add (Note: additional instruction websites for some libraries available, reference below, last accessed 20180631)
  - Note: all libraries have instructions available on Processing.org/reference
  - Ketai (http://ketai.org/, text available from Pragmatic Book Shelf, "Rapid Android Development")
  - Minim (http://code.compartmental.net/minim/, additional YouTube Videos, etc. are available)
    - Currently the Sound Library since "Sound" is not supported in Windows 10, 20200416
  - OpenCV (https://opencv.org/)
  - Interfascia (http://interfascia.berg.industries/)
  - Sound (Built in Processing Library: https://processing.org/reference/libraries/sound/)
    - Currently not supported in Windows 10, DO NOT USE (use Minim instead), 20200416
- Modes to Add: Android Mode (note: requires Processing 3.3.7, 20180613)
- Tools to Add
  - Git Manager
  - Upload to Pi
- Examples to Add (Accessed through Menu: File / Examples)
  - Note: 20180614 some examples were not available
  - Getting Started with Processing
  - Learning Processing 2nd Edition
  - Processing for Android
  - Processing Handbook 2nd Edition
  - The Nature of Code

Restart might be required: close program and restart Processing using Start Menu shortcut
- Ensures all libraries, etc., added to correct folder in Program Files
- Able to Open c:\Program Files \ processing-3.3.7
- Navigate to Libraries folder and visually verify package installations

Other Libraries Exist: Processing.org/reference
- Search for these and read about what they do, then start to use them
- Google Search these to see if additional websites or texts exist
- Note: if a text exists, able to Google Search filetype:pdf to see if reading is acceptable before purchasing and supporting the author

*Processing-JAVA Mode is now ready for use*

## Following Instructions require Android Device for further installation and configuration

**CAUTION**: Student installation of Processing-Android is being broken by "School's Network"
- Possible Reason: part of Processing-IDE is being installed to the C-Drive, other part is being installed to a server drive
- Working Solution: Only use non-school computer, everything installs to C-Drive

Processing-Android Mode Dependencies and Testing
- MUST have android device with USB Debugging Enabled (Google Search to enable this on your device, if necessary)
  - Double CAUTION: rooting a device has had issues in the past (if you know what rooting is, then you are also aware of the issues)
  - To Activate Developer Options: click "Build Number" (Settings / About)
  - To Activate USB Debugging: see Developer Options / USB Debugging
- Instructional Website & Text References: http://android.processing.org/

Processing IDE: change Java Mode to Android Mode
- Once Android Mode selected, follow prompts if Android Mode is not installed (this means install the mode :) )
  - Download SDK Manually (does not need Android Studio SDK GUI Manager, 20180613)
  - Accept Licenses
- Verify pathway of installation (record this! you might need it later)
  - Example: C:\Users\MercersKitchen\Documents\Processing\android\sdk\extras\google\usb_driver
  - Example: C:\Users\Mark\AppData\Local\Android\sdk
- Note this will take a while, be prepared
- Select Java Mode again: will need to restart machine and Processing-Java is better to start from here
- Close Processing IDE

Android Driver Installations: doubleClick to install, may need to Unzip first
- Install Samsung Driver first, then Universal Driver (worked as of 20180615)
  - Optional: only install the Universal Driver until you have a Samsung device
- For Samsung install: SAMSUNG_USB_Driver_for_Mobile_Phones.exe (Last Accessed 201502)
  - http://downloadcenter.samsung.com/content/SW/201410/20141017131240597/SAMSUNG_USB_Driver_for_Mobile_Phones.exe?utm_source=gsmmaniak.pl&utm_medium=artykul&utm_campaign=techmaniak.pl
- For other Android Devices: UniversalAdbDriverSetup.msi (Last Accessed 20180614)
  - Universal ABD Drivers: https://adb.clockworkmod.com/
    - Double Click
    - Install for Everyone
    - Remember to be patient
  - Caution: Windows 7 Only
    - Windows "doesn't believe" this is a safe driver, doesn't want a virus; these steps used successfully 20180615
    - Open "Devices and Printers" (Windows 7), in Control Panel / Devices and Printers
      - Ensure device is plugged in and USB Debugging is enabled
    - Under "Device Properties", navigate to where driver software can be loaded/changed/seen
    - Click "Update Driver"
    - Follow the Prompts and navigate menus
      - "Browse My Computer" and "Let me pick..."
    - Select device you have
    - Click on all and load the whole list: clockworkmod
      - Future Research: read how and why to do this
    - In the left pane: sorted by manufacture, look for clockworkmod
    - INSTALL IT :)
      - Now: device will freak out and implode :) (Quote from student who helped write instruction list)
    - After device reassembles itself, popup asking permission for this computer to debug via USB
    - Click YES

Restart Entire Machine, ensures all pathways are correct (especially environmental pathways)
- Troubleshooting Example: Set Path to Android SDK Path (in C:\Users\Mark\AppData\Local\Android\sdk)

Restart Processing-Android (reselect Processing-Android)
- Plug in device to WINDOWS
  - Follow Prompts like "Always allow USB Debugging From this Computer"
- Normal Processing IDE Boot: no prompts for downloads, etc. (besides optional updates)
- Verify in Android / Device that device is connected
- Processing-Android ready to side-load to device

Download and Run Processing-Android "Hello World" Sketch (Sketches are name for Processing coded programs, from Processing)
- See AcerHelloWorld
- Run on Device (but not on Emulator)
- Remember about device permission (not activated on this Hello World Sketch, but might be needed in future)
  - Android / Sketch Permissions
Click only the ones needed by your code
"Opens Cyber Security Door"
  - CAUTION: if these are not used, the door is open for inappropriate use from the "wild"
- Ensure device is connected and you can see it in Processing-Android Menu: Sketch
- Run the Sketch on the Device
  - Ensure device does NOT activate screen lock
  - Remember, be patient, to build project Processing-Android will need to download dependencies from Internet
- Play with the Touch Screen Program
- To dismount Processing-Android from device, after Sketch is Loaded and working
  - Stop the Sketch executing
  - Power-down device to "Dismount the Drive" (currently Task-bar does not have dismount function)
  - Unplug Device from Computer

Verify Processing-Android Program is installed on device
- Power-ON Device, not connected to computer
- Find tile with name of program
- Double Click the file
  - CAUTION: to stop the program without an EXIT-Button, use the HOME Button and the "Show Running Program", then swipe off
  - Alternatively: Settings / Apps / [YourProgram] / Force Stop

Final Test ... Finally: Testing Pure JAVA (Windows 7 or Windows 10)
- See Testing JavaJDK
- Move Folder to Pure Java Programs in My Documents (or where you will store Pure Java Files)
- Shift-Right-Click on the folder, "Open command window here"

```Java
javac HelloWorld.java
java HelloWorld
```

---

Exporting Processing-JAVA or ANDROID Programs as stand-a-lone executables
- WINDOWS will work on non-school computer (everything installed to C-Drive), tested 20180613
- Linux will work on non-school computer (everything installed to C-Drive), tested 20180613
- MAC will work on non-school computer (everything installed to C-Drive), tested 20180613

---
