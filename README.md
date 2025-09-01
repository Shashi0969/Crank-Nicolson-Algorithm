# Time Evolution of a Quantum Wave Packet in a 1D Box

This project simulates the time evolution of a quantum particle in a 1D infinite potential well using the Crank–Nicolson method. The simulation visualizes the probability density, real part, and imaginary part of the wavefunction through 2D/3D plots and animations.

I have designed the simulation inspired by Adib Kabir's [Numerical Simulation of the Time-Dependent Schrödinger Equation Using the Crank-Nicolson Method](https://arxiv.org/pdf/2410.10060)

Python libraries used: NumPy, SciPy, and Matplotlib
## Features 
- Numerical solution of the time-dependent Schrödinger equation (TDSE).
- Implementation of the Crank–Nicolson scheme with sparse matrices for efficiency.
- Multiple visualization modes:
  - **2D plots** at single or multiple timesteps.
  - **3D plots** of the wavefunction.
  - **2D** and **3D** animations of the wave packet evolution.
  - Option to save animations as .mp4 files (requires ffmpeg).
## Requirements 
Ensure you have the following Python packages installed : 
```
python -m pip install numpy matplotlib scipy
```
Additionally, ffmpeg is required if you want to save animations as videos.
## How to Run 
Clone the repository:
```
git clone https://github.com/Shashi0969/Crank-Nicolson-Algorithm.git
cd Crank-Nicolson-Algorithm
```
Run the script:
```
Particle_in_a_1D_box.py
```
You will be prompted with options:
```
Enter '1' to start and '0' to terminate :
```
If you enter 1, you can choose:
1. 2D plot at 2000th step
2. 3D plot at 2000th step
3. 2D plots at 500th, 1000th, 1500th, and 2000th steps
4. 3D plots at 500th, 1000th, 1500th, and 2000th steps
5. 2D animation of evolution
6. 3D animation of evolution
### Example Outputs
- **2D Plot**: Probability density, real and imaginary parts at a specific timestep.
- **3D Plot**: Real vs imaginary part evolution in 3D space.
- **Animation**: Continuous time evolution of the wavefunction.

- ![Figure_2](outputs/Figure_2.png)
## Notes
- Default parameters simulate an electron in a 1D box of length $10^{-8}$ m.
- You can modify wave packet parameters (sigma, $k_0$, etc.) in the Start() function.
