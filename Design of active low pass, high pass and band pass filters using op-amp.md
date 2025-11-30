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
<img width="1080" height="689" alt="image" src="https://github.com/user-attachments/assets/f4583556-32af-4052-808b-8ef0649c2575" />

## HIGH-PASS
<img width="1080" height="772" alt="image" src="https://github.com/user-attachments/assets/312e3e02-8f93-4390-bc21-08445696860f" />

## BAND-PASS
<img width="1080" height="689" alt="image" src="https://github.com/user-attachments/assets/2cdbac52-746e-47f8-91ed-a9b8be7e31bb" />

## MODEL GRAPH: 
## LOW_PASS
<img width="1080" height="821" alt="image" src="https://github.com/user-attachments/assets/e6bd0a1b-2b21-4881-b0cc-3f3dc48e9996" />

## HIGH-PASS
<img width="1080" height="724" alt="image" src="https://github.com/user-attachments/assets/f65a307a-385b-429b-811f-e27df39b5dbf" />

## BAND-PASS
<img width="1280" height="1263" alt="image" src="https://github.com/user-attachments/assets/75aa97ed-fd98-492e-a3b2-05a0820e93ce" />


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
<img width="1280" height="1087" alt="image" src="https://github.com/user-attachments/assets/ea54d63b-c89a-4c5c-8eee-dbaf01fe203f" />

## HIGH-PASS
<img width="1280" height="1073" alt="image" src="https://github.com/user-attachments/assets/fe09ffb6-ea38-4a48-88c1-7a49e5c0bf1d" />

## BAND-PASS
-<img width="1080" height="1215" alt="image" src="https://github.com/user-attachments/assets/70af58d7-d871-4caa-83d4-1c0efe4e3e58" />

## GRAPH:
## LOW_PASS

<img width="1534" height="1069" alt="image" src="https://github.com/user-attachments/assets/4c22effd-6fd9-45e3-9eba-3f839c427ce9" />

## HIGH-PASS
<img width="920" height="1280" alt="image" src="https://github.com/user-attachments/assets/b33205e1-6338-454e-a9f9-e9c811ae9afb" />

## BAND-PASS
<img width="732" height="1280" alt="image" src="https://github.com/user-attachments/assets/1ef7b8fe-76e0-46f3-b455-6a8d9c610d4c" />

 ## RESULTS:
Thus an Active Low pass, High pass and Band Pass Filters are designed and 
tested using op-amp IC 741. 

