# Home Assistant Nexia UX360 Integration

This is a copy of the official Home Assistant integration for Nexia with an updated version of the python library which supports the Trane ux360 thermostat. The core of the Nexia integration is the same.  This is currently in use for my own Home Assistant installation and has been working so far.   

The Home Assistant Nexia Integration code comes from the official source: 
https://github.com/home-assistant/core/tree/dev/homeassistant/components/nexia

The Python Library that is replaced comes from:
https://github.com/bdraco/nexia 
There is a pending pull request (as of 2024/10/05) to bring these updates into the official Python library which should eventually enable the builtin Nexia inegration to just work with the UX360. 



# Installation

## Overview
This integration has to be installed manually since its not a part of any official sources

- Clone git repository
- Copy into homeassistant/custom_components
- Restart Home Assistant
- In Home Assistant, add inegration "Nexia/American Standard/Trane UX360"
- Enter in Trane account details and select Trane

## Git cloning
The fastest way to get this onto Home Assistant is to install a ssh addon that allows connecting directly to call the git clone command in the correct directory.  For example "Advanced SSH & Web Terminal".  The process would appear like this:

- Open the SSH GUI:  Settings->Addons->Advanced SSH & Web Terminal->Open Web UI
- Navigate to the custom_components directory:
```
   cd homeassistant/custom_components/
```
- Use the git clone command to pull down the latest version
```
git clone https://github.com/davidhewing/nexia_ux360.git
```

## Steps after git structure installation

- Navigate to Settings -> Top Left Menu -> Dropdown: Restart Home Assistant.
- Navigate to Settings -> Devices & Services
- Select "Add Integration" at the bottom right corner
- Search for "nexia" and select "Nexia/American Standard/Trane UX360"
- Enter in Trane Account Details and select Trane


