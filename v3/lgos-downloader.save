#!/bin/bash

# Colors
red=$(echo -e '\e[31m')
green=$(echo -e '\e[32m')
brown=$(echo -e '\e[33m')
blue=$(echo -e '\e[34m')
purple=$(echo -e '\e[35m')
cyan=$(echo -e '\033[1m\e[36m')
yellow=$(echo -e '\e[1;33m')
white=$(echo -e '\e[1;37m')
dark_gray=$(echo -e '\e[1;30m')
light_red=$(echo -e '\e[1;31m')
light_green=$(echo -e '\e[1;32m')
light_blue=$(echo -e '\e[1;34m')
light_purple=$(echo -e '\e[1;35m')
light_cyan=$(echo -e '\e[1;36m')
light_gray=$(echo -e '\e[37m')
orange=$(echo -e '\e[38;5;202m')
light_orange=$(echo -e '\e[38;5;214m')
bold=$(echo -e '\033[1m')
reset=$(echo -e '\033(B\033[m')
unterstrich=$(echo -e '\033[4m')
# main

echo -e "
${green}${bold}Willkommen bei den offiziellen LinuxGuidesOS ISO Downloader!${reset}
************************************************************
Vielen Dank das sie sich für LinuxGuidesOS entschieden haben!
Dieses Tool lädt die ISO Datei von LinuxGuidesOS auf den schnellsten Download-Server herunter.

${red}${bold}Downloader-Version 3.0${reset}

${bold}${unterstrich}Quellen${reset}
- ${blue}https://linuxguides-os.de/${reset}
- ${blue}https://cd.linuxguides-os.de/${reset}
- ${blue}https://github.com/LinuxGuides-OS${reset}

${bold}${unterstrich}Downloadinformationen${reset}
- Download-Server: Offizieller Server (${blue}https://cd.linuxguides-os.de/${reset})
- Dateigröße: 1.5GB

Downloader geschrieben by Julian: ${blue}https://github.com/Juliaaan2502${reset}

${bold}Daten für das herunterladen werden gerade gesammelt. Habe etwas gedult!${reset}"
sleep 1
echo -e "${bold}Vorbereitung läuft!${reset}"
sleep 2

echo -e "${yellow}[ACHTUNG!] ${reset}${bold}Um LGOS herunterzuladen benötigen wir die Einwilligung, das du Fortfahren willst. Fortfahren? [Ja/Nein | J/N]"
read -r continue
if [[ $continue != "Ja" ]] && [[ $continue != "ja" ]]  && [[ $continue != "j" ]]  && [[ $continue != "J" ]]; then
        echo "Abgebrochen. Nichts zu tun"
        exit
fi


echo -e "${bold}**************Downloadvorgang...**************${reset}
"

# Zum HOME-Verzeichnis des Benutzers Navigieren
cd $HOME

# Neuen Ordner erstellen für die ISO Datei
mkdir LinuxGuidesOS-Downloader

# Im LGOS Ordner reinnavigieren
cd LinuxGuidesOS-Downloader/

# Neuen Ordner für die ISO erstellen
mkdir linuxguidesos-21_04_2-alpha

# In den Ordner reinnavigieren
cd linuxguidesos-21_04_2-alpha/

# ISO herunterladen (wget)
wget https://cd.linuxguides-os.de/alpha/LinuxGuides-OS-21.04.2_Alpha_Aphrodite.iso

sleep 2

echo -e "Geschafft! Deine ISO wurde erfolgreich heruntergeladen, und befindet sich in $HOME/LinuxGuidesOS-Downloader/linuxguidesos-21_04_2-alpha/"
sleep 0.5
echo -e "${bold}${red}Programm wird beendet, Temporäre Dateien werden bereinigt...${reset}"