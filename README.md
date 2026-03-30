# Digital-Signal-Processing--Correlation
## AIM:
To generate discrete auto correlation and cross correlation of signals using MATLAB.
## APPARATUS REQUIRED:
MATLAB R2012.
## ALGORITHM:
Step 1: Open matlab. Write the program.

Step 2: Read the input sequence 1 and input sequence 2 sequence.

Step 3: Perform auto correlation and cross correlation for both the sequences. 

Step 4: Plot the output sequence with x-label and y-label with suitable title.

Step 5: Terminate the program.


## PROGRAM: 
```
clc; % clear screen
clear all; % clear screen
close all; % close all figure windows
% INPUT SIGNAL-1
a=input('enter the starting x(n)');
x=input('Enter the x(n) sequence');
n=a:1:length(x)+a-1;
figure(1)
stem(n,x)
xlabel('Time')
ylabel('Amplitude')
title('Input Signal-1')
% INPUT SIGNAL 2
b=input('enter the starting y(n)');
y=input('Enter the y(n) sequence');
m=input('enter the ending of y(n)');
n1=b:1:length(y)+b-1;
figure(2)
stem(n1,y)
xlabel('Time')
ylabel('Amplitude')
title('Input signal-2')
% DISCRETE AUTO CORRELATED SIGNAL
out1=xcorr(x,x)
n2=a-m:1:length(out1)+a-m-1;
figure(3)
stem(n2,out1)
xlabel('Time')
ylabel('Amplitude')
title(' Discrete auto correlated waveform')
% DISCRETE CROSS CORRELATED SIGNAL
out2=xcorr(x,y);
n3=a-m:1:length(out2)+a-m-1;
figure(4)
stem(n3,out2)
xlabel('Time')
ylabel('Amplitude')
title(' Discrete cross correlated waveform')
```


## OUTPUT:
<img width="837" height="746" alt="image" src="https://github.com/user-attachments/assets/37231cc6-c020-4f37-ad0e-8c19558e815e" />
<img width="832" height="744" alt="image" src="https://github.com/user-attachments/assets/147404e4-5a49-424a-ac2a-d0a968edc06d" />
<img width="837" height="751" alt="image" src="https://github.com/user-attachments/assets/94da7a06-495f-4cde-b701-095d60de5e10" />
<img width="836" height="744" alt="image" src="https://github.com/user-attachments/assets/2360b172-34dc-492d-b42b-a4fae4005949" />





## RESULT:
<img width="1600" height="702" alt="image" src="https://github.com/user-attachments/assets/70c345eb-9542-4cfe-bd06-f59a79e7e1c4" />

