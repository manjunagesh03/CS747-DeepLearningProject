*Deep Learning-Based Adaptive Channel Code Selection for UAV-to-Ground Broadcast Communications in 6G*
&nbsp;
Course: CS 747 – Deep Learning
&nbsp;
Team Members: Farhan Nawaz, Manju Nagesh 
&nbsp;
Project Status: In Development
&nbsp;

Project Overview-
This project investigates the use of deep learning to improve the reliability and efficiency of UAV-to-ground broadcast communications in 6G wireless networks.
A single Unmanned Aerial Vehicle (UAV) broadcasts information to multiple ground sensor nodes. As the UAV moves, wireless channel conditions change due to variations in distance, elevation angle, signal strength, and fading.
The goal is to develop a deep learning-based system that adaptively selects Polar-code configurations based on channel conditions, balancing broadcast reliability and communication throughput.
We compare reactive and predictive deep learning approaches to determine whether incorporating historical channel information improves coding decisions, particularly during rapidly changing wireless conditions.


System Features-
The system uses four channel-related features for each ground sensor: SNR (Signal-to-Noise Ratio, representing received signal quality), K-factor (Rician fading parameter representing line-of-sight strength), Elevation (Angle between the ground sensor and UAV), Distance.
These features are used to predict an appropriate coding configuration for upcoming UAV broadcasts.


Methodology-
1. UAV and Channel Simulation
  (Simulate UAV movement and multiple ground sensor nodes. Generate time-varying channel measurements based on UAV geometry and Rician fading.)
2. Polar-Code Evaluation
  (Use the NVIDIA Sionna library to simulate Polar encoding, transmission, and decoding under different channel conditions.)
3. Dataset Generation
  (Evaluate candidate coding configurations and generate labeled training examples using the best-performing configurations according to the selected optimization objective.)
4. Deep Learning
  (Train the reactive MLP and predictive LSTM using simulated channel information.)
5. Evaluation
  (Compare the models against fixed and random baselines using metrics such as: Broadcast coverage, Bit Error Rate (BER) or Block Error Rate (BLER), Effective throughput, Performance under different UAV mobility conditions.)

Technologies-
1. Python (Main programming language)
2. NVIDIA Sionna (Wireless communication and Polar-code simulations)
3. TensorFlow/Keras (Neural network development)
4. NumPy/Pandas (Numerical computation and data processing)
5. Matplotlib (Experimental plots and visualization)
6. Git/GitHub (Version control and collaboration)

