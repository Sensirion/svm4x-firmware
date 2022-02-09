# SVM41 Firmware Changelog

## v3.2 (2021-11-10)
- This firmware is based on the SVM40 firmware but with replaced sensor 
  (SGP41 instead of SGP40) and a new algorithm version including NOx 
  calculation
- Implement gas index algorithm to released version "3.1.0"
- SHDLC:
  - Bump to version 0.8.4
  - Implement new version of "voc algorithm tuning paramter" command (0x600D),
    includes the additional argument "gain factor" of the new algorithm release.
  - Replace the "time hours"-argument in the "voc algorithm tuning parameter"
	command (0x600D( by two arguments. One for the time gain hours, and another
	one for the time offset hours.
  - Implement "nox algorithm tuning paramter" command (0x600E)
  - Remove support of float values in "get temperature offset for rht
    measurments" command
- I2C:
  - Bump to version 0.7.4
  - Implement new version of "voc algorithm tuning paramter" command (0x60D0),
    includes the additional argument "gain factor" of the new algorithm release.
  - Replace the "time hours"-argument in the "voc algorithm tuning parameter"
	command (0x60E1) by two arguments. One for the time gain hours, and another
	one for the time offset hours.
  - Implement "nox algorithm tuning paramter" command (0x60E1)

