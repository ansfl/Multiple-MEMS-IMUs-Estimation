&nbsp; &nbsp;  &nbsp;  &nbsp; &nbsp;  &nbsp;  &nbsp; &nbsp;  &nbsp;  &nbsp; &nbsp;  &nbsp;  &nbsp; &nbsp;  &nbsp;  &nbsp;  <img src="https://github.com/ansfl/MEMS-IMU-Denoising/blob/main/figrues/Logo.png?raw=true" width="500" />

<!-- # MEMS-IMU-Denoising
This repository contains both code and experimental data associated with our paper "Parametric and State Estimation of Stationary MEMS-IMUs: A Tutorial". -->

## Introduction
Inertial navigation systems (INS) are widely used in almost any operational environment, including aviation, marine, and land-based vehicles. Inertial measurements from accelerom- eters and gyroscopes, allow the INS to estimate position, velocity, and orientation of its host vehicle. However due to inherent sensor bias and noise, accuracy is degraded over time, as these error sources propagate into the state estimates, causing them to drift. To mitigate this, different approaches of parametric and state estimation have been proposed, to compensate for undesirable errors, by either frequency-domain filtering, or external information fusion. A candidate solution that is often overlooked is the use of multiple sensors. The increased sampling of the observed phenomenon, results in the improvement of several key factors such as signal accuracy, frequency resolution, noise rejection, and higher redundancy. In this study, a stationary and levelled sensors array is taken, and its robustness against the instrumental errors is simplified and analyzed. Subsequently, the hypothesized model is compared with the experimental results, and the level of agreement between them is thoroughly discussed. Ultimately, our results showcase the vast potential of employing multiple sensors, as we observe improvements spanning from the signal level to each navigation state.

&nbsp; &nbsp;  &nbsp; &nbsp; &nbsp;  &nbsp;  &nbsp; &nbsp;  &nbsp; &nbsp; <img src="https://github.com/ansfl/Multiple-MEMS-IMU-Estimation/blob/main/figures/Fig_Ellipsoid_Medium_B.png?raw=true" width="500" class='center'/>



&nbsp; &nbsp;  &nbsp; &nbsp; &nbsp;  &nbsp;  &nbsp; &nbsp;  &nbsp; &nbsp; <img src="https://github.com/ansfl/Multiple-MEMS-IMU-Estimation/blob/main/figures/PDF_vs_Time_Fin.png?raw=true" width="500" class='center'/>

&nbsp; &nbsp;  &nbsp; &nbsp; &nbsp;  &nbsp;  &nbsp; &nbsp;  &nbsp; &nbsp; <img src="https://github.com/ansfl/Multiple-MEMS-IMU-Estimation/blob/main/figures/Fig_combined.png?raw=true" width="500" class='center'/>


Next, we compare their effectiveness over the well-known stationary coarse alignment procedure, where roll and pitch angles are being evaluated from specific forces. Based on the benchmarking results obtained in field experiments, we show that: (i) learning-based models perform better than traditional signal processing filtering; (ii) non-parametric kNN algorithm outperforms all state of the art deep learning models examined in this study; (iii) denoising can be fruitful for pure inertial signal reconstruction, but moreover for navigation-related tasks, as both errors are shown to be reduced up to one order of magnitude.

&nbsp; &nbsp; &nbsp;  &nbsp; &nbsp;  &nbsp; &nbsp; &nbsp;  &nbsp;  &nbsp; &nbsp;  &nbsp; &nbsp; <img src="https://github.com/ansfl/MEMS-IMU-Denoising/blob/main/figrues/VID_levelling.gif" width="650" class='center'/>

## Dataset

<!-- Autonomous Navigation and Sensor Fusion Lab -->
The inertial measurements are obtained from a dedicated apparatus for alignment and synchronization of two arrays of five inertial MEMS-IMU  [`Xsense-DOT`](chrome-extension://oemmndcbldboiebfnladdacbdfmadadm/https://www.xsens.com/hubfs/Downloads/DOT/Documents/2021-07%20-%20Archived%20-%20Xsens%20DOT%20User%20Manual%20.pdf). 

&nbsp; &nbsp;  &nbsp;  &nbsp; &nbsp;  &nbsp;  &nbsp; &nbsp;  &nbsp; &nbsp;  &nbsp;  &nbsp; 
&nbsp;  &nbsp;  &nbsp; &nbsp;  &nbsp;  &nbsp; &nbsp;  &nbsp;  &nbsp; <img src="https://github.com/ansfl/Multiple-MEMS-IMU-Estimation/blob/main/figures/Fig_XSENS_1.jpg?raw=true" width="500" class='center'/>


## Code

Execution code is straight forward, and for convenience, concentrated in one consolidated Python notebooks, enabling reproduction of our results.


### Directory tree
<pre>
[root directory]
├── figures
├── data
├── code
|   └── *execution.ipynb*
...
└── requirements.txt
<!--  Readme.md -->
</pre>


## Citation

If you found the paper's CODE helpful in your research, please cite our paper:
```
@article{engelsman2023multiple,
  title={Parametric and State Estimation of Stationary MEMS-IMUs: A Tutorial},
  author={Engelsman, Daniel, and Stolero, Yair, and Klein, Itzik},
  journal={arXiv},
  year={2023},
}
```

[<img src=https://upload.wikimedia.org/wikipedia/commons/thumb/a/a8/ArXiv_web.svg/250px-ArXiv_web.svg.png width=70/>](https://arxiv.org/abs/2206.05937)
