📖 Overview

An advanced Indoor Real-Time Location System (RTLS) utilizing UHF RFID technology. Unlike traditional RSSI-based methods which are prone to noise, this project exploits the Phase Difference of Arrival (PDoA) of the backscattered signal to estimate tag positions with centimeter-level precision.

🧠 The Algorithm
The core of the project is a Python-based processing engine that interprets raw phase data from a UHF RFID reader.
1.	Data Acquisition: The reader interrogates passive tags from multiple antenna positions, capturing the phase angle ($\phi$) of the reflected signal.

2.	Signal Processing:


o	Phase Unwrapping: Resolving the $2\pi$ ambiguity in phase measurements across different frequencies.

o	Noise Filtering: Mitigating multipath interference using statistical averaging and filtering.


3.	Localization:
o	Applies trilateration and non-linear optimization algorithms to solve for the tag's $(x, y)$ coordinates based on phase distance constraints.
🎯 Results

•	Accuracy: Achieved a target localization error of ±30 cm in controlled test environments.

•	Scale: Capable of processing datasets with 500+ phase readings efficiently.


🛠️ Tech Stack

•	Language: Python (NumPy, SciPy, Pandas).

•	Hardware: UHF RFID Reader, Multi-static Antenna Array, Passive Tags.


•	Concepts: Signal Propagation, Multipath Mitigation, Convex Optimization.

________________________________________
Author: Uzair Ashfaq

