@echo off

::Created by @XPnerd

set "scriptver=1.2.8"
title PowerUser Tools v%scriptver%

for /f "tokens=6 delims=[]. " %%i in ('ver') do set build=%%i

if %build% LSS 1507 (
    echo ================================================================================================
    echo This script is compatible only with Windows 10 Build 1507 and later.
    echo ================================================================================================
    echo.
    pause
    goto :EOF
)
reg query HKU\S-1-5-19 1>nul 2>nul
if %ERRORLEVEL% equ 0 goto :START_SCRIPT

echo =====================================================
echo This script must be executed as administrator.
echo =====================================================
echo.
echo Press any key to exit.
pause >nul
goto :EOF

:START_SCRIPT
set "scriptver=1.2.8"
title PowerUser Tools v%scriptver% 
goto :CHOICE_MENU

:CHOICE_MENU
cls
set "choice="
echo.
echo 1 - Apps
echo 2 - Commands
echo.
echo 3 - Quit without making any changes
echo.
set /p choice="Choice: "
echo.
if /I "%choice%"=="1" goto :APPS
if /I "%choice%"=="2" goto :COMMANDS
if /I "%choice%"=="3" goto :EOF
goto :CHOICE_MENU

:APPS
cls
set "choice="
echo.
echo 1 - Offline Insider Enroll
echo 2 - ViVe Tool Whether Widgit
echo.
echo 3 - Quit without making any changes
echo.
set /p choice="Choice: "
echo.
if /I "%choice%"=="1" goto :OFFLINE_INSIDER_ENROLL
if /I "%choice%"=="2" goto :VIVE_TOOL
if /I "%choice%"=="3" goto :EOF
goto :APPS

:COMMANDS
cls
set "choice="
echo.
echo 1 - System Info
echo 2 - Test Signing
echo.
set /p choice="Choice: "
echo.
if /I "%choice%"=="1" goto :SYSTEM_INFO
if /I "%choice%"=="2" goto :TEST_SIGNING
goto :COMMANDS

