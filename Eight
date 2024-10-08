clc; clear all; close all;
n = -250:250;
wc = 0.4;
hd = ((wc/pi).*sinc(wc.*n));
stem(hd);
figure

w = ones(1,201);
stem(w);
hw = hd(150:350).*w;
figure;
stem(hw);
a = 1; b = hw;
figure; freqz(b,a);figure;

w = transpose(bartlett(201));
stem(w);
hw = hd(150:350).*w;
figure;
stem(hw);
a = 1; b = hw;  figure; freqz(b,a);figure;

% for hamming window (cosine window)
w = transpose(hamming(201));
stem(w);
hw = hd(150:350).*w;
figure;
stem(hw);  a = 1; b = hw;  figure; freqz(b,a);figure;

% for hanning window
w = transpose(hanning(201));
stem(w);
hw = hd(150:350).*w;
figure;
stem(hw);  a = 1; b = hw;  figure; freqz(b,a);
