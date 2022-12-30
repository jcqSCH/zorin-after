# ZORIN OS 16.2 CORE: after install
Things to do after installing Zorin Operating System. <br/>
Tested version: Zorin OS 16.2 Core (based on Ubuntu 22.04 LTS)
<br/>
https://zorin.com/os/download/

<br/>

## 1 ➜ DOWNLOAD .DEB OR SNAP PACKAGES
**VS Code:** https://code.visualstudio.com/download/ <br/> 
**PowerShell:** https://github.com/PowerShell/PowerShell#get-powershell <br/> 
**Spotify:** https://www.spotify.com/br/download/linux/ <br/>
**Google Chrome:** https://www.google.com/chrome/browser/desktop/ <br/>
**OpenRGB:** https://openrgb.org/releases.html

<br/>

## 2 ➜ RUN COMMANDS IN TERMINAL
	sudo apt-get update && 

	# sudo apt install ubuntu-unity-desktop -y && 		# OPTIONAL

	sudo apt-get update && 

	# sudo apt-get install plank -y && 			# OPTIONAL
	# sudo apt-get install libreoffice-style-sifr -y && 	# OPTIONAL
	# sudo apt-get install unity-tweak-tool -y && 		# OPTIONAL
	
	sudo apt-get install grub-customizer -y && 
	sudo apt-get install python3-pip -y && 
	sudo apt-get install software-properties-common -y && 
	sudo apt-get install ubuntu-restricted-extras -y && 
	sudo apt-get install unace unrar zip unzip p7zip-full p7zip-rar sharutils rar -y && 
	sudo apt-get install compizconfig-settings-manager -y && 
	sudo apt-get install bleachbit -y && 
	sudo apt-get install git-all -y && 
	sudo apt-get install qbittorrent -y && 
	sudo apt install qt5-style-plugins -y && 
	sudo apt install numix-gtk-theme numix-icon-theme -y && 
	sudo apt install curl -y && 
	sudo apt install nautilus-admin -y && 

	sudo apt-get update && 

	sudo add-apt-repository ppa:slimbook/slimbook -y && 
	sudo add-apt-repository ppa:inkscape.dev/stable -y && 
	sudo add-apt-repository ppa:plushuang-tw/uget-stable -y && 
	sudo add-apt-repository ppa:rvm/smplayer -y && 

	sudo apt-get update && 

	sudo apt-get install slimbookbattery -y && 
	sudo apt-get install inkscape -y && 
	sudo apt-get install uget -y && 
	sudo apt-get install smplayer smplayer-themes smplayer-skins -y && 
	sudo apt-get install mpv -y

> Join lines using Sublime Text or VS Code shortcut `CTRL + J`. Then run all commands at once.

<br/>

### 2.1 ➜ REALTEK RTL8821CU DRIVER
	sudo apt-get install build-essential dkms git-all bc -y 
	
	# OPEN DRIVER FOLDER IN TERMINAL #
	
	sudo su
	make
	sudo make install
	sudo reboot

- Source 1: https://github.com/brektrou/rtl8821CU
- Source 2: https://www.youtube.com/watch?v=tyLMzIAxj-4

<br/>

### 2.2 ➜ WPS OFFICE FULL VERSION (BR LANGUAGE)
	wget -qO - "https://winunix.github.io/debian/public.key" | sudo apt-key add -
	echo "deb https://winunix.github.io/debian focal main" | sudo tee /etc/apt/sources.list.d/winunix-focal.list

	sudo apt-get update && 

	sudo apt install fonts-3rd-party -y && 
	sudo apt install wps-office-full -y

- Source: https://plus.diolinux.com.br/t/wps-office-completo-em-portugues/18836

<br/>

## 3 ➜ SETTINGS

### 3.1 – Plank:
Download themes: https://github.com/kennyh7279/plank-themes

|  SETTINGS   |             …             |
|       ---        |            ---            |
|  Theme:          |  Shade                    |
|  Icons:          |  68                       |
|  Zoom:           |  125                      |

>**Ordem:** Arquivos, Terminal, Spotify, Firefox, VS Code, Writer, Calculadora, Unity Tweak, Configuraçes do Sistema

