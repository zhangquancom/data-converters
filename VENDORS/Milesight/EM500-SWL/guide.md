# Submersible Water Level Sensor - Milesight IoT

The payload decoder function is applicable to EM500-SWL.

## Payload Definition

|     CHANNEL     |  ID  | TYPE | LENGTH | DESCRIPTION                               |
| :-------------: | :--: | :--: | :----: | ----------------------------------------- |
|     Battery     | 0x01 | 0x75 |   1    | battery(1B)<br/>battery, unit: %          |
|   Water Level   | 0x03 | 0x77 |   2    | water_level(2B)<br/>water_level, unit: cm |
| Historical Data | 0x20 | 0XCE |   6    | timestamp(4B) + water_level(2B)           |