#2.4GHz Digital Voice Transceiver

A robust digital walkie-talkie system utilizing Arduino microcontrollers and the nRF24L01+ transceiver module. This project leverages GFSK modulation and packet-based voice transmission to ensure reliable audio communication, featuring comprehensive MATLAB simulations for BT-product optimization and spectral efficiency analysis.

#Hardware Components
(Note: The list below details the components required to build 1 transceiver node. You will need to double this list to build the complete two-way walkie-talkie system.)

| Component | Quantity | Description |
| Arduino Nano / Uno | 1 | Core microcontroller for audio ADC sampling and SPI management. |
| nRF24L01+ Module | 1 | 2.4GHz RF Transceiver. |
| Electret Microphone Amp | 1 | Captures voice and amplifies it for the Arduino ADC (e.g., MAX4466). |
| PAM8403 Amplifier | 1 | Class-D audio amplifier to drive the speaker. |
| 8Ω Speaker | 1 | Audio output (0.5W to 3W). |
| Push Button | 1 | Triggers the Push-to-Talk (PTT) mechanism. |
| 10µF - 100µF Capacitor | 1 | Bypass capacitor across nRF24L01+ power pins (**CRITICAL** for module stability). |
| Resistors & Capacitors | Set | Used to build the custom RC Low-Pass Filter. |

#Repository Structure
├── README.md
├── Documentation/
│   ├── architecture_diagram.jpeg
│   ├── block_diagram.jpeg
│   ├── ckt_diagram.jpeg
│   └── flowchart.jpeg
├── Hardware/
├── Arduino_Walkie_Talkie_nRF24L01/
    │   ├── Arduino_Walkie_Talkie_nRF24L01.ino
│   ├── RF24Audio-1.0.zip
│   ├── prototype_img_1.jpeg
│   └── prototype_img_2.jpeg
└── Matlab_Simulations/
    ├── FSK_vs_GFSK/
    │   ├── BER_Graph.png
    │   ├── FSK_vs_GFSK_Code.m
    │   └── PSD_Graph.png
    └── GFSK_Simulation/
        ├── BER.png
        ├── GFSK_Sim_Code.m
        └── PSD.png
