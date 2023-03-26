# Sibilla

Sibilla is a 10HP eurorack module based on a DSP platform that can easily be updated via USB without the need for external programs. 
During its development we had to take so many decision in terms of signal routing, compromise stuff to achieve more playability, and many times we were forced to choose only one great idea from the many cool possibility we had in mind. So, why not gradually releasing alternative firmwares to the original one? Why not seeing what other people are capable of?

## Story and introduction

Sibilla is a digital stereo oscillator that aims to traslate into music the beauty and harshness of a semi-barren mountain. Its sound is sculpted by various saw and sine waves running through intricate delay networks, altered by LFOs, white noises and creating constructive and destructive interferences.

Both stereo channels are the output stages of two feedback audio loops.
Each loop is made up by a main sub sinusoidal wave oscillator and two saw and sine waves with frequencies affected by the generation of harmonics (right channel) and subharmonics (left channel). All waves have different phases whose offset is constantly affected by minor variations created by two pairs of grains randomly fluctuating within the waves amplitude spectrum and being sampled at a certain speed.
Waves then meet to each other to a common point, together with two white noise sources, creating constructive and destructive interferences constantly affected by two LFOs movements.
Interferences are then run into a resonant low pass filter and then distributed to four different delay lines from which they are fed back into the audio loops at different time intervals depending on the grains movements.

#### Current draw
- +12V: 125mA;
- -12V: 30mA;
- +5V: 0mA;

Please note that the above current consumption is highly influenced by the code Sibilla is running and refers to the Sibilla v.1.0 firmware.
