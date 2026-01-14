# LC Voltage Controlled Oscillator (LC-VCO)

**Design and simulation of an LC Voltage Controlled Oscillator (LC-VCO)** implemented in **Cadence Virtuoso (gpdk045 technology)**.  
The oscillator is based on a **cross-coupled NMOS differential pair** with an **LC tank** providing frequency selectivity and a **tail current source** ensuring bias stability.

## 🧠 <ins>Operating Principle</ins>
- Thermal noise and initial imbalance trigger oscillations.
- The cross-coupled NMOS pair introduces **negative resistance**.
- When |R<sub>neg</sub>| > R<sub>p</sub>, oscillations grow.
- The amplitude stabilizes due to device non-linearities.
- Oscillation frequency is primarily determined by:

$$\[
f_0 = \frac{1}{2\pi\sqrt{LC}}
\]$$


## 📊 <ins>Results and Observations</ins>

### 1️⃣ Transient Start-Up
- Oscillations initiate from noise.
- Exponential growth observed during start-up.
- Stable sinusoidal waveform achieved after settling.

### 2️⃣ Differential Node Voltages (Vx & Vy)
- 180° phase difference between Vx and Vy.
- Centered around the bias voltage.
- Symmetric amplitude confirms balanced design.

### 3️⃣ Tank Currents (Ix & Iy)
- Sinusoidal current waveforms.
- Phase shift consistent with LC tank behavior.
- Equal magnitude currents validate differential operation.

### 4️⃣ Voltage–Current Relationship
- Proper phase alignment between tank voltage and current.
- Confirms energy exchange between L and C.

### 5️⃣ Frequency Spectrum Analysis
- Dominant single frequency peak at oscillation frequency.
- Low noise floor relative to carrier.
- Harmonics visible due to MOS non-linearities.

