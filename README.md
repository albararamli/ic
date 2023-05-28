Here's an enhanced and professional version of your repository description:

---

# Initial Contact (IC) Detection from Accelerometer Signals 

Welcome to our repository, where we present our code designed to detect Initial Contact (IC) events from raw accelerometer data. This algorithm not only identifies each step's IC events, represented as red dots in our visualizations, but it also accurately marks the beginning and end of each step (duration), depicted with gray borders. Further, it estimates the total count of steps taken. 

## Visual Representation

To help you better understand our process, we've provided illustrations of both the input data and the output of our IC detection below:

**Input Signal**
:-----------------------:
![Input Signal](https://albara.ramli.net/download/xin.liu/dmd/ic/in.png)

**Output Signal**
:-----------------------:
![Output Signal](https://albara.ramli.net/download/xin.liu/dmd/ic/out.png)

## Hyperparameters

Our code comes equipped with several hyperparameters. These are adjustable and can be fine-tuned to meet the specific requirements of your accelerometer data. 

```python
# Hyperparameters for the filter and orientation signals
FILTER_LEVEL_DISTANCE, FILTER_LEVEL_HEIGHT, FILTER_CUTOFF_FREQ, ORI_LEVEL_DISTANCE, ORI_LEVEL_HEIGHT = 30, 0.008, 0.029, 1, -1
```

The above hyperparameters control the filter level for distance and height of the accelerometer signal, as well as the cutoff frequency of the filter. Experimenting with these parameters might help you optimize the IC detection for your specific needs. However, we strongly recommend validating your results against a ground truth or reference data whenever you adjust these parameters.

## Cite Our Work

We request that if you use our code, please cite the following paper in your work:

- **Automated Detection of Gait Events and Travel Distance Using Waist-worn Accelerometers Across a Typical Range of Walking and Running Speeds**\
Authors: Albara Ah Ramli, Xin Liu, Kelly Berndt, Chen-Nee Chuah, Erica Goude, Lynea B. Kaethler, Amanda Lopez, Alina Nicorici, Corey Owens, David Rodriguez, Jane Wang, Daniel Aranki, Craig M. McDonald, Erik K. Henricson

## Recommended Reading

For more comprehensive insight into our technology and its various applications, we recommend the following research papers:

- **Gait Characterization in Duchenne Muscular Dystrophy (DMD) Using a Single-Sensor Accelerometer: Classical Machine Learning and Deep Learning Approaches** [[PDF](https://example.com/link_to_second_paper)]\
Authors: Albara Ah Ramli, Xin Liu, Kelly Berndt, Erica Goude, Jiahui Hou, Lynea B. Kaethler, Rex Liu, Amanda Lopez, Alina Nicorici, Corey Owens, David Rodriguez, Jane Wang, Huanle Zhang, Daniel Aranki, Craig M. McDonald, Erik K. Henricson

- **Walk4Me: Telehealth Community Mobility Assessment, An Automated System for Early Diagnosis and Disease Progression** [[PDF](https://arxiv.org/abs/2305.05543)]\
Authors: Albara Ah Ramli, Xin Liu, Erik K Henricson

## Get Started

To utilize our code, simply clone this repository and install the required packages. You're then ready to execute the main Python script to initiate the IC detection process. Enjoy exploring!
