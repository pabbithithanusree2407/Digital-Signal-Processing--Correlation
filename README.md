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
<img width="1891" height="1018" alt="Screenshot 2026-02-22 224711" src="https://github.com/user-attachments/assets/675eae45-e6a6-4f91-9036-42e507b8c1ec" />
<img width="1902" height="1006" alt="Screenshot 2026-02-22 224755" src="https://github.com/user-attachments/assets/8e5e7688-3a48-4935-9c32-95bb41f98a8d" />
<img width="1855" height="972" alt="Screenshot 2026-02-22 225730" src="https://github.com/user-attachments/assets/d82ab52b-d7a6-4ea6-b88e-d33b7ce11309" />
<img width="1902" height="1032" alt="Screenshot 2026-02-22 225521" src="https://github.com/user-attachments/assets/b4ac9342-9d39-43e2-8487-8f314239abff" />


## RESULT:
![WhatsApp Image 2026-03-30 at 8 42 46 PM](https://github.com/user-attachments/assets/e093fa23-4869-4898-88d8-c75d637ed65d)

