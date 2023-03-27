
```json
{
    "package": {
        "productName": "vitauri",
        "version": "1.5.2"
    },
    "build": {
        "distDir": "../dist",
        "devPath": "http://localhost:8080",
        "beforeDevCommand": "",
        "beforeBuildCommand": ""
    },
    "tauri": {
        "systemTray": {
            "iconPath": "./icons/icon.png",
            "iconAsTemplate": true
        },
        "bundle": {
            "active": true,
            "targets": "all",
            "identifier": "com.spada.vitauri",
            "icon": [
                "icons/32x32.png",
                "icons/128x128.png",
                "icons/128x128@2x.png",
                "icons/icon.icns",
                "icons/icon.ico"
            ],
            "resources": [],
            "externalBin": [],
            "copyright": "",
            "category": "DeveloperTool",
            "shortDescription": "",
            "longDescription": "",
            "deb": {},
            "macOS": {},
            "windows": {
                "certificateThumbprint": null,
                "digestAlgorithm": "sha256",
                "timestampUrl": ""
            }
        },
        "updater": {
            "active": false
        },
        "allowlist": {
            "shell": {
                "all": true,
                "scope": [
                    {
                        "name": "cmd",
                        "cmd": "cmd",
                        "args": ["/C", { "validator": "\\S+" }]
                    },
                    {
                        "name": "pwsh",
                        "cmd": "powershell", // The command name. It can start with a variable that resolves to a system base directory. The variables are: $AUDIO, $CACHE, $CONFIG, $DATA, $LOCALDATA, $DESKTOP, $DOCUMENT, $DOWNLOAD, $EXE, $FONT, $HOME, $PICTURE, $PUBLIC, $RUNTIME, $TEMPLATE, $VIDEO, $RESOURCE, $APP, $LOG, $TEMP, $APPCONFIG, $APPDATA, $APPLOCALDATA, $APPCACHE, $APPLOG.
                        "args": ["-Command", { "validator": "\\S+" }]
                    }
                ]
            },
            "notification": {
                "all": true
            }
        },
        "windows": [
            {
                "title": "ViTauri",
                "width": 1920,
                "height": 1080,
                "resizable": true,
                "fullscreen": false
            }
        ],
        "security": {
            "csp": null
        }
    }
}
```
