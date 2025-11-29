# EC1421-19EC421-Analysis-and-Design-of-Analog-ICs
# DESIGN OF ACTIVE LOW PASS,HIGH PASS AND BAND PASS FILTERS USING OP-AMP 

## AIM: 

To design and obtain the frequency response of 
i) First order Low Pass Filter (LPF) 
ii) First order High Pass Filter (HPF) 
iii) Band pass filter
 
## APPARATUS REQUIRED

<img width="625" height="170" alt="image" src="https://github.com/user-attachments/assets/900fc8b3-3a8c-4208-bf52-98cc9e281e21" />

## THEORY
## LOW PASS FILTER 
 A LPF allows frequencies from 0 to higher cut of frequency, fH.  At fH the gain is 0.707 
Amax, and after fH gain decreases at a constant rate with an increase in frequency.  The gain 
decreases 20dB each time the frequency is increased by 10.  Hence the rate at which the gain 
rolls off after fH is 20dB/decade or 6 dB/ octave, where octave signifies a two fold increase in 
frequency.  The frequency f=fH is called the cut off frequency because the gain of the filter at this 
frequency is down by 3 dB from 0 Hz.  Other equivalent terms for cut-off frequency are -3dB 
frequency, break frequency, or corner frequency.
# HIGH PASS FILTER 
The frequency at which the magnitude of the gain is 0.707 times the maximum value of 
gain is called low cut off frequency.  Obviously, all frequencies higher than fL are pass band 
frequencies with the highest frequency determined by the closed –loop band width all of the op
amp. 
# BAND PASS FILTER 
A band pass filter has a pass band between two cutoff frequencies fH and fL such that fH > 
fL.  Any input frequency outside this pass band is attenuated.  There are two types of band-pass 
filters.  Wide band pass and Narrow band pass filters.  We can define a filter as wide band pass if 
its quality factor Q <10.  If Q>10, then we call the filter a narrow band pass filter.  A wide band 
pass filter can be formed by simply cascading high-pass and low-pass sections.  The order of 
band pass filter depends on the order of high pass and low pass sections.

## CIRCUIT DIAGRAM: 
## LOW_PASS

<img width="1280" height="792" alt="image" src="https://github.com/user-attachments/assets/b213e2d3-9c15-4d37-b721-ff974689680e" />

## HIGH-PASS
<img width="1250" height="838" alt="image" src="https://github.com/user-attachments/assets/a0f57359-66a7-4cf3-99bf-c703c6ab5a4b" />

## BAND-PASS
<img width="1155" height="688" alt="image" src="https://github.com/user-attachments/assets/6eb4093b-496d-4994-bdc8-d21adc2e2ccc" />

## MODEL GRAPH:
## LOW_PASS

<img width="1142" height="836" alt="image" src="https://github.com/user-attachments/assets/65bb4252-039a-4036-a8aa-f7957019512a" />

## HIGH-PASS

<img width="1158" height="860" alt="image" src="https://github.com/user-attachments/assets/5fa2f0e9-1a1f-41d5-91c2-d8d69e78fb67" />

## BAND-PASS

<img width="1060" height="866" alt="image" src="https://github.com/user-attachments/assets/56e63d31-340b-4f89-b7e0-c4a688053a63" />

## PROCEDURE - (LPF & HPF): 
1. Connect the circuit as shown in the circuit diagram. 
2. Select the corresponding cut-off frequency (higher or lower) and determine the value of C&R. 
select the value of R1 & Rf depending on desired passband gain Af.. 
3. Apply a constant voltage input sinusoidal signal to the non-inverting terminal of op-amp. 
4. Tabulate the output voltage Vo with respect to different values of input frequency. 
5. Calculate passband gain and plot the graph of frequency versus voltage gain & check the 
graph to  get approximately the same characteristic as shown in the model graph. 
# PROCEDURE:BAND PASS FILTER 
1. Select the lower and higher cut-off frequency and calculate the value of R & C for the given 
frequencies. 
2. Design for LPF & HPF separately and then combine the circuit by first placing the HPF 
followed by a LPF (i.e) HPF in series with LPF. 
3. Connect the circuit as shown in the circuit diagram. 
4. Apply a constant voltage input sinusoidal signal to the non-inverting terminal of op-amp. 
5. Tabulate the output voltage Vo with respect to different values of input frequency. 
6. Calculate passband gain and plot the graph of frequency versus voltage gain & check the 
graph to get approximately the same characteristic as shown in the model graph

## DESIGN:LPF & HPF:

<img width="429" height="324" alt="image" src="https://github.com/user-attachments/assets/b0f0ac0a-3006-494c-9096-e91ae2d6e87c" />

# DESIGN: BAND PASS FILTER
Design a BPF to pass a band of 400Hz to 2KHz with a pass band gain of 4.  
1. Select the highest cut-off frequency of LPF as fH = 10 KHz and the lowest cut-off frequency 
of HPF as fL = 1 KHz.  
2. Design the HPF first by taking fL = 1KHz. Assume the value of C < 1μf.  
Let C = 0.1μf.  
3. Calculate R from the expression.  
Given: fH = 2KHz  = 1/ (2πR1C1) 
   Let C1 = 0.1 µF, R1 = 7.9 KΩ 
Given: fL = 400Hz  = 1/ (2πR2C2) 
   Let C2 = 0.1 µF, R2 = 39.8 KΩ 
  Pass band Gain=4 
   Now   Ao = 1 + (Rf / R1)  
               2-1=(Rf / Ri) 
                Ri = Rf 
                 Let  Ri = Rf = 10 KΩ
## TABULATION:
## LOW_PASS

<img width="1089" height="924" alt="image" src="https://github.com/user-attachments/assets/4d258f81-338c-454c-a17f-52a9cb54c0a1" />

## HIGH-PASS

<img width="1280" height="1213" alt="image" src="https://github.com/user-attachments/assets/aa5c126f-a081-4466-8a9e-2e893a543765" />

## BAND-PASS

<img width="1280" height="1156" alt="image" src="https://github.com/user-attachments/assets/f49c9a9e-f807-41e4-96a8-d4bda7f2c122" />


## GRAPH:
## LOW_PASS

<img width="1280" height="829" alt="image" src="https://github.com/user-attachments/assets/e41e9aaa-dd08-4cf6-ab37-5f3b1a2a6cc6" />

## HIGH-PASS

<img width="1280" height="857" alt="image" src="https://github.com/user-attachments/assets/cd8d0de1-c904-4595-8d6d-0a0f1ea14b56" />

## BAND-PASS

<img width="1280" height="809" alt="image" src="https://github.com/user-attachments/assets/28ddbf16-5e1a-4674-82f1-b793047ab79a" />

 ## RESULTS:
Thus an Active Low pass, High pass and Band Pass Filters are designed and 
tested using op-amp IC 741. 

