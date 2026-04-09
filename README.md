# PHASE-MODULATION
EXPT NO: 5 PHASE MODULATION
---


Aim:

To implement and analyze phase modulation (PM) using scilab.

---

Apparatus Required:


Software: SCILAB
Hardware: Personal Computer

---

Theory:


Phase Modulation (PM) is a technique where the phase of the carrier wave is varied in proportion to the instantaneous amplitude of the input signal (message signal). Unlike frequency modulation, where the frequency is varied, in phase modulation, the phase angle of the carrier wave changes with the amplitude of the message signal.

The general form of a PM signal can be represented as:

epm=ac * cos ( (2 * 3.14 * fc * t) + (4.9 * cos (2 * 3.14 * fm * t) ) );

---

Algorithm:


Initialize Parameters: o Set values for carrier amplitude (Ac, carrier frequency (fc, message frequency (fm), sampling frequency(fs), and phase deviation sensitivity (kp).
Generate Time Axis: o Create a time vector for the signal duration based on the sampling frequency.
Generate Message Signal: o Define the message signal as a cosine wave.
Generate PM Signal: o Apply the PM modulation formula to obtain the modulated signal.
Plot the Signals: o Use plot to plot the message signal, carrier signal, and phase-modulated signal.

---

Program:

```
am=7.8

fm=278;

ac=15.6;

fc=2780;

fs=27800;

t=0:1/fs:2/fm;

em=am * cos (2 * 3.14 * fm * t);

subplot(3,1,1);

plot(t,em);

ec=ac * cos (2 * 3.14 * fc * t);

subplot(3,1,2);

plot(t,ec);

epm=ac * cos ( (2 * 3.14 * fc * t) + (4.9 * cos (2 * 3.14 * fm * t) ) );

subplot(3,1,3);

plot(t,epm);
```

---
Calculation:

---

Output :

![WhatsApp Image 2026-04-09 at 16 34 27](https://github.com/user-attachments/assets/56fde1be-8afb-4ead-9585-8ef5bbedff14)


---

Result :

The message signal, carrier signal, and phase-modulated (PM) signal will be displayed in separate plots. The modulated signal will show phase variations corresponding to the amplitude of the message signal.
