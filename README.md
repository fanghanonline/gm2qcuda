# gm2qcuda 
The gm2qcuda project is developed for Muon g-2 experiment Q-method(Integrated-energy Method) Analysis. The authors include Tim, Wes and Ran Hong. It is base on the code of [QMethodUtilities](https://github.com/hongran/QMethodUtilities) maintained by Ran Hong. The gm2cuda uses Nvidia cuda to simulate positron energy deposited in the calorimeter as in the real expriment. Interaction with the materials is not the point of the simulation. The energy distribution is calculated with a series of empirical parameters and simple fucntions.
## Organization of the Code
The input
## Build Prerequisites
- CMake 3.10+
- CUDA 10.0+
- GNU Build Tool 8.0+
- CERN ROOT 6.0 +
## How to Build
Make a ```build_dir```.
```cd build```
```cmake ..```
```make -j16```
## Run the Simulation
```cd build```
```./QSimulation -c ../input/FFT_ADCHist_elab2.0.json -flush 10240 -run 3 ```