:OFFLINE_INSIDER_ENROLL (
@setlocal DisableDelayedExpansion
@echo off

::Edited by @XPnerd
::Credits to @abbodi1406

set "scriptver=2.6.2"

set "_cmdf=%~f0"
if exist "%SystemRoot%\Sysnative\cmd.exe" (
setlocal EnableDelayedExpansion
start %SystemRoot%\Sysnative\cmd.exe /c ""!_cmdf!" "
exit /b
)
if exist "%SystemRoot%\SysArm32\cmd.exe" if /i %PROCESSOR_ARCHITECTURE%==AMD64 (
setlocal EnableDelayedExpansion
start %SystemRoot%\SysArm32\cmd.exe /c ""!_cmdf!" "
exit /b
)
set "SysPath=%SystemRoot%\System32"
if exist "%SystemRoot%\Sysnative\reg.exe" (set "SysPath=%SystemRoot%\Sysnative")
set "Path=%SysPath%;%SystemRoot%;%SysPath%\Wbem;%SysPath%\WindowsPowerShell\v1.0\"

for /f "tokens=6 delims=[]. " %%i in ('ver') do set build=%%i

if %build% LSS 17763 (
    echo =============================================================
    echo The script is compatible only with Windows 10 v1809 and later
    echo =============================================================
    echo.
    pause
    goto :EOF
)

reg query HKU\S-1-5-19 1>nul 2>nul
if %ERRORLEVEL% equ 0 goto :START_SCRIPT1

echo =====================================================
echo This script needs to be executed as an administrator.
echo =====================================================
echo.
pause
goto :EOF

:START_SCRIPT1
set "FlightSigningEnabled=0"
bcdedit /enum {current} | findstr /I /R /C:"^flightsigning *Yes$" >nul 2>&1
if %ERRORLEVEL% equ 0 set "FlightSigningEnabled=1"

:CHOICE_MENU1
cls
title OfflineInsiderEnroll v%scriptver%
set "choice="
echo.
echo 1 - ReadMe.md
echo.
echo 2 - Enroll to Dev Channel
echo 3 - Enroll to Beta Channel
echo 4 - Enroll to Release Preview Channel
echo.
echo 5 - Stop receiving Insider Preview builds
echo 6 - Quit without making any changes
echo 7 - Back to PowerUser Tools menu
echo.
set /p choice="Choice: "
echo.
if /I "%choice%"=="1" goto :README1
if /I "%choice%"=="2" goto :ENROLL_DEV1
if /I "%choice%"=="3" goto :ENROLL_BETA1
if /I "%choice%"=="4" goto :ENROLL_RP1
if /I "%choice%"=="5" goto :STOP_INSIDER1
if /I "%choice%"=="6" goto :START_SCRIPT1
if /I "%choice%"=="7" goto :START_SCRIPT
goto :CHOICE_MENU1

:ENROLL_RP1
set "Channel=ReleasePreview"
set "Fancy=Release Preview Channel"
set "BRL=8"
set "Content=Mainline"
set "Ring=External"
set "RID=11"
goto :ENROLL1

:ENROLL_BETA1
set "Channel=Beta"
set "Fancy=Beta Channel"
set "BRL=4"
set "Content=Mainline"
set "Ring=External"
set "RID=11"
goto :ENROLL1

:ENROLL_DEV1
set "Channel=Dev"
set "Fancy=Dev Channel"
set "BRL=2"
set "Content=Mainline"
set "Ring=External"
set "RID=11"
goto :ENROLL1

:RESET_INSIDER_CONFIG1
reg delete "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\Account" /f
reg delete "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\Applicability" /f
reg delete "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\Cache" /f
reg delete "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\ClientState" /f
reg delete "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\UI" /f
reg delete "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\Restricted" /f
reg delete "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\ToastNotification" /f
reg delete "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\WindowsUpdate\SLS\Programs\WUMUDCat" /f
reg delete "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\WindowsUpdate\SLS\Programs\Ring%Ring%" /f
reg delete "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\WindowsUpdate\SLS\Programs\RingExternal" /f
reg delete "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\WindowsUpdate\SLS\Programs\RingPreview" /f
reg delete "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\WindowsUpdate\SLS\Programs\RingInsiderSlow" /f
reg delete "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\WindowsUpdate\SLS\Programs\RingInsiderFast" /f
reg delete "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Policies\DataCollection" /f /v AllowTelemetry
reg delete "HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\Windows\DataCollection" /f /v AllowTelemetry
reg delete "HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\Windows\WindowsUpdate" /f /v BranchReadinessLevel
goto :EOF

:ADD_INSIDER_CONFIG1
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\WindowsUpdate\Orchestrator" /f /t REG_DWORD /v EnableUUPScan /d 1
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\WindowsUpdate\SLS\Programs\Ring%Ring%" /f /t REG_DWORD /v Enabled /d 1
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\WindowsUpdate\SLS\Programs\WUMUDCat" /f /t REG_DWORD /v WUMUDCATEnabled /d 1
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\Applicability" /f /t REG_DWORD /v EnablePreviewBuilds /d 2
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\Applicability" /f /t REG_DWORD /v IsBuildFlightingEnabled /d 1
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\Applicability" /f /t REG_DWORD /v IsConfigSettingsFlightingEnabled /d 1
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\Applicability" /f /t REG_DWORD /v IsConfigExpFlightingEnabled /d 0
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\Applicability" /f /t REG_DWORD /v TestFlags /d 32
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\Applicability" /f /t REG_DWORD /v RingId /d %RID%
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\Applicability" /f /t REG_SZ /v Ring /d "%Ring%"
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\Applicability" /f /t REG_SZ /v ContentType /d "%Content%"
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\Applicability" /f /t REG_SZ /v BranchName /d "%Channel%"
if %build% LSS 21990 reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\UI\Strings" /f /t REG_SZ /v StickyXaml /d "<StackPanel xmlns="^""http://schemas.microsoft.com/winfx/2006/xaml/presentation"^""><TextBlock Style="^""{StaticResource BodyTextBlockStyle }"^"">This device has been enrolled to the Windows Insider program using OfflineInsiderEnroll v%scriptver%. If you want to change settings of the enrollment or stop receiving Insider Preview builds, please use the script. <Hyperlink NavigateUri="^""https://github.com/abbodi1406/offlineinsiderenroll"^"" TextDecorations="^""None"^"">Learn more</Hyperlink></TextBlock><TextBlock Text="^""Applied configuration"^"" Margin="^""0,20,0,10"^"" Style="^""{StaticResource SubtitleTextBlockStyle}"^"" /><TextBlock Style="^""{StaticResource BodyTextBlockStyle }"^"" Margin="^""0,0,0,5"^""><Run FontFamily="^""Segoe MDL2 Assets"^"">&#xECA7;</Run> <Span FontWeight="^""SemiBold"^"">%Fancy%</Span></TextBlock><TextBlock Text="^""Channel: %Channel%"^"" Style="^""{StaticResource BodyTextBlockStyle }"^"" /><TextBlock Text="^""Content: %Content%"^"" Style="^""{StaticResource BodyTextBlockStyle }"^"" /><TextBlock Text="^""Telemetry settings notice"^"" Margin="^""0,20,0,10"^"" Style="^""{StaticResource SubtitleTextBlockStyle}"^"" /><TextBlock Style="^""{StaticResource BodyTextBlockStyle }"^"">Windows Insider Program requires your diagnostic data collection settings to be set to <Span FontWeight="^""SemiBold"^"">Full</Span>. You can verify or modify your current settings in <Span FontWeight="^""SemiBold"^"">Diagnostics &amp; feedback</Span>.</TextBlock><Button Command="^""{StaticResource ActivateUriCommand}"^"" CommandParameter="^""ms-settings:privacy-feedback"^"" Margin="^""0,10,0,0"^""><TextBlock Margin="^""5,0,5,0"^"">Open Diagnostics &amp; feedback</TextBlock></Button></StackPanel>"
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\UI\Visibility" /f /t REG_DWORD /v UIHiddenElements /d 65535
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\UI\Visibility" /f /t REG_DWORD /v UIDisabledElements /d 65535
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\UI\Visibility" /f /t REG_DWORD /v UIServiceDrivenElementVisibility /d 0
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\UI\Visibility" /f /t REG_DWORD /v UIErrorMessageVisibility /d 192
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Policies\DataCollection" /f /t REG_DWORD /v AllowTelemetry /d 3
if defined BRL reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\Windows\WindowsUpdate" /f /t REG_DWORD /v BranchReadinessLevel /d %BRL%
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\UI\Visibility" /f /t REG_DWORD /v UIHiddenElements_Rejuv /d 65534
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\UI\Visibility" /f /t REG_DWORD /v UIDisabledElements_Rejuv /d 65535
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\UI\Selection" /f /t REG_SZ /v UIRing /d "%Ring%"
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\UI\Selection" /f /t REG_SZ /v UIContentType /d "%Content%"
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\UI\Selection" /f /t REG_SZ /v UIBranch /d "%Channel%"
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\UI\Selection" /f /t REG_DWORD /v UIOptin /d 1
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\Applicability" /f /t REG_SZ /v RingBackup /d "%Ring%"
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\Applicability" /f /t REG_SZ /v RingBackupV2 /d "%Ring%"
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\Applicability" /f /t REG_SZ /v BranchBackup /d "%Channel%"
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\Cache" /f /t REG_SZ /v PropertyIgnoreList /d "AccountsBlob;;CTACBlob;FlightIDBlob;ServiceDrivenActionResults"
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\Cache" /f /t REG_SZ /v RequestedCTACAppIds /d "WU;FSS"
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\Account" /f /t REG_DWORD /v SupportedTypes /d 3
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\Account" /f /t REG_DWORD /v Status /d 8
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\Applicability" /f /t REG_DWORD /v UseSettingsExperience /d 0
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\ClientState" /f /t REG_DWORD /v AllowFSSCommunications /d 0
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\ClientState" /f /t REG_DWORD /v UICapabilities /d 1
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\ClientState" /f /t REG_DWORD /v IgnoreConsolidation /d 1
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\ClientState" /f /t REG_DWORD /v MsaUserTicketHr /d 0
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\ClientState" /f /t REG_DWORD /v MsaDeviceTicketHr /d 0
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\ClientState" /f /t REG_DWORD /v ValidateOnlineHr /d 0
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\ClientState" /f /t REG_DWORD /v LastHR /d 0
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\ClientState" /f /t REG_DWORD /v ErrorState /d 0
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\ClientState" /f /t REG_DWORD /v PilotInfoRing /d 3
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\ClientState" /f /t REG_DWORD /v RegistryAllowlistVersion /d 4
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\ClientState" /f /t REG_DWORD /v FileAllowlistVersion /d 1
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\UI" /f /t REG_DWORD /v UIControllableState /d 0
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\UI\Selection" /f /t REG_DWORD /v UIDialogConsent /d 0
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\UI\Selection" /f /t REG_DWORD /v UIUsage /d 26
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\UI\Selection" /f /t REG_DWORD /v OptOutState /d 25
reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\UI\Selection" /f /t REG_DWORD /v AdvancedToggleState /d 24
reg add "HKEY_LOCAL_MACHINE\SYSTEM\Setup\WindowsUpdate" /f /t REG_DWORD /v AllowWindowsUpdate /d 1
reg add "HKEY_LOCAL_MACHINE\SYSTEM\Setup\MoSetup" /f /t REG_DWORD /v AllowUpgradesWithUnsupportedTPMOrCPU /d 1
reg add "HKEY_LOCAL_MACHINE\SYSTEM\Setup\LabConfig" /f /t REG_DWORD /v BypassRAMCheck /d 1
reg add "HKEY_LOCAL_MACHINE\SYSTEM\Setup\LabConfig" /f /t REG_DWORD /v BypassSecureBootCheck /d 1
reg add "HKEY_LOCAL_MACHINE\SYSTEM\Setup\LabConfig" /f /t REG_DWORD /v BypassStorageCheck /d 1
reg add "HKEY_LOCAL_MACHINE\SYSTEM\Setup\LabConfig" /f /t REG_DWORD /v BypassTPMCheck /d 1
reg add "HKEY_CURRENT_USER\SOFTWARE\Microsoft\PCHC" /f /t REG_DWORD /v UpgradeEligibility /d 1
if %build% LSS 21990 goto :EOF
(
echo Windows Registry Editor Version 5.00
echo.
echo [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\UI\Strings]
echo "StickyMessage"="{\"Message\":\"Device Enrolled Using OfflineInsiderEnroll\",\"LinkTitle\":\"\",\"LinkUrl\":\"\",\"DynamicXaml\":\"^<StackPanel xmlns=\\\"http://schemas.microsoft.com/winfx/2006/xaml/presentation\\\"^>^<TextBlock Style=\\\"{StaticResource BodyTextBlockStyle }\\\"^>This device has been enrolled to the Windows Insider program using OfflineInsiderEnroll v%scriptver%. If you want to change settings of the enrollment or stop receiving Insider Preview builds, please use the script. ^<Hyperlink NavigateUri=\\\"https://github.com/abbodi1406/offlineinsiderenroll\\\" TextDecorations=\\\"None\\\"^>Learn more^</Hyperlink^>^</TextBlock^>^<TextBlock Text=\\\"Applied configuration\\\" Margin=\\\"0,20,0,10\\\" Style=\\\"{StaticResource SubtitleTextBlockStyle}\\\" /^>^<TextBlock Style=\\\"{StaticResource BodyTextBlockStyle }\\\" Margin=\\\"0,0,0,5\\\"^>^<Run FontFamily=\\\"Segoe MDL2 Assets\\\"^>^&#xECA7;^</Run^> ^<Span FontWeight=\\\"SemiBold\\\"^>%Fancy%^</Span^>^</TextBlock^>^<TextBlock Text=\\\"Channel: %Channel%\\\" Style=\\\"{StaticResource BodyTextBlockStyle }\\\" /^>^<TextBlock Text=\\\"Content: %Content%\\\" Style=\\\"{StaticResource BodyTextBlockStyle }\\\" /^>^<TextBlock Text=\\\"Telemetry settings notice\\\" Margin=\\\"0,20,0,10\\\" Style=\\\"{StaticResource SubtitleTextBlockStyle}\\\" /^>^<TextBlock Style=\\\"{StaticResource BodyTextBlockStyle }\\\"^>Windows Insider Program requires your diagnostic data collection settings to be set to ^<Span FontWeight=\\\"SemiBold\\\"^>Full^</Span^>. You can verify or modify your current settings in ^<Span FontWeight=\\\"SemiBold\\\"^>Diagnostics ^&amp; feedback^</Span^>.^</TextBlock^>^<Button Command=\\\"{StaticResource ActivateUriCommand}\\\" CommandParameter=\\\"ms-settings:privacy-feedback\\\" Margin=\\\"0,10,0,0\\\"^>^<TextBlock Margin=\\\"5,0,5,0\\\"^>Open Diagnostics ^&amp; feedback^</TextBlock^>^</Button^>^</StackPanel^>\",\"Severity\":0}"
echo.
)>"%SystemRoot%\oie.reg"
regedit /s "%SystemRoot%\oie.reg"
del /f /q "%SystemRoot%\oie.reg"
goto :EOF

:ENROLL1
echo Applying changes...
call :RESET_INSIDER_CONFIG1 1>NUL 2>NUL
call :ADD_INSIDER_CONFIG1 1>NUL 2>NUL
bcdedit /set {current} flightsigning yes >nul 2>&1
echo Done.

echo.
if %FlightSigningEnabled% neq 1 goto :ASK_FOR_REBOOT1
echo Press any key to exit.
pause >nul
goto :EOF

:STOP_INSIDER1
echo Applying changes...
call :RESET_INSIDER_CONFIG1 1>nul 2>nul
bcdedit /deletevalue {current} flightsigning >nul 2>&1
echo Done.

echo.
if %FlightSigningEnabled% neq 0 goto :ASK_FOR_REBOOT1
echo Press any key to exit.
pause >nul
goto :EOF

:ASK_FOR_REBOOT1
set "choice="
echo A reboot is required to finish applying changes.
set /p choice="Would you like to reboot your PC? (Y/N) "
if /I "%choice%"=="Y" shutdown -r -t 0
goto :EOF


:README1
cls
echo =============================================================
echo Description
echo =============================================================
echo OfflineInsiderEnroll is a simple Windows Command Prompt script to
echo enable access to the Windows Insider Program on machines not signed
echo in with Microsoft Account.
echo.
echo This script is compatible only with Windows 11 or Windows 10 version
echo 1809 and later.
echo.
echo =============================================================
echo Usage
echo =============================================================
echo This script requires administrative priviliges to run. You can simply 
echo execute it by right clicking it - Run as Administrator.
echo.
echo Installation and configuration changes
echo After starting, the script offers selection of Windows Insider Program 
echo channels. To make a selection, press a letter coresponding to option 
echo you choose and press ENTER.
echo.
echo If the machine was not enrolled to the Insider Program, you will get 
echo prompted to restart your machine to enable Microsoft Flight Signing
echo which is required by Windows Insider Program.
echo.
echo Notice: Windows Insider Program requires telemetry to be set to Full.
echo After enrolling your machine to the Windows Insider Program please
echo make sure that your diagnostic data collection settings are set to Full.
echo Some Insider Preview builds may not get offered in Windows Update
echo if you do not have correct telemetry settings.
echo.
echo You can verify or modify your telemetry settings as follows:
echo.
echo Windows 11: Settings - Privacy and Security - Diagnostics "&" feedback
echo.
echo Windows 10: Settings - Privacy - Diagnostics "&" Feedback
echo.
echo Restoring Windows Insider Program to default options. To restore 
echo Windows Insider Program to default settings simply choose Stop 
echo receiving Insider Preview builds in OfflineInsiderEnroll Script. You will
echo get prompted to reboot, because this option will disable Microsoft
echo Flight Signing.
echo.
echo =============================================================
echo How does this work?
echo =============================================================
echo This script takes advantage of undocumented TestFlags registry value.
echo If this value is set to 0x20, all access to online Windows Insider services
echo gets disabled. Because of this, we can set our own Windows Insider
echo Preview configuration without being overriden by the contact to the
echo service. Since Windows Update does not check if machine is actually
echo enrolled to the program, you will get offered Insider Preview builds
echo by just setting correct values in the registry.
echo.
echo =============================================================
echo License
echo =============================================================
echo This project is licensed under the "MIT License". See "LICENSE" for details.
echo.
echo.

:SECOND_CHOICE_MENU1
set "choice="
echo.
echo 1 - Main Menu
echo 2 - License
echo 3 - Quit without making any changes
echo.
set /p choice="Choice: "
echo.
if /I "%choice%"=="1" goto :START_SCRIPT1
if /I "%choice%"=="2" goto :LICENSE1
if /I "%choice%"=="3" goto :EOF
goto :SECOND_CHOICE_MENU1

:LICENSE1
cls
echo ===================================================
echo abbodi1406/offlineinsiderenroll is licensed under the MIT License
echo ===================================================
echo A short and simple permissive license with conditions only requiring preservation of copyright and license notices. 
echo Licensed works, modifications, and larger works may be distributed under different terms and without source code.
echo.
echo.
echo [Permissions]                                [Limitations]
echo Commercial use                               Liability
echo Modification                                 Warranty
echo Distribution
echo Private use
echo.
echo.
echo ==============================================
echo MIT License
echo ==============================================
echo.
echo Copyright (c) 2021 abbodi1406
echo.
echo Permission is hereby granted, free of charge, to any person obtaining a copy
echo of this software and associated documentation files (the "Software"), to deal
echo in the Software without restriction, including without limitation the rights
echo to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
echo copies of the Software, and to permit persons to whom the Software is
echo furnished to do so, subject to the following conditions:
echo.
echo The above copyright notice and this permission notice shall be included in all
echo copies or substantial portions of the Software.
echo.
echo THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
echo IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
echo FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
echo AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
echo LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
echo OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
echo SOFTWARE.
echo.
echo.
goto :THIRD_CHOICE_MENU1

:THIRD_CHOICE_MENU1
set "choice="
echo.
echo 1 - Main Menu
echo 2 - Quit without making any changes
echo.
set /p choice="Choice: "
echo.
if /I "%choice%"=="1" goto :START_SCRIPT1
if /I "%choice%"=="2" goto :EOF
goto :THIRD_CHOICE_MENU1
)

:SYSTEM_INFO (
systeminfo
echo.
echo.
echo Press any key to return to main menu.
pause >nul
goto START_SCRIPT
)

:TEST_SIGNING
cls
set "choice="
echo.
echo 1 - Toggle on
echo 2 - Toggle off
echo.
set /p choice="Choice: "
echo.
if /I "%choice%"=="1" bcdedit -set TESTSIGNING ON
if /I "%choice%"=="2" bcdedit -set TESTSIGNING OFF
echo Press any key to return to main menu.
pause >nul
goto :START_SCRIPT

:VIVE_TOOL
cls
echo Adding Configs,
echo Please wait...
echo.
echo.
vivetool addconfig 34301415 2
vivetool addconfig 36553793 2
vivetool addconfig 36226054 2
vivetool addconfig 36226456 2
echo.
Done.
echo Press any key to return to main menu.
pause >nul
goto :START_SCRIPT
