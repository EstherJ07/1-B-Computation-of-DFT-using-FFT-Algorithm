# EXPT 1b: Computation-of-DFT-using-FFT-ALGORITHM

## AIM
To perform and verify DFT using FFT-ALGORITHM by SCILAB.
## APPARATUS REQUIRED
PC installed with SCILAB
## PROGRAM 
### DFT FFT-ALGORITHM
PROGRAM:
```
clc;
clear;
close;
xn=[1 1 1 1 1 1 0 0];
n1=0:1:length(xn)-1;
subplot(2,2,1);
plot2d3(n1,xn);
xlabel('time n');
ylabel('amplitude');
title('input sequence');
xk=fft(xn);
k1=0:1:length(xk)-1;
magnitude=abs(xk)
subplot(2,2,2);
plot2d3(k1,magnitude);
xlabel('frequency(Hz)');
ylabel('magnitude(gain)');
title('magnitude spectrum');

angle=atan(imag(xk),real(xk));
subplot(2,2,3);
plot2d3(k1,angle);
xlabel('frequency(Hz)');
ylabel('Phase');
title('phase spectrum');
y=ifft(xk);
n2=0:1:length(y)-1;
subplot(2,2,4);
plot2d3(n2,y);
xlabel('time n');
ylabel('amplitude');
title('inverse FFT of x(k)');
```

### CALCULATIONS:
<img width="900" height="1200" alt="image" src="https://github.com/user-attachments/assets/fbebe7e7-ae73-41e8-bf7d-0439305a3956" />
<img width="900" height="600" alt="image" src="https://github.com/user-attachments/assets/3510e0cd-6176-4a6c-9631-f164832d8451" />

### SAMPLE OUTPUT:
<img width="800" height="800" alt="image" src="https://github.com/user-attachments/assets/6c001b1f-9c37-49df-aaa0-f9dc5aa6543e" />


## RESULT:
Thus,  DFT using FFT-ALGORITHM for two given sequences were performed and its result was verified.

