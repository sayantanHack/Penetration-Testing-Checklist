# Mobile App Pentest 
> Mobile Application Penetration Testing - iOS and Andorid 

## Android

### labs
- [dvaa](https://code.google.com/archive/p/dvaa/)
- [android digital bank](https://github.com/CyberScions/Digitalbank)
- [dvfa](https://github.com/arroway/dvfa)
- [exploitme mobile](https://securitycompass.github.io/AndroidLabs/)
- [hacme bank android](https://www.mcafee.com/au/downloads/free-tools/hacme-bank-android.aspx)
- [insecurebank](github.com/dineshshetty/Android-InsecureBankv2)
- [ncn wargame](https://github.com/NocONName/Wargame_NcN2012)
- [owasp goatdroid](github.com/jackMannino/OWASP-GoatDroid-Project)
- [dodo Vulnerable Bank](https://github.com/CSPF-Founder/DodoVulnerableBank)
- [urdu app](http://urdusecurity.blogspot.com/2014/08/Exploiting-debuggable-android-apps.html)
- [appknox](https://github.com/appknox/vulnerable-application)
- [owasp crackme](https://github.com/OWASP/owasp-mstg/tree/master/Crackmes)

### Tools
- [frida](https://www.frida.re/) : hooking method , bypassing root detection , bypassing cert pinning, etc .
- [Burpsuite](https://portswigger.net/burp) : intercept request
- [apktool](https://ibotpeaches.github.io/Apktool/) : reversing 
- [Xposed Framework](http://repo.xposed.info/module/de.robv.android.xposed.installer) :  hooking native method 
- [Drozer](https://labs.mwrinfosecurity.com/tools/drozer/) : reverse engineerring 
- [Tcpdump](https://www.tcpdump.org/) : capture the traffic
- [adb , fastboot](https://developer.android.com/studio/releases/platform-tools)  : install apk , logging , push or pull file from devices.
- [sqlite browser](https://sqlitebrowser.org/) : to browse sqlite database.
- zipgrep : Searching purpose. 
- [jdgui](http://jd.benow.ca/) : code review
- dex2jar : reverse engineering purpose
- [modSF](https://github.com/MobSF/Mobile-Security-Framework-MobSF) : Dynamic Analysis
- [jarsigner](https://docs.oracle.com/en/java/javase/11/tools/jarsigner.html) : tool to sign and verify Java Archive (JAR/APK) files 

 
### Techniques
- Root Detecting Bypass
    - https://kyawthiha7.github.io/2018/12/27/Android-Root-Detection-Bypass/
    - https://resources.infosecinstitute.com/android-root-detection-bypass-reverse-engineering-apk/
    - https://resources.infosecinstitute.com/android-hacking-security-part-8-root-detection-evasion/#gref
    - http://repo.xposed.info/module/com.devadvance.rootcloak2
    - https://www.notsosecure.com/pentesting-android-apps-using-frida/
    - https://github.com/dineshshetty/Android-InsecureBankv2/blob/master/Walkthroughs/Bypass%20Android%20Root%20Detection.docx


- Cert Pinning Bypass
    - [intercepting-traffic-from-android-flutter-applications](https://blog.nviso.be/2019/08/13/intercepting-traffic-from-android-flutter-applications/)
    - [bypassing-root-ca-checks-in-flutter-based-apps-on-android](https://orangewirelabs.wordpress.com/2019/06/04/bypassing-root-ca-checks-in-flutter-based-apps-on-android/)
    - https://kyawthiha7.github.io/2017/09/27/Android-Cert-Pinning-Bypass/
    - https://blog.netspi.com/four-ways-bypass-android-ssl-verification-certificate-pinning/
    - https://github.com/ac-pm/SSLUnpinning_Xposed
    - http://sh3llc0d3r.com/certificate-pinning/

- Hooking native API
    - https://koz.io/android-substrate-c-hooking/
    - https://www.notsosecure.com/instrumenting-native-android-functions-using-frida/
    - https://resources.infosecinstitute.com/android-hacking-and-security-part-25-hooking-and-patching-android-apps-using-xposed-framework/
    - https://resources.infosecinstitute.com/android-hacking-and-security-part-22-hooking-and-patching-android-apps-using-cydia-substrate-extensions/
    - https://www.nccgroup.trust/sg/about-us/newsroom-and-events/blogs/2015/september/code-injection-on-android/
    - http://www.syssec-project.eu/m/page-media/158/syssec-summer-school-Android-Code-Injection.pdf

- Reverse Engineering
    - http://mobiletools.mwrinfosecurity.com/Using-Drozer-for-application-security-assessments/
    - https://pentestlab.blog/2017/02/06/reverse-engineering-android-applications/
    - https://github.com/OWASP/owasp-mstg/blob/master/Document/0x05c-Reverse-Engineering-and-Tampering.md
    - https://medium.com/@thomas_shone/reverse-engineering-apis-from-android-apps-part-1-ea3d07b2a6c
    - https://www.rsaconference.com/writable/presentations/file_upload/stu-w02b-beginners-guide-to-reverse-engineering-android-apps.pdf
    - https://resources.infosecinstitute.com/android-hacking-security-part-6-exploiting-debuggable-android-applications/#gref
    

### Tutorials & courses & books

- https://www.tutorialspoint.com/android_penetration_testing/index.asp
- https://gbhackers.com/android-application-penetration-testing
- https://www.udemy.com/android-hacking-and-penetration-testing/
- https://resources.infosecinstitute.com/android-application-security-testing-guide-part-1/
- [Android Applicaiton Hacker's Handbook](https://www.wiley.com/en-sg/Android+Hacker%27s+Handbook-p-9781118608647)
- [Mobile Application Hackers' Handbook](https://www.wiley.com/en-au/The+Mobile+Application+Hacker%27s+Handbook-p-9781118958506)


### CheckLists & Testing Guide

- https://github.com/OWASP/owasp-mstg/blob/master/Checklists/Mobile_App_Security_Checklist-English_1.1.2.xlsx
- https://github.com/OWASP/owasp-mstg
- https://gbhackers.com/penetration-testing-android-application-checklist/


### Public Exploits

- XXE : https://research.checkpoint.com/parsedroid-targeting-android-development-research-community/

- TinyCards RCE (CVE-2017-16905) : https://wwws.nightwatchcybersecurity.com/2018/01/04/rce-in-duolingos-tinycards-app-for-android-cve-2017-16905/

- Finding XSS in an html based android application : https://labs.detectify.com/2015/02/20/finding-an-xss-in-an-html-based-android-application/

- Broken Down SSL in Android Apps : https://www.owasp.org/images/7/77/Hunting_Down_Broken_SSL_in_Android_Apps_-_Sascha_Fahl%2BMarian_Harbach%2BMathew_Smith.pdf

## iOS
### jailbreak chart
   - [Jailbreak Chart](https://www.reddit.com/r/jailbreak/wiki/escapeplan/guides/jailbreakcharts)
   - [CanIJailbreak](https://canijailbreak.com/)
   
### Labs
   - [exploitme mobile](https://securitycompass.github.io/iPhoneLabs/)
   - [Damn Vulnerable iOS Applicatio (DVIA)](http://damnvulnerableiosapp.com/)
   - [owasp igoat](code.google.com/p/owasp-igoat/)
   - [owasp crackme](https://github.com/OWASP/owasp-mstg/tree/master/Crackmes)
   - [Myriam iOS sec App](https://github.com/GeoSn0w/Myriam)
   - [iOS online CTF](https://ivrodriguez.com/mobile-ctf/)

### Tools

- [Frida](https://frida.re) : hooking , bypassing , anlysis dynamic
- **GDB**  : Dynamic analysis
- [Cycript](http://iphonedevwiki.net/index.php/Cycript) : Dynamic analysis
- [Clutch](https://github.com/KJCracks/Clutch) : Static Analysis
- [dumpdecrypted](https://github.com/stefanesser/dumpdecrypted) : dumping decrypted iPhone Applications to a file
- [class-dump](http://stevenygard.com/projects/class-dump/) : dumping class info
- [class-dump-z](https://code.google.com/archive/p/networkpx/wikis/class_dump_z.wiki) : dumping class info
- **otool** : disassembler
- **strings** : print all the strings in a given binary. 
- **nm** : utility that displays the symbol table of a given binary.
- [cydia impactor](http://www.cydiaimpactor.com/) : for jailbreaking
- openssh (cydia)
- wget (cydia)
- Erica Utilities
- Snoop-it (cydia)
- unzip (cydia)
- adv-cmds (cydia)
- [usbmuxd](https://github.com/libimobiledevice/usbmuxd) : SSH over USB
- syslogd
- socat
- burpsuite 
- [iphonessh](https://github.com/rcg4u/iphonessh)
- [idb](https://www.idbtool.com)

### Techniques

- Jail Break Detection Bypass
    - https://www.notsosecure.com/bypassing-jailbreak-detection-ios/
    - https://www.theiphonewiki.com/wiki/Bypassing_Jailbreak_Detection
    - https://resources.infosecinstitute.com/ios-application-security-part-44-bypassing-jailbreak-detection-using-xcon/#gref
    - https://blog.attify.com/bypass-jailbreak-detection-frida-ios-applications/
    - https://www.c0d3xpl0it.com/2017/05/ios-jailbreak-bypass-using-needle.html
    - https://resources.infosecinstitute.com/ios-application-security-part-23-jailbreak-detection-evasion/
    - https://agostini.tech/2018/02/05/ios-application-security-part-three-bypassing-jailbreak-and-certificate-pinning-let-the-right-one-in/

- Cert Pinning Bypass
    - https://blog.netspi.com/four-ways-to-bypass-ios-ssl-verification-and-certificate-pinning/
    - https://www.nccgroup.trust/us/about-us/newsroom-and-events/blog/2015/january/bypassing-openssl-certificate-pinning-in-ios-apps/
    - https://github.com/vtky/Swizzler2/wiki/Case-Study:-SSL-Pinning
    - https://labs.nettitude.com/tutorials/using-frida-to-bypass-snapchats-certificate-pinning/


- Static and Dynamic Analysis
    - https://medium.com/@ansjdnakjdnajkd/dynamic-analysis-of-ios-apps-wo-jailbreak-1481ab3020d8
    - https://labs.mwrinfosecurity.com/assets/BlogFiles/Needle-Finding-Issues-within-iOS-Applications.pdf
    - https://medium.com/@drag0n/needle-analysis-of-ios-mobile-applications-cfd9e407c0d9

- Reverse Engineering
    - https://labs.mwrinfosecurity.com/blog/repacking-and-resigning-ios-applications/
    - https://github.com/OWASP/owasp-mstg/blob/master/Document/0x06c-Reverse-Engineering-and-Tampering.md
    - https://resources.infosecinstitute.com/ios-application-security-part-2-getting-class-information-of-ios-apps/
    - https://resources.infosecinstitute.com/penetration-testing-for-iphone-applications-part-5

- Misc
    - https://www.igeeksblog.com/how-to-sideload-apps-on-iphone-ipad-in-ios-10/

### Tutorials & courses & books
- [iOS Hacker's Handbook](https://www.amazon.com/iOS-Hackers-Handbook-Charlie-Miller/dp/1118204123)
- [iOS Application Security: The Definitive Guide for Hackers and Developers](https://www.amazon.com/iOS-Application-Security-Definitive-Developers/dp/159327601X)
- [Mobile Application Hackers' Handbook](https://www.wiley.com/en-au/The+Mobile+Application+Hacker%27s+Handbook-p-9781118958506)
- [Pentesting iOS Application by Pentester Academy](http://www.pentesteracademy.com/course?id=2)


### CheckLists & Testing Guide
- [OWASP MSTG](https://github.com/OWASP/owasp-mstg#ios-testing-guide)
- [SANS White Paper](https://www.sans.org/reading-room/whitepapers/testing/ipwn-apps-pentesting-ios-applications-34577)

### Public Exploits
- https://nvisium.com/blog/2014/07/30/swift-core-data-format-string-injection.html
- https://www.owasp.org/index.php/Mobile_Top_10_2016-Top_10

## Checklist

|  Categories	 |  Issues	 |                 
|-----|---|
| Network   | Certificate pinning |   
|           | Weak Cipher           |   
|           | API to negotiated with SSL  |   
|           | Leak Info via Side Channel   |   
|           | Improper Usage of HTTP Method |   
|           |              |         
| Server   | Authentication |   
|           |Injection           |    
|    | Session Management Issues |   
|           | Server banners           |    
|   | |   
|     Device      |       Insecure Data Storage (log, database, keychain, NSUserDefaults, cache, etc)|  
|    | JavaScript Execution(Webview) |  
|           | Code Quality (codesign , debug symbol,free security features, etc ..) |    
|           | Anti-reversing Detection(jailbreak/root detection, File integrity , Device Bonding ) |    


