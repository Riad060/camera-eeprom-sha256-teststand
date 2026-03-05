# Test Plan

## Objective
Verify that the EEPROM contents of the camera match the expected SHA256 hash stored on the imager.

## Test Steps

1. Connect to the camera
2. Dump EEPROM contents
3. Compute SHA256 hash of EEPROM data
4. Read expected SHA256 hash from the imager
5. Compare calculated hash with expected hash

## Expected Results

Pass:
Calculated SHA256 matches the stored hash.

Fail:
Calculated SHA256 does not match the stored hash.

## Output

- Pass/Fail result
- EEPROM data dump
- Calculated SHA256
- Expected SHA256
