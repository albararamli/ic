# Initial Contact (IC) Detection in Accelerometer Signals

This repository hosts the code for detecting Initial Contact (IC) events from raw accelerometer signals. The code identifies each step's IC events (visualized as red dots), marks the beginning and end of each step (duration, depicted with gray borders), and estimates the total step count.

## Visualization
Below are examples demonstrating the input and output from the IC detection process:

Input Signal             
:-----------------------:
![](https://albara.ramli.net/download/xin.liu/dmd/ic/in.png)

Output Signal
:-----------------------:
![](https://albara.ramli.net/download/xin.liu/dmd/ic/out.png)

## Hyperparameters
This code has several hyperparameters which you can adjust and fine-tune according to your requirements:

```python
# Define levels and cutoff frequency
FILTER_LEVEL_DISTANCE = 30
FILTER_LEVEL_HEIGHT = 0.008
FILTER_CUTOFF_FREQ = 0.029
ORI_LEVEL_DISTANCE = 1
ORI_LEVEL_HEIGHT = -1
```
These hyperparameters determine the filtering level for distance and height of the signal, as well as the filter's cutoff frequency. Feel free to experiment with these values to optimize the IC detection for your specific use case. Remember to always validate your results against your ground truth or reference data when adjusting these parameters.

## Citation
If you utilize this code, kindly reference the following paper:

- **Automated Detection of Gait Events and Travel Distance Using Waist-worn Accelerometers Across a Typical Range of Walking and Running Speeds**\
Authors: Albara Ah Ramli, Xin Liu, Kelly Berndt, Chen-Nee Chuah, Erica Goude, Lynea B. Kaethler, Amanda Lopez, Alina Nicorici, Corey Owens, David Rodriguez, Jane Wang, Daniel Aranki, Craig M. McDonald, Erik K. Henricson

## Further Reading
For an in-depth understanding of the underlying technology and its various applications, consider referring to these research papers:

- **Gait Characterization in Duchenne Muscular Dystrophy (DMD) Using a Single-Sensor Accelerometer: Classical Machine Learning and Deep Learning Approaches** [[PDF](https://example.com/link_to_second_paper)]\
Authors: Albara Ah Ramli, Xin Liu, Kelly Berndt, Erica Goude, Jiahui Hou, Lynea B. Kaethler, Rex Liu, Amanda Lopez, Alina Nicorici, Corey Owens, David Rodriguez, Jane Wang, Huanle Zhang, Daniel Aranki, Craig M. McDonald, Erik K. Henricson

- **Walk4Me: Telehealth Community Mobility Assessment, An Automated System for Early Diagnosis and Disease Progression** [[PDF](https://arxiv.org/abs/2305.05543)]\
Authors: Albara Ah Ramli, Xin Liu, Erik K Henricson

## How to Use
To leverage this code, clone this repository and install the necessary packages. Run the main Python script to start the IC detection process.
