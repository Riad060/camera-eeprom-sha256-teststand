# System Architecture

The automated verification system will be built using TestStand and LabVIEW.

## Components

Camera Module
- The hardware device containing the EEPROM and imager.

TestStand
- Controls the overall test sequence.
- Executes steps for communication, hashing, and comparison.

LabVIEW Modules
- Used for hardware communication and EEPROM data extraction.

SHA256 Calculation
- Computes the cryptographic hash of the EEPROM data.

Comparison Logic
- Compares calculated SHA256 with the expected hash stored on the imager.

## Data Flow

Camera → EEPROM Dump → SHA256 Calculation → Hash Comparison → Pass/Fail Result
