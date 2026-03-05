# Project Overview

## Goal
Automate the verification of camera EEPROM integrity using TestStand.

## Current Manual Process
1. Connect the camera to the system
2. Open the VI used for camera communication
3. Dump the EEPROM data
4. Extract the hexadecimal data
5. Format the hex data for SHA256 input
6. Calculate the SHA256 hash
7. Compare the calculated hash with the hash stored on the camera imager

## Target Automated Solution
A TestStand module that will automatically:

- Connect to the camera
- Dump EEPROM contents
- Calculate the SHA256 hash of the EEPROM data
- Read the expected hash stored on the imager
- Compare the calculated hash with the stored hash
- Output a Pass/Fail result

## Tools Used
- NI TestStand
- NI LabVIEW
- SHA256 hashing
- Camera communication modules
