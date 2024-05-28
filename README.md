# sim_tempering_3d_ising
#### Aim of the Project:

Investigate the magnetization of a 3D ferromagnetic Ising model as a function of temperature for various numbers of spins N, and explore the effectiveness of simulated tempering in improving sampling efficiency.

#### Methodology:

1) Implementation of the Metropolis Algorithm:

Simulate 3D ferromagnetic Ising models using the Metropolis algorithm.
Perform simulations for different numbers of spins N and a range of temperatures.

2) Simulated Tempering:

Implement simulated tempering to improve the sampling efficiency at different temperatures.
Use preliminary simulations to estimate the optimal weights $g_i$ for simulated tempering.

3) Data Collection:

Compute and record the average magnetization and energy for each lattice size at each temperature.

4) Analysis and Visualization:

Plot the magnetization and energy as functions of temperature for different lattice sizes.
Compare the results to understand how the number of spins affects the phase transition and magnetization behavior.

5) Verification of Simulated Tempering:

Verify that the weights $g_i$ are optimal by checking whether the probabilities P(β_i) are similar.
Compare the performance of simulated tempering with the plain Metropolis algorithm.

### Results

#### Implementation of the Metropolis Algorithm

The Metropolis algorithm was successfully implemented to simulate 3D ferromagnetic Ising models for different lattice sizes (\(N = 4, 6, 8\)) and a range of temperatures. The simulations captured the expected magnetization and energy behaviors, showing clear phase transitions.

#### Simulated Tempering

Simulated tempering was implemented to enhance sampling efficiency across temperatures. Preliminary simulations estimated the optimal weights \( $g_i$ \), which balanced the exploration of the temperature space.

#### Analysis and Visualization

**Magnetization vs. Temperature**:
- Smaller lattice sizes showed a gradual decrease in magnetization with temperature, indicating the transition from ordered to disordered states.
- Larger lattice sizes exhibited sharper transitions, highlighting the phase change more clearly.

**Energy vs. Temperature**:
- Energy remained low at lower temperatures, corresponding to ordered states, and increased with temperature, reflecting increased disorder.

**Energy Distribution**:
- Simulated tempering displayed a broader energy distribution, indicating better exploration of the energy landscape compared to the Metropolis algorithm.

#### Verification of Simulated Tempering

**Optimal Weights \( $g_i$ \)**:
- Probabilities \( P(\beta_i) \) were nearly uniform, confirming the optimal calculation of \( $g_i$ \).

**Comparison with Metropolis Algorithm**:
- Simulated tempering showed improved performance in exploring the energy landscape, avoiding local minima more effectively than the Metropolis algorithm.
- Temperature history during simulated tempering showed efficient transitions between temperatures.

Overall, simulated tempering significantly improved sampling efficiency and provided a more accurate representation of the 3D Ising model's behavior across different temperatures and lattice sizes, outperforming the plain Metropolis algorithm.
