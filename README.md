

   <h2> <div align="center"><b> Modified Spotify Client for Windows </b></div> </h2>

<h1>System requirements</h1>

- <strong>OS: Windows 7-11</strong>
- <strong>Spotify: Recommended official version [1.1.99.878](https://cutt.ly/8EH6NuH)</strong>
- <strong>For Windows Desktop only (Microsoft store version is not suitable).</strong>
- <strong>PowerShell: 3 or higher</strong>

<h1>Features</h1>

- <strong>Blocks all banner, video and audio ads in the client</strong>
- <strong>Unlocks the skip function of any track</strong>
- <strong>Hiding podcasts, episodes and audiobooks from the homepage (optional)</strong>
- <strong>Block Spotify automatic updates (optional)</strong>
- <strong>Automatic clearing of audio cache (optional)</strong>
- <strong>More experimental features have been activated see the full list</strong>
- <strong>Disabled Sentry Prevented Sentry from sending console log/error/warning to Spotify developers</strong>
- <strong>Disabled logging (Stopped various elements to log user interaction)</strong>
- <strong>Removed RTL rules (Removed all right-to-left CSS rules to simplify CSS files)</strong>
- <strong>Code minification</strong>

<h1>Fast installation / Update</h1>
<h3>Choose installation type:</h3>
<details>
<summary><small>Usual installation</small></summary><p>
  
  #### During installation, you need to confirm some actions, also contains:

  - All experimental features included

  <h4> </h4>
  
#### Just download and run [Install.bat](https://raw.githack.com/ALBINPRAVEEN/Spotify-Win/main/Install.bat)

or

#### Run The following command in PowerShell:

```ps1
[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; (iwr -useb 'https://raw.githubusercontent.com/ALBINPRAVEEN/Spotify-Win/main/Install.ps1').Content | iex
```

</details>
  
  
<details>
<summary><small>Automatic full installation</small></summary><p>
  
  <h4>Automatic installation without confirmation, what does it do?</h4> 
  
  - Automatic removal of Spotify MS if it was found 
  - Automatic installation of the recommended version of Spotify (if another client has already been found, it will be installed over) 
  - Hiding podcasts/episodes/audiobooks from the homepage 
  - Automatic blocking of Spotify updates
  - All experimental features included
  - After the installation is completed, the client will autorun.
  
<h4> </h4>

#### Just download and run [Install_Auto.bat](https://raw.githack.com/ALBINPRAVEEN/Spotify-Win/main/scripts/Install_Auto.bat)

or

#### Run The following command in PowerShell:

```ps1
[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; iex "& { $((iwr -useb 'https://raw.githubusercontent.com/ALBINPRAVEEN/Spotify-Win/main/Install.ps1').Content) } -confirm_uninstall_ms_spoti -confirm_spoti_recomended_over -podcasts_off -cache_off -block_update_on -start_spoti"
```

</details>

<details>
<summary><small>Other types of installations</summary><p>

<details>
<summary><small>Automatic basic installation</small></summary><p>
  
  #### Automatic basic installation without confirmation, what does it do? 
  
  - Automatic removal of Spotify MS if it was found 
  - Automatic installation of the recommended version of Spotify (if another client has already been found, it will be installed over)
  - After the installation is completed, the client will autorun
  
<h4> </h4>

#### Just download and run [Install_Basic.bat](https://raw.githack.com/ALBINPRAVEEN/Spotify-Win/main/scripts/Install_Basic.bat)

or

#### Run The following command in PowerShell:

```ps1
[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; iex "& { $((iwr -useb 'https://raw.githubusercontent.com/ALBINPRAVEEN/Spotify-Win/main/Install.ps1').Content) } -confirm_uninstall_ms_spoti -confirm_spoti_recomended_over -podcasts_on -cache_off -block_update_off -exp_standart -hide_col_icon_off -start_spoti"
```

</details>

<details>
<summary><small>Installation for premium</small></summary><p>
  
  #### Usual installation only without ad blocking, for those who have a premium account, also contains:

  - All [experimental features](https://github.com/ALBINPRAVEEN/Spotify-Win/discussions/50) included

  <h4> </h4>
  
#### Just download and run [Install_Prem.bat](https://raw.githack.com/ALBINPRAVEEN/Spotify-Win/main/scripts/Install_Prem.bat)

or

#### Run The following command in PowerShell:

```ps1
[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; iex "& { $((iwr -useb 'https://raw.githubusercontent.com/ALBINPRAVEEN/Spotify-Win/main/Install.ps1').Content) } -premium"
```

</details>

<details>
<summary><small>Installing with Scoop</small></summary><p>
  
  #### Installing Spotify via the Scoop package manager includes:

  - Automatic removal of Spotify MS if it was found 
  - Automatic installation of the recommended version of Spotify (if another client has already been found, it will be installed over) 
  - Hiding podcasts/episodes/audiobooks from the homepage  
  - Automatic blocking of Spotify updates
  - All [experimental features](https://github.com/ALBINPRAVEEN/Spotify-Win/discussions/50) included 
  
  <h4> </h4>
  
#### Installing Spotify with Scoop
Just run these commands in the command prompt or powershell:
<br>
<br>```scoop bucket add nonportable```
<br>```scoop install spotx-np```

#### Updating Spotify with Scoop

To update Spotify or check for updates run this command in the command prompt or powershell:

```scoop update spotify-np```

#### Uninstalling SpotX with Scoop

To fully uninstall SpotX and Spotify run this command in the command prompt or powershell:

```scoop uninstall spotify-np```

</details>


<details>
<summary><small>Installing with parameters</small></summary><p>

You can specify various parameters for a more flexible installation, more [details here](https://github.com/ALBINPRAVEEN/Spotify-Win/discussions/60)

</details>

</details>

<h1>Uninstall</h1>

- Just run [Uninstall.bat](https://raw.githack.com/ALBINPRAVEEN/Spotify-Win/main/Uninstall.bat)

or

- Reinstall Spotify ([Full uninstall Spotify](https://github.com/ALBINPRAVEEN/Uninstall-Spotify) recommended)

<h1>FAQ</h1>

- Read [FAQ](https://telegra.ph/SpotX-FAQ-09-19)

<h1>Credits</h1>

- This repository partially uses <a href="1">BlockTheSpot</a>, and also some tricks were taken from <a href="https://github.com/khanhas/spicetify-cli">spicetify-cli</a>, many thanks to the contributors
