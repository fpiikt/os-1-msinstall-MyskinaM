# Отчёт по Лабораторной работе №0 «Создание скрипта для автоматизации установки под Windows»<br/>
## Выполнил студент: Мыскина М. Группа P3369<br/>

### install-7-zip<br/>
    mkdir "C:\Program Files\7-Zip"
    msiexec /i 7z1900-x64.msi INSTALLDIR="C:\Program Files\7-Zip" REBOOT=ReallySuppress /passive /l*vs 7zip-log.txt

### install-paintnet<br/>
    paintnet_4.2.10.exe /auto "TARGETDIR=C:\Program Files\Graphics\Paint" DESKTOPSHORTCUT=1

### inkscape<br/>
    mkdir "C:\Program Files\Graphics\Inkscape"
    msiexec /i inkscape-0.92.4-x64.msi INSTALLDIR="C:\Program Files\Graphics\Inkscape" REBOOT=ReallySuppress /qr /l*vs inkscape-log.txt

### install-LibreOffice<br/>
    msiexec /i LibreOffice_6.4.2_Win_x64.msi REBOOT=ReallySuppress /passive /l*vs libreoffice-install-log.txt
    msiexec /i LibreOffice_6.4.2_Win_x64_helppack_ru.msi REBOOT=Force /passive

### install-notepad<br/>
    start /wait npp.7.8.5.Installer.x64.exe /S

### install-java<br/>
    mkdir "C:\Java\JRE"<br/>
    JavaSetup8u241.exe INSTALLDIR=C:\Java\JRE WEB_ANALYTICS=Disable WEB_JAVA=Enable /s /L C:\Users\Noyt2\Downloads\jre-log.txt
