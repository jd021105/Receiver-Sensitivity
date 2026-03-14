# Receiver-Sensitivity
# Optical Receiver Sensitivity Analysis

## Objective
Determine the sensitivity of a PIN photodiode-based optical receiver by calculating the minimum received power necessary to achieve a given Q factor. Compare simulation results with those obtained analytically.

---

## Theory
If only thermal noise is considered, the sensitivity of a PIN photodiode-based receiver is:



<img width="1126" height="718" alt="image" src="https://github.com/user-attachments/assets/22298a91-302d-41e4-b254-86c9b8ec704e" />

---

## Calculations
Receiver specifications:

| Parameter                        | Value                          |
|----------------------------------|--------------------------------|
| Operating bit rate               | 2.5 Gb/s                       |
| Bandwidth                        | 1.65 × bit rate                |
| Thermal noise spectral density    | X.Y × 10⁻²² A²/Hz              |
| Desired Q factor                 | 6                              |
| PIN photodiode responsivity      | 1 A/W                          |

> **Note:** X and Y are the last two digits of your student ID.  
> Example: If ID ends with **43**, then ST = 4.3 × 10⁻²² A²/Hz.  

Using the formulas above, calculate the receiver sensitivity.

---

## Layout
The simulation layout consists of:
1. CW laser source  
2. NRZ modulator  
3. Optical attenuator  
4. PIN photodiode with electrical filter  

Settings:
- Responsivity = 1 A/W (default)  
- Dark current = 0  
- ASE noise = off  
- Thermal noise parameter = editable  

Power meters are placed:
- At the modulator output  
- After the attenuator (input to receiver)  

---

## Simulation
Steps:
1. Adjust output power to **0 dBm**.  
2. Set attenuator to **20 dB**.  
3. Run the simulation.  
4. Adjust attenuator until **Q factor = 6.00 ± 0.05**.  

---

## Report
Your report should include:
- Pre-lab calculations (attach handwritten work if applicable).  
- Screenshots or displays of simulation results:  
  - Power readings  
  - BER analyzer output  
  - Eye diagram  
- Discussion of differences between analytical and simulation results.  
<img width="769" height="1280" alt="image" src="https://github.com/user-attachments/assets/05545419-1b10-4da3-8290-da59a7e64838" />
<img width="799" height="1280" alt="image" src="https://github.com/user-attachments/assets/cca53c3a-6628-4fcd-a02f-1bad9e547a08" />
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/4e197502-1199-48e4-ad4c-7a847f6c4d64" />

![alt text](<Screenshot 2025-09-24 213808.png>)

---

 ## result 
 Thus the receiver sensitivity is obtained and calculated.
