# Camera EEPROM SHA256 TestStand

## Overview
This project aims to automate the verification of camera EEPROM integrity using NI TestStand and LabVIEW.

The automated test will connect to a camera, dump the EEPROM contents, compute a SHA256 hash of the EEPROM data, and compare it to the SHA256 hash stored on the camera imager.

The goal is to eliminate the current manual verification process and provide a reliable automated Pass/Fail result.

---

## Current Manual Process
The current workflow used by engineers involves several manual steps:

1. Connect the camera to the system
2. Open the VI used for camera communication
3. Dump the EEPROM data
4. Extract and format the hexadecimal data
5. Calculate the SHA256 hash using a hash calculator
6. Compare the calculated hash with the hash stored on the camera imager

---

## Automated Solution
The automated TestStand module will perform the following steps:

1. Connect to the camera
2. Dump EEPROM contents
3. Compute SHA256 hash of the EEPROM data
4. Read the expected SHA256 hash stored on the imager
5. Compare both hashes
6. Output a Pass/Fail result

---

## Tools Used
- NI TestStand
- NI LabVIEW
- SHA256 hashing
- Camera communication modules

---

## Repository Structure

docs/
Project documentation such as system architecture, test plan, and project overview.

docs/logs/
Development progress log.

research/
Technical notes and investigation related to SHA256 and EEPROM data.

teststand_sequences/
TestStand sequence files used to automate the test.

labview_modules/
LabVIEW VIs used for camera communication and EEPROM data extraction.

screenshots/
Screenshots of the TestStand and LabVIEW implementation.

data_examples/
Example EEPROM dumps and hash comparison data.

---

## Status
Project in development as part of an engineering internship.
