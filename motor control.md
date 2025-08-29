# DC Motor with Gear Box JGA25-370-12V-210RPM 12Kg.cm

![1756444914825](image/motorcontrol/1756444914825.png)
![1756444924834](image/motorcontrol/1756444924834.png)

[Product Link](https://makerselectronics.com/product/dc-motor-with-gear-box-jga25-370-12v-210rpm-12kg-cm/?srsltid=AfmBOopo4nG8ZZGngsGIekyhnOatHNANZfpcCv5DG7JuyXZaMDWsJSfs)

**Specifications:**

- Operating voltage: between 6 V and 18 V
- Nominal voltage: 12 V
- Free-run speed at 12 V: 210 RPM
- Free-run current at 12 V: 50 mA
- Stall current at 12V: 1200 mA
- Stall torque at 12V: 12 kg.cm
- Reductor size: 20.5 mm

---

## Motor with Encoder (Specs)

[Product Link](https://makerselectronics.com/product/dc-motor-ga25-370-with-encoder-2kg-280rpm-12v-with-bracket/?campaignid=20503411856&adgroid=up&network=x&device=c&campaignname=sales_pmax&gad_source=1&gad_campaignid=20503433012&gbraid=0AAAAApRJSNE4wSCHg3GhG2qAX8W8JFz_4&gclid=Cj0KCQjw_L_FBhDmARIsAItqgt49KK8sweIGdAin_c3GotssxFyOU7bmKSqn5d4HHsuBkCs0aBybfnEaAgQDEALw_wcB)

---

## Hall Effect Two Channel Magnetic Rotary AB Encoder for DC motors

![1756444970527](image/motorcontrol/1756444970527.png)

[Product Link](https://uge-one.com/product/hall-effect-two-channel-magnetic-rotary-ab-encoder-for-dc-motors/?srsltid=AfmBOoqJ4M-L5KCFwuAimLcF1_Iutna2yb9JH8yx7tWUMciwEZAPg4Ab)

**Quadrature mode:**

- **X1 decoding**
  - pulse per A or B channel rising
- **X2 decoding**
  - 1 pulse per A or B channel rising & another for falling
- **X4 decoding**
  - 2 pulses for rising 1 of them for each channel & 2 pulses for falling
  - More accurate but require more magnets 1 every 90 deg of the encoder disk

![1756445046656](image/motorcontrol/1756445046656.png)

---

## Algorithm idea (X1 mode)

- Enable interrupt only on **rising edge of channel A**.
  - Each time channel A rises:
    - Read the state of channel B.
    - If B = HIGH → rotation is CW.
    - If B = LOW → rotation is CCW.

---

## Algorithm idea using Hardware (x1 mode)

- Configure hardware timer/counter in quadrature mode with **X1 resolution**.
- The hardware increments/decrements counter once per full A cycle (only on one edge).
- You can Read the counter register whenever position is needed.

![1756445134020](image/motorcontrol/1756445134020.png)

---

## BTS7960 H-Bridge High-Power DC Motor Driver

![1756445180739](image/motorcontrol/1756445180739.png)

[Product Link](https://makerselectronics.com/product/bts7960-h-bridge-dc-motor-driver-43a/?srsltid=AfmBOopHyXbIaTu3WWemrBgyPAI9ZnkS268g9QA4mBAzp8UFHzclzPqo)

[Data Sheet &amp; Arduino Tutorial](https://makerselectronics.com/wp-content/uploads/2016/11/BTS7960-Motor-Driver.pdf)

**Specifications:**

- Input Voltage: 6 ~ 27Vdc.
- Driver: Dual BTS7960 H Bridge Configuration.
- Peak current: 43-Amp.
- PWM capability of up to 25 kHz.
- Control Input Level: 3.3~5V.
- Control Mode: PWM or level
- Working Duty Cycle: 0 ~100%.
- Over-voltage Lock Out.
- Under-voltage Shut Down.

![1756445221197](image/motorcontrol/1756445221197.png)
![1756445231117](image/motorcontrol/1756445231117.png)
