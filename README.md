# Analog to Digital Signal Conversion
By [Naimur Rahman](https://github.com/nayeem-rafi)
## [Click for Files](https://drive.google.com/drive/folders/1aYsiQ6l6xobzYM8NmtJ5ZH6Zgu7BMiFH?usp=drive_link)

## Introduction:
This MATLAB code demonstrates the process of analog-to-digital conversion (ADC) through three key stages: **sampling**, **quantization**, and **digital encoding**. It visualizes how a continuous sine wave is sampled, quantized, and then converted into a digital binary representation. The goal is to demonstrate fundamental digital signal processing concepts that are critical in various real-world applications such as audio processing, telecommunications, and data transmission.

## Objective:
The primary objective of this code is to:
1. Sample a continuous sine wave at a rate defined by the Nyquist theorem.
2. Quantize the sampled data into discrete levels.
3. Encode the quantized values into a binary digital format.

## Analyzing the Input:
The input signal is a continuous sine wave described by:
- **Frequency (f)**: 20 Hz
- **Amplitude (A)**: 5
- **Phase**: 0

The sine wave is sampled over 3 cycles at a multiple of the Nyquist rate (8 times). The Nyquist rate is twice the signal frequency, ensuring that the signal can be reconstructed accurately from the samples.

## Sampling:
The sine wave is sampled at discrete time intervals using the following parameters:
- **Nyquist rate** (FN): \(2 \times f = 40 \, Hz\)
- **Sampling frequency** (Fs): \(8 \times FN = 320 \, Hz\)
- **Sampling period** (Ts): \(1 / Fs\)

The sampled values are extracted at time intervals defined by `ts`, and the corresponding continuous sine wave is plotted for comparison.
## How the Code Works:
1. **Input Sine Wave Generation:**
   The continuous sine wave is generated using the sine function, which is plotted to show the original analog signal.

2. **Sampling the Signal:**
   The signal is sampled at a rate determined by the Nyquist theorem. The sampled values are plotted as a stem plot, illustrating the discrete points where the continuous signal is captured.

3. **Quantization:**
   The sampled signal is then quantized. A 5-bit quantizer is used, providing 32 discrete levels, ranging between -5 and 5. Each sampled value is assigned to the nearest quantization level, simulating the loss of precision during quantization.

4. **Digital Encoding:**
   Each quantized value is converted into its binary representation using a 5-bit encoding. The binary sequence is then visualized as a digital signal (using a -1 for binary 0, and 1 for binary 1), representing the final output.

## Digital Output:
In the final step, the binary encoded signal is plotted as a digital waveform. This binary signal is what would be transmitted or stored in a digital system after conversion from its original analog form.

<h1 align= "center">

**Digital Conversion**
</h1>
<p align="center">
<img src="https://github.com/user-attachments/assets/f021a117-4940-4608-9608-3dce72e5cd2c", width="620">
</p>

## How to Run the Code:
1. Install MATLAB on your system.
2. Open the MATLAB editor and copy the provided code.
3. Run the script directly in the MATLAB environment.
4. The code will generate three plots:
   - A continuous sine wave (input signal).
   - A sampled sine wave.
   - The quantized and digitally encoded signal.

## Conclusion:
This MATLAB script effectively demonstrates the key stages in analog-to-digital conversion (ADC). The continuous analog sine wave is sampled, quantized, and encoded into a digital format. The visual representation aids in understanding how the signal changes at each stage, providing insights into the fundamentals of digital signal processing.

This simple approach forms the backbone of more complex digital signal processing systems used in real-world applications like audio processing, image processing, and data communication.

---

You can replace the values for frequency, amplitude, and number of bits in the quantizer to explore how they impact the digital output!
