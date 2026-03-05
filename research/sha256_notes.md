# SHA256 Notes

SHA256 is a cryptographic hash function that produces a 256-bit (32 byte) hash value.

Purpose in this project:
Ensure EEPROM data integrity.

Key Points

- The hash must be calculated on the exact byte sequence of EEPROM data.
- Formatting errors in hexadecimal data can produce incorrect hashes.
- The calculated hash must match the hash stored on the camera imager.

Future Work

- Confirm EEPROM memory range used in the hash
- Verify byte formatting before hashing
