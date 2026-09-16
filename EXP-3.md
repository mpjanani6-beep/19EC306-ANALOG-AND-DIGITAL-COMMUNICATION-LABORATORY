# Aim:
To obtain Pulse Amplitude Modulation & Demodulation using trainer kit.

# THEORY
In Pulse Amplitude Modulation, the signal is sampled at regular intervals and the amplitude of each sample is made proportional to the amplitude of the signal at that instant of sampling. This amplitude of each sample is hold for the sample duration to make pulses flat top.
The Pulse Amplitude Demodulator consists of Active Low Pass Butterworth Filler. It filters out the sampling frequency and their harmonics from the modulated signal and recovers the base band by integratedaction

# EQUIPMENTS
Experimental kit DCL -08 Connecting chords
Power supply
20 MHz Dual trace oscilloscope
NOTE: Keep The Switch Faults In Off Position.

# PROCEDURE
Refer to the block diagram (Fig. 1) and carry out the following connections and switch settings.
ConnectthePower Supply withproperpolaritytothekit DCL-08 andswitch it on. Select 16KHZ sampling frequency by jumper JP1.
Connect the1KHz,2Vp-psinewavesignalgenerated onboardtoPAM in post.
Shortthe followingposts with the Connecting chords provided as shown in diagram. PAM OUT and AMP IN
AMP OUT and FIL IN.
Keep the amplifier gain control potentiometer PS to maximum completely clockwise. Observe the Pulse Amplitude Demodulated signal at FIL OUT, which is same as the input signal. Repeat the experiment for different input signal and sampling frequencies.
 
# SWITCH FAULTS;
Note: Keep the connections as per the procedure.
Now switch corresponding fault switch button in ON condition & observe the different effect onthe output. The faults are normally used one at a time. Put Switch 1 of SF1 in Switch Fault section to ON position. The feedback resistor isbypassed from Amplifiersection. Gainof Amplifiernowdepends on potentiometer P5 only Put switch 2 of SF1 in Switch Fault section to ON position. This will generate twomixedsinewaves, whichcouldbeused as a modulatinginput signal for modulators PAM, PWM and PPM. Put switch 3 of SF1 in Switch Fault section to ON position. This willbypass one filter from filter section. The output consists of ripple with reference to previous output without switch fault. Put switch 4 of SF1 in Switch Fault section to ON position. This provides constant high sampling signal to the sampling switch, which in turn gives natural sampling at the output. Put switch 5 of SF2 in Switch Fault section to ON position. This removes the control signal of first switch of PAM section, this will open pin of CMOS IC. Due to this output will be abrupt or may follow the input.

# BLOCK DIAGRAM:
<img width="846" height="597" alt="image" src="https://github.com/user-attachments/assets/8bb62333-4780-422a-98cf-5691a39012f6" />


# Tabulation:
<img width="1600" height="999" alt="WhatsApp Image 2026-09-15 at 6 33 59 PM (1)" src="https://github.com/user-attachments/assets/d83e5807-fedb-4c34-b323-ad4ef64e084c" />

# MODEL GRAPH:
<img width="581" height="742" alt="image" src="https://github.com/user-attachments/assets/86726ea8-2457-468d-aae0-57ced7f9d25a" />


# OUTPUT GRAPH:
<img width="1179" height="1600" alt="WhatsApp Image 2026-09-15 at 6 33 59 PM" src="https://github.com/user-attachments/assets/59675c80-29bc-4c58-bc48-9ece6a2ac6de" />

# Result:
Thus the pulse amplitude modulated and demodulated signals is generated and output is verified.
