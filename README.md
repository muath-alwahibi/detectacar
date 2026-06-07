🚗 DetectaCar — Vehicle Detection & Counting Device

Diploma Final Project — University of Technology and Applied Sciences (UTAS)

A low-cost, portable roadside device that counts vehicles passing through a specific location using ultrasonic sensing. Results are transmitted wirelessly to a mobile phone via Bluetooth — providing actionable traffic data for businesses, urban planners, and government agencies.

🔧 Hardware Used
ComponentPurposeArduinoMain microcontrollerUltrasonic SensorDetects vehicle presence within calibrated rangeBluetooth ModuleTransmits count data to mobile deviceLCD DisplayLocal real-time count displayLED IndicatorsVisual feedback on detection eventsBatteryPortable, self-powered operation

⚙️ How It Works

The ultrasonic sensor continuously monitors a set distance and height threshold
When a vehicle passes, it breaks the sensor's range — triggering a count increment
Sensor range is carefully calibrated to detect only vehicles, filtering out pedestrians and small objects
The running count is displayed on the LCD and simultaneously broadcast via Bluetooth
A paired mobile phone receives and logs the data in real time


🎯 Key Features

Vehicle-specific detection — custom distance and height calibration filters out non-vehicle objects
Wireless data output — Bluetooth connectivity to mobile device for easy data access
Portable & battery-powered — no fixed infrastructure required, deployable anywhere
Real-time LCD display — instant local readout without needing a phone
Cost-effective — built entirely from off-the-shelf components


🧩 System Architecture
[Ultrasonic Sensor] ──► [Arduino] ──► [LCD Display]
                              │
                        [Bluetooth] ──► [Mobile Phone]

🎯 Use Cases

Business site selection — measure foot and vehicle traffic before opening a business
Traffic congestion analysis — identify peak hours on specific roads
Government & urban planning — low-cost alternative to expensive traffic counters
Law enforcement — monitor traffic volume in specific zones


🔍 Design Decisions
Initially tested with a pothole/pressure sensor — abandoned because it picked up all movement regardless of object type. Switched to ultrasonic sensing, which allowed precise range and height calibration to isolate vehicle-sized objects only.
