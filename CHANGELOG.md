# Changelog for `wpg-weatherchan`

## 2.0.9 [2024-02-11]
- Fixed bug that has old blue colour upon launch (line 817), also changed blue to 0x00006D as noted in 2.0.8 but missed
- Updated RSS section -- old code assumed at least 8 entries. new code is flexible up to max pixel size, also fixed it so it actually refreshes
- Changed RSS scroll time to 2ms (was 5ms) to match original videon/shaw feed

## 2.0.8 [2024-01-20]
BUGFIX:
- Added try functions to weather update (line 610 & 619) to prevent crashing once running - program will still crash if weather update fails on initial launch
- Updated RSS feed URL to use CTV News (Thanks Tekhnocyte!)
- Added code in screen 4 to avoid colour not changing if page is skipped
- moved print/debug messages to new function debug_msg. Can enable/disable, select verbosity, add datestamp
IMPROVEMENT/MISC:
- Updated channel listings on page 11 / removed pages 12 and 13
- Increased vertical size of center page / moved text locations
- Changed red colour from 0xBC0000 to 0x6D0000, changed blue colour from 0x0000A5 to 0x00006D (better visibility on b&w TVs)
- Increased time between page changes to 20sec (was 10sec)

## 2.0.7 [2023-09-11]
- Updated CityofWinnipeg RSS feed URL (old URL 404)

## 2.0.6 [2023-09-02]
- Updated channel listings

## 2.0.5 - Skipped

## 2.0.4 [2023-06-06]
- Line 89 humidex typo
- Line 203 fixed high/low yesterday temp - added check for nonetype   

## 2.0.3
- Updated channel listings

## 2.0.1
- Changed forecast time to use current time when updating weather - the date and time from forecast_time in env_canada returns odd results
- Changed UV INDEX to show -- instead of blank if no index is preset
