# FloatingGlucose
FloatingGlucose is a windows program aiming to display your current bloogsugars live on your desktop.

A transparent popup window will be displayed in the bottom right corner of your desktop, with your current blood glucose values fetched from your nightscout site.

## Screenshot
![Image of Floating glucose in action](https://s9.postimg.org/ut4dnjnfj/floatingglucose_0_9_7_beta7.png)

## Installation
Download The Setup.exe of the latest release, [which you can find here](https://github.com/dabear/FloatingGlucose/releases/) and run it. You should normally just install it to the default directory which is C:\Program Files (x86)\FloatingGlucose. 





## Running the program and configuring your nightscout endpoint
After configuring the nightscout installation URL, double click on FloatingGlucose.exe to open the program. A settings dialog will appear where you can enter your nightscout url.

## Hidden / Nice to Know features
* You can drag the window around and place it where you want to.
* To show the settings again, please right click the notification area icon or the app. A menu will pop up allowing you to access the application settings
* The same pop up menu can be used to temporarily disable sound alarms.

## Debugging
Having troubles with crashes or with the widget not updating? Please make sure you have enabled exception logging to stderr (in the configfile) then run the program from command line:

```bash
cd c:\glucose
glucose.exe 2> glucose_log.txt
```

Then open glucose_log.txt

## Settings files
Please note that you can edit the settings from inside the application. If you still need to access the conig files directly, please go to either of these locations

* Installation directory, and open FloatingGlucose.exe.config
* %localappdata%\Bjorns_opensource_utils and locate user.config

The user.config file will override any values inside the FloatingGlucose.exe.config file

