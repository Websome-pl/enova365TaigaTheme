### Taiga theme installation guide for enova365 Web version 2512.9.11 or lower

**⚠️ Important**

Starting with enova365 version **2512.10.12**, this installation guide is no longer applicable.
Please switch to the [**enova365_2512.10.12 or later**](https://github.com/Websome-pl/enova365TaigaTheme/tree/enova365_2512.10.12) branch to use the updated installation guide for newer versions of enova365.

If you are still using the old version, please proceed with the instructions below:

First [these files](https://github.com/Websome-pl/CustomTaigaThemeEnova365Websome/tree/main/TaigaTheme) need to be downloaded and put in this enova365 directory: Soneta.Products.Web.Standard\wwwroot-Standard\css\palettes

Secondly in this directory: Soneta.Products.Web.Standard file appsettings.json needs to be modified:

```
"DefaultThemes": {
      "Default": "Base",
	      "TEST2504": "Taiga"     <-    Add this if database name is TEST2504, replace with actual database name if needed
      },
      "Themes": {
        "Base": {
          "Caption": "Podstawowy",
          "DarkMode": false
        },
        "Dark": {
          "Caption": "Tryb ciemny",
          "DarkMode": true
        },
	      "Taiga": {     <-    Add this whole block for theme, e.g. Taiga
          "Caption": "Taiga",
          "DarkMode": true
        }
      },
      "LogoSettings": {
        "Default": {
          "CustomLogo": "",
          "CustomLogoLink": "",
          "CustomMobileMenuBg": ""
        }
      }
    },
```
File needs to be saved and services restarted.

Soneta.Products.Web.Standard is usually located on server wherever enova365 Multi is installed, alongside Soneta.Products.Server.Standard.

Result should look like this:

![image](https://github.com/user-attachments/assets/63f23f72-ade2-4241-97c7-9e89b8f216dc)

Key features added:

1. Contrast improved for default row coloring (e.g. Towary, Dokumenty)

2. Visuals set to something in between dark and light theme

More screenshots

![image](https://github.com/user-attachments/assets/879623c5-c314-4432-b0b7-05f93e8a7654)

![image](https://github.com/user-attachments/assets/18b16ebf-d949-4b7c-b606-077888ee6ea1)

Get enova365 [here](https://www.enova.pl/)

**Repository created for educational purposes only**

Example of a background

![me](https://github.com/Websome-pl/enova365TaigaTheme/blob/main/TaigaGif.gif)

**Background is not included in this instruction and used for educational purposes only**

**Background source: https://vsgif.com/gif/3555500**

Get instruction for making backgrounds in enova365 [here](https://www.enova.pl/)
