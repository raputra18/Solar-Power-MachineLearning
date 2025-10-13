==========================================
Solar Concentrator Dataset
==========================================

Rahmadi Putra A.
Department of Instrumentation and Control Engineering,
Universitas Gadjah Mada (UGM)
Indonesia

==========================================
Background
==========================================

This dataset was collected from an experimental vertical dual-axis solar concentrator system
using mirrors to reflect sunlight toward a vertically mounted photovoltaic panel. 
The system was equipped with LDR sensors, servo motors, and an ESP32 microcontroller 
for light tracking and data logging.

The data represents the real-time measurements of light intensity from multiple sensors,
motor angle adjustments, and energy output over time. It aims to support research in 
solar tracking optimization, IoT-based energy monitoring, and renewable energy control systems.

==========================================
Dataset Description
==========================================

The dataset contains recorded values aggregated over time intervals, with environmental
and control variables affecting system performance.


==========================================
Data Fields
==========================================

- datetime       : Date and time of data collection
- LDR1, LDR2, LDR3, LDR4 : Light intensity readings from four LDR sensors
- servo_angle    : Servo motor angle in degrees
- panel_voltage  : Output voltage from the solar panel
- panel_current  : Output current from the solar panel
- irradiance     : Estimated solar irradiance (W/m²)
- axis_position  : DC motor rotation value (for vertical axis)
- energy_output  : Computed power (Watt)

==========================================
Associated Tasks
==========================================

- Regression:
    Predicting solar power output or light intensity based on environmental conditions.

- Control Analysis:
    Evaluating servo response and control efficiency under varying light distribution.

- IoT Data Monitoring:
    Developing visualization or dashboards for real-time solar tracking performance.

==========================================
License
==========================================

This dataset is open for academic and research purposes.
Please cite the author if used in publications:

Rahmadi Putra A. (2025). Solar Concentrator Dataset. Universitas Gadjah Mada.

==========================================
Contact
==========================================

For more information, please contact:
Rahmadi Putra A.
Email: rahmadi.putra.aji@mail.ugm.ac.id
GitHub: https://github.com/raputra18
linkedin: https://www.linkedin.com/in/rahmadiputraaji2001
