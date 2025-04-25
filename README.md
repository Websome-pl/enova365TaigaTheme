Guide to install theme Taiga for enova365 version 2504.1.1

First these files need to be downloaded and put in this enova365 directory: Soneta.Products.Web.Standard\wwwroot-Standard\css\palettes

Secondly in this directory: C:\Program Files (x86)\Soneta\Soneta.Standard 2504.1.1\Soneta.Products.Web.Standard (or any other directory in which enova365Multi is installed) file appsettings.json needs to be modified:

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

Result should look like this:

![image](https://github.com/user-attachments/assets/63f23f72-ade2-4241-97c7-9e89b8f216dc)

Key features added:

1. Contrast improved for default row coloring (e.g. Towary, Dokumenty)

2. Visuals set to something in between dark and light theme


