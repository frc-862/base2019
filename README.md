# base2019
Base code for - Destination Deep Space

# Goals

* Clean design
  * Subsystem provide only access to hardware
  * Constants that are not robot specific, and non-global in nature moved into module where actually used
  * Unit tests (please WPILib folk make this easier)
  * Provide an DriveTeam subsystem for named access to controls, rather than rawAxis/button calls
  
* Fix CAN timeout warnings 

* Logging
  * Build on existing logging framework
  * Provide better file naming when possible
    * Prefer FMS names
    * Use date/time based names
    * Unique numbering
  * Have multiple logging timing loops to support systems with slower access (CAN)
  * Provide an http server in disabled mode that serves raw log files, and a javascript graphing system
  
* Motion Profiling
  * Incorporate best of our code from last
  * Update (or find another) visualizer
  * Work with calibration tools to improve path following
  
* Turn to 
  * Fix issue with motion magic updates on rotate
  * Check gains used by motion magic
  
* Vision
  * Train freshman/sophomores on jevois
  * Train freshman/sophomores on opencv
  * Accurate timestamps between systems
  * Integrate with state space model
  
* Adaptive pursuit
  * Figure this out :-)
  
* Motion Profile record / playback

* I2C for time of flight distance sensors

* CANifier testing

