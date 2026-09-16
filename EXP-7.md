# AIM:
To implement error control coding schemes with linear block codes using MATLAB.

# SOFTWARE REQUIRED: 
  MATLAB

# PROGRAM:
# ERROR CODING
# ENCODING:
~~~
clc;
clear;
close all;

% Generator matrix for (7,4) cyclic Hamming code
G = [1 0 0 0 1 0 1;
    0 1 0 0 1 1 1;
    0 0 1 0 1 1 0;
    0 0 0 1 0 1 1];

% Message bits
msg = [1 0 0 1;
    1 0 1 0;
    1 0 1 1];

% Encoding
code = mod(msg * G, 2);

disp('Message Bits:')
disp(msg)

disp('Generator Matrix:')
disp(G)

disp('Encoded Codewords:')
disp(code)
~~~
# ENCODING OUTPUT:
<img width="450" height="383" alt="image" src="https://github.com/user-attachments/assets/9da8c939-4de4-4e5b-92aa-7cefc2c739d6" />

# DECODING PROGRAM:
~~~
clc;
clear all;
close all;

q = 3;
n = 2^q - 1;
k = n - q;

% Parity check matrix for Hamming (7,4)
parmat = [1 0 1 0 1 0 1;
          0 1 1 0 0 1 1;
          0 0 0 1 1 1 1];

recd = [1 0 1 1 1 1 0];

% Calculate syndrome
syndrome = rem(recd * parmat', 2);

% Convert binary syndrome to decimal
syndrome_de = syndrome(1)*4 + syndrome(2)*2 + syndrome(3);

disp(['Syndrome = ', num2str(syndrome_de), ...
      ' (decimal) ', num2str(syndrome), ' (binary)']);

% Error correction
corrvect = zeros(1,n);

if syndrome_de ~= 0
    corrvect(syndrome_de) = 1;
end

% Correct received code
correctedcode = rem(recd + corrvect, 2);

disp('Parity check matrix:');
disp(parmat);

disp('Correction vector:');
disp(corrvect);

disp('Corrected code:');
disp(correctedcode);
~~~
# DECODING OUTPUT:
<img width="492" height="288" alt="image" src="https://github.com/user-attachments/assets/4e013a82-bb6f-49e2-bd6c-e3f58d50c290" />

# RESULT:
Thus encoding and decoding of block codes are performed using MATLAB.
