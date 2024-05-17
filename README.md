This project aims to digitally replicate the electrical behavior of the MXR Distortion+ guitar pedal circuit.

**MATLAB Folder** 
The Matlab folder contains Matlab scripts based on the transfer function derived from the circuit discretization, and audio samples used as input signals in wave file format.

**How to Use the Matlab Scripts**
1. Import the script and audio file into Matlab.
2. Adjust the positions of the distortion knob (line 25) and the output knob (line 86) in the script. The distortion knob can be set from 0 to 1. For example, if you want to turn the knob halfway, enter 0.5, and for 75%, enter 0.75. Note that the maximum value for the output knob should be set to 0.999 instead of 1.
3. Run the script.
4. To compare the sound of the input and output signals, type and execute `play(input)` or `play(output)` in the console. To stop the sound, type `stop(input)` or `stop(output)`.

**realpedal_vs_VAmodel Folder:**  
The realpedal_vs_VAmodel folder contains audio files generated by setting the distortion knob to 50% and 75% using the above Matlab model, and recordings from the actual MXR Distortion+ guitar pedal. This allows for a comparison of the signal processing behavior between the actual pedal and the digital replication model.

**p.s.**  
Creating this model required a circuit discretization process using methods such as Nodal Analysis, Nodal DK method, and the Newton-Raphson method. If you would like a detailed report on the theory and calculations involved, please request it at imsohyun065@gmail.com.

Thank you!

Best,
Sohyun
