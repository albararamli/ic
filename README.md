# Initial Contact (IC) Detection from Accelerometer Data

Welcome to our repository. We have developed an algorithm that detects Initial Contact (IC) events from raw accelerometer data. This algorithm identifies each step's IC events, represented as red dots in our visualizations, and marks the beginning and end of each step (duration), depicted with gray borders. Further, it estimates the total count of steps taken. 

## Visualizations

Understanding data and its transformations are crucial. Therefore, we provide visualizations of both the input and output data of our IC detection process:

**Input Signal**
:-----------------------:
![Input Signal](https://albara.ramli.net/download/xin.liu/dmd/ic/in.png)

**Output Signal**
:-----------------------:
![Output Signal](https://albara.ramli.net/download/xin.liu/dmd/ic/out.png)

## Data Requirements

Included in this repository is an example CSV file that demonstrates the expected accelerometer data format for this algorithm. For optimal results, use files exported directly from the Walk4Me system.

If you're generating your own data file, ensure it adheres to these guidelines:
- A z_axis column is mandatory, as it represents accelerometer readings along the z-axis.
- The data rows must be sorted in a chronological order to represent time progression.
Strict adherence to these standards ensures the successful operation of the IC detection process.

## Tunable Hyperparameters

Our code allows fine-tuning through several hyperparameters to meet the unique requirements of your accelerometer data. 

```python
# Filter and original signal hyperparameters
FILTER_LEVEL_DISTANCE, FILTER_LEVEL_HEIGHT, FILTER_CUTOFF_FREQ = 30, 0.008, 0.029  # filter levels and cutoff frequency
ORI_LEVEL_DISTANCE, ORI_LEVEL_HEIGHT = 1, -1  # original signal levels for distance and height
```

While these hyperparameters provide a certain level of control, we highly recommend validating your results against a ground truth or reference data whenever you modify these parameters.

## Acknowledging Our Work

If you find our code useful, we kindly request you to cite our paper in your work:

- **Automated Detection of Gait Events and Travel Distance Using Waist-worn Accelerometers Across a Typical Range of Walking and Running Speeds**\
Authors: Albara Ah Ramli, Xin Liu, Kelly Berndt, Chen-Nee Chuah, Erica Goude, Lynea B. Kaethler, Amanda Lopez, Alina Nicorici, Corey Owens, David Rodriguez, Jane Wang, Daniel Aranki, Craig M. McDonald, Erik K. Henricson

Cite using bibtex:
```bibtex
@article{ramli2023,
  author = {Ramli, Albara Ah and Liu, Xin and Berndt, Kelly and Chuah, Chen-Nee and Goude, Erica and Kaethler, Lynea B. and Lopez, Amanda and Nicorici, Alina and Owens, Corey and Rodriguez, David and Wang, Jane and Aranki, Daniel and McDonald, Craig M. and Henricson, Erik K.},
  title = {Automated Detection of Gait Events and Travel Distance Using Waist-worn Accelerometers Across a Typical Range of Walking and Running Speeds}
}
```
<!--,
  journal={Gait & Posture},
  year={2023},
  publisher={Elsevier}-->

## Further Reading

For a comprehensive understanding of our work and its various applications, please refer to the following research papers:

- **Gait Characterization in Duchenne Muscular Dystrophy (DMD) Using a Single-Sensor Accelerometer: Classical Machine Learning and Deep Learning Approaches** [[PDF](https://arxiv.org/abs/2105.06295)]\
Authors: Albara Ah Ramli, Xin Liu, Kelly Berndt, Erica Goude, Jiahui Hou, Lynea B. Kaethler, Rex Liu, Amanda Lopez, Alina Nicorici, Corey Owens, David Rodriguez, Jane Wang, Huanle Zhang, Daniel Aranki, Craig M. McDonald, Erik K. Henricson

- **Walk4Me: Telehealth Community Mobility Assessment, An Automated System for Early Diagnosis and Disease Progression** [[PDF](https://arxiv.org/abs/2305.05543)]\
Authors: Albara Ah Ramli, Xin Liu, Erik K Henricson

## Getting Started

To dive into our code, clone this repository and install the necessary packages. You can then execute the main Python script to launch the IC detection process. We hope you find our work insightful.
