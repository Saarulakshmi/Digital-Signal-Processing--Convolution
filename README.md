# Digital-Signal-Processing--Convolution
## Aim:
To perform linear convolution using MAT LAB.
## Software Required:
MAT LAB R2012
## Algorithm:
Step 1: Open mat lab. Write the program.

Step 2: Read the first input sequence.

Step 3: Read the second impulse sequence.

Step 4: Plot the input sequences with x-label and y-label with suitable title. 

Step 5: Perform convolution for both the sequences using conv2() function.
  
Step 6: Plot the sequence with x-label and y-label with suitable title

Step 7: Terminate the program.

## PROGRAM: 
```
% Saaru lakshmi D [212223050040]

clc; % clear screen
clear all; % clear screen
close all; % close all figure windows

% input sequence
% 𝑥[𝑛]={2.5,−3,1,3.5,2.4,6} and ℎ[𝑛]={3,−12.5,−3,1,2.5}

a = input("enter the starting x(n)");
x = input("enter the x(n) sequence");
n = a:1:length(x)+a-1;
figure(1);
stem(n,x);
xlabel('time');
ylabel('amplitude');
title('input sequence');

%impulse sequence

b= input('enter the starting h(n)');
y = input('enter the h(n) sequence');
m = b:1:length(y)+b-1;
figure(2);
stem(m,y);
xlabel('time');
ylabel('amplitude');
title('impulse response');

%linear convolution

z = conv2(x,y);
n1 = a+b:1:length(z)+a+b-1;
figure(3);
stem(n1,z);
xlabel('time');
ylabel('amplitude');
title('linear convolution');
```

## OUTPUT:
<img width="1600" height="737" alt="image" src="https://github.com/user-attachments/assets/058d0134-0359-4bb8-a6e6-371696645b22" />
<img width="1600" height="765" alt="image" src="https://github.com/user-attachments/assets/68c91010-db85-4832-bd81-c870a0aa74e7" />
<img width="1600" height="777" alt="image" src="https://github.com/user-attachments/assets/1218e8ac-233b-424c-9669-6a135894f8f5" />



## RESULT:
The linear Convolution of signal is 𝒚[𝒏] = {7.5,-40.25,33,9.5,-36.3,-29,-76.2,-6.85,12,15}

