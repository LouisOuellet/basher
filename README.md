# Basher
Basher is a library of functions to help write bash script. It's intent is to provide functions and variables.

## How to use
This is how you can add basher to your bash project.

First you need to add basher as a submodule:
```bash
mkdir vendor && cd vendor
git submodule add https://github.com/LouisOuellet/basher basher
```

Then you can simply source basher at the beginning of your script.
```bash
source ${scriptDirectory}/vendor/basher/basher
```

## Supported OS
 * macOS
 * Ubuntu
 * Debian
 * Rasbian
 * Arch
## Variables
### Formatting
#### COLORS
 * formatBlack
 * formatRed
 * formatGreen
 * formatYellow
 * formatBlue
 * formatMagenta
 * formatCyan
 * formatWhite
 * formatGrey
 * formatLightRed
 * formatLightGreen
 * formatLightYellow
 * formatLightBlue
 * formatLightMagenta
 * formatLightCyan
 * formatLightGrey
 * formatReset
#### STYLES
 * formatBold
 * formatBlinking
 * formatDim
### Elements
#### BOXES
 * elementBoxGood
 * elementBoxBad
 * elementBoxQuestion
 * elementBoxInfo
 * elementBoxOutput
#### FRAMES
 * elementFrameTopLeft
 * elementFrameTopRight
 * elementFrameBottomLeft
 * elementFrameBottomRight
 * elementFrameHline
 * elementFrameHlineStart
 * elementFrameHlineEnd
 * elementFrameVline
 * elementFrameVlineStart
 * elementFrameVlineEnd
### System
 * OS
 * Distribution
 * Architecture
 * PackageManager
 * IP
### Settings
 * smtpHost
 * smtpPort
 * smtpSecurity
 * smtpUsername
 * smtpPassword
 * smtpName
 * smtpFrom
### Basher
 * verboseMode
 * debugMode
 * debugSend
 * logDirectory
 * logFile
 * scriptDirectory
 * scriptName
 * helpUsage
 * helpOptions
 * helpFunctions
## Functions
 * help : Display help
 * error : Interrupt script and execute help
 * dbg : When string is piped into this function, it adds some debugging data.
 * exec : Execute command through the debugger
 * pkg : Install a package
 * send : Send an email
