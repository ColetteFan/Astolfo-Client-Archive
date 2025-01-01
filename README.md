# Astolfo-Client-Archive
An Archive from Astolfo Client Latest!

# How to Run Astolfo
How to Run the client?

1. Install Zulu 8 or BellSoft JDK 8.
2. Install one from theses JDK and go in "Astolfo-Latest" Folder.
3. go in "start.bat" file and click to open as Notepad
4. Click "CTRL A + DEL" and change the text that will be just below (This only for who will use Bellsoft JDK! for those who will use Zulu 8 don't need to do this!)
5. Save and Click 2 times in "start.bat" (Note: "start.bat" need to be on top of all files!)
6. Your Astolfo Client must have CMD open at all times (i think the cmd open all time is only for who use Bellsoft Jdk)
7. Enjoy Astolfo Client! (Rip Script cuz the document is lost 😭)


Text To put in "start.bat":
@echo off
SET JDK_PATH="C:\Program Files\BellSoft\LibericaJDK-8\bin\javaw.exe"

echo JDK: %JDK_PATH%

SET SCRIPT_DIR=%~dp0

%JDK_PATH% -Dos.name="Windows 11" -Dos.version="10.0" ^
-XX:HeapDumpPath=%SCRIPT_DIR%Astolfo.heapdump ^
-Djava.library.path=%SCRIPT_DIR%natives ^
-Dminecraft.launcher.brand=minecraft-launcher ^
-Dminecraft.launcher.version=3.2.13 ^
-Dminecraft.client.jar=%SCRIPT_DIR%Astolfo.jar ^
-cp "%SCRIPT_DIR%libs;%SCRIPT_DIR%Astolfo.jar" ^
-Xmx4G -XX:+UnlockExperimentalVMOptions -XX:+UseG1GC ^
-XX:G1NewSizePercent=20 -XX:G1ReservePercent=20 -XX:MaxGCPauseMillis=50 -XX:G1HeapRegionSize=32M ^
-Dlog4j.configurationFile=%SCRIPT_DIR%assets\log_configs\client-1.7.xml ^
start.Main --username Free --version 1.8.9 ^
--gameDir "%APPDATA%\.minecraft" ^
--assetsDir "%APPDATA%\.minecraft\assets" --assetIndex 1.8 ^
--uuid 887341c45ea94dd3bae9bb00502124f1 --accessToken changeme ^
--userProperties {} --userType msa



you still can use Astolfo in HvH servers, Bad Ac servers, or idk?
