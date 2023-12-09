# Van der Pol-informed Neural Networks for Multi-step-ahead Forecasting of Extreme Climatic Events

In this study, we propose a novel Van der Pol-informed Neural Networks (VPINN) model for generating multi-step forecasts of extreme climatic events. The VPINN framework leverages the dynamics of the Van der Pol oscillatory system to generate reliable forecasts in chaotic datasets. Our study considers publicly available real-world climatic datasets namely -  Turkey seismic waves, El Niño sea surface temperature, Philippines temperature, Madrid humidity, and Delhi wind speed[1-2] to analyze the forecasting ability of our proposed model. A graphical representation of the study is provided below:
![Poster](https://github.com/mad-stat/VPINN/blob/main/Codes/New_Poster.png)

Usage of the repository for the paper "Van der Pol-informed Neural Networks for Multi-step-ahead Forecasting of Extreme Climatic Events [3]".

* The training phase of the proposed VPINN model initially simulates data from the Van der Pol oscillatory system with default/user-specified parameters and calculates time-derivates for the simulated series in a task-agnostic manner. 
  
* Subsequently, the VPINN model having been pre-trained with the dynamics of the non-linear system models the real-world datasets using an LSTM network with physics-informed loss regularization.
  
* This framework transfers its knowledge gained from the Van der Pol oscillator through the time derivates and analyzes them along with the real-world climatic data in a multivariate setting.

* In the model training the architecture leverages a combination of data-centric loss and a physics-informed loss function to enforce the dynamics of the Van der Pol oscillator on the prediction.
  
* The [VPINN](https://github.com/mad-stat/VPINN/blob/main/Codes/VPINN_Codeipynb.ipynb) file contains the source code and the implementation of the proposed VPINN model. A simulated series from the Van der Pol oscillator with parameter value 4 is made available here [Van der Pol data](https://github.com/mad-stat/VPINN/blob/main/Dataset/van_der_pol_intermittency.dat). Real-world datasets used in the experiments are provided in [Dataset](https://github.com/mad-stat/VPINN/tree/main/Dataset).

## Citing Our Work
Dutta, Anurag, Madhurima Panja, Uttam Kumar, Chittaranjan Hens, and Tanujit Chakraborty.\
"Van der Pol-informed Neural Networks for Multi-step-ahead Forecasting of Extreme Climatic Events."\
In NeurIPS 2023 AI for Science Workshop. 2023.

@inproceedings{dutta2023van,\
  title={Van der Pol-informed Neural Networks for Multi-step-ahead Forecasting of Extreme Climatic Events},\
  author={Dutta, Anurag and Panja, Madhurima and Kumar, Uttam and Hens, Chittaranjan and Chakraborty, Tanujit},\
  booktitle={NeurIPS 2023 AI for Science Workshop},\
  year={2023}
}

## References
* <a id="1">[1]</a> [Weather Underground](https://www.wunderground.com/)
* <a id="2">[2]</a> [National Centers for Environmental Information](https://www.ncei.noaa.gov/)
* <a id="3">[3]</a> [Van der Pol-informed Neural Networks for Multi-step-ahead Forecasting of Extreme Climatic Events](https://openreview.net/attachment?id=OQXCc21rgM&name=pdf)