<br/>

### 3.2 – Fontes do Sistema:
|  Configurações        |            …            |
|          ---          |           ---           |
|  Fonte padrão:        |  Inter Regular ➜ 11,5   |
|  Fonte de documento:  |  Inter Regular ➜ 11,5   |
|  Fonte monoespaçada:  |  Maax Mono Regular ➜ 13 |
|  Fonte de título:     |  Inter Medium ➜ 12      |
|           ⠀           |            ⠀            |
|  Suavização:          |  RGBA                   |
|  Fator escalonamento: |  1,00                   |
|  Hinting:             |  Médio                  |

<br/>

### 3.3 – VS Code
	{
	    "workbench.colorTheme": "Monokai",
	    "workbench.iconTheme": "material-icon-theme",
	    "editor.fontFamily": "'Code Saver', 'Apercu Pro Mono', 'Anonymous Pro Minus', 'Droid Sans Mono', 'monospace', monospace, 'Droid Sans Fallback'",
	    "window.zoomLevel": 0.8,
	    "editor.fontWeight": "500"
	}
>**Font Size:** 14

<br/>

|  Extensões        |                      …                      |
|        ---        |                     ---                     |
|  Atalhos:         |  Sublime Text Keymap and Settings Importer  |
|  Ícones:          |  Material Icon Theme, by Philipp Kief       |
|  Tema:            |  Monokai Pro, by monokai                    |
|  Terminal:        |  PowerShell                                 |

<br/>

### 3.4 – Spotify:
	sudo gedit /usr/share/applications/spotify.desktop
>**Substituir:** Exec=spotify %U <br/>
>**Por:** Exec=spotify %U --force-device-scale-factor=1.25

<br/>

### ~3.5 – Sumblime Text~

~{
"color_scheme": "Packages/Panda Syntax Sublime/Panda/panda-syntax.tmTheme",
"font_face": "Anonymous Pro Minus",
"font_size": 12,
"ignored_packages":
[
"Vintage"
],
"theme": "Adaptive.sublime-theme",
"ui_scale": 1.5
}~

<br/>

### ~3.6 – Firefox (não é mais necessário):~
	about:config
>~**Substituir:** layout.css.devPixelsPerPx; -1~ <br/>
>~**Por:** layout.css.devPixelsPerPx; 1.25~

<br/>

### ~3.7 – Google Chrome (não é mais necessário):~
	sudo gedit /usr/share/applications/google-chrome.desktop
>~**Substituir:** Exec=/usr/bin/google-chrome-stable %U~ <br/>
>~**Por:** Exec=/usr/bin/google-chrome-stable --force-device-scale-factor=1.175 %U~

<br/>

## 4 ➜ HINTS

### 4.1 – Open folder as Administrator:
	sudo nautilus /usr/share/icons
> Edit `/usr/share/icons` above, if you want to access another directory.

<br/>

### 4.2 – Unmount the Windows partition while logged into Ubuntu or another Ubuntu based OS:
	mount -o ro /dev/sda2
> Edit `sda2` above if that's not the partition your Windows is installed on.
- Source: http://askubuntu.com/questions/335909/error-mounting-dev-sda2-at-media

<br/>

### 4.3 – Check the video driver installed
	lspci -k | grep -EA3 'VGA|3D|Display'
> The `VGA|3D|Display` stands for `INTEL|NVIDIA|AMD` respectively.

<br/>

### 4.4 – Fix the bug "Can't move files to the trash":
	sudo chown -R “$USER” ~/.local/share/Trash
> Edit the `“$USER”` part above and enter your Ubuntu username (without quotes).
- Source: http://askubuntu.com/questions/288513/cant-move-files-to-the-trash

<br/>

### 4.5 – Recover lost GRUB after a Windows update (dual boot):
	bcdedit /set "{bootmgr}" path \EFI\ubuntu\grubx64.efi
> Logged into Windows, run the command above in PowerShell as Administrator.
- Source: https://askubuntu.com/questions/655011/windows-10-upgrade-kills-grub-and-boot-repair-doesnt-help

<br/>
