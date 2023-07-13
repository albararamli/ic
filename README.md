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

This repository includes an example CSV file, 'a.csv,' which demonstrates the expected accelerometer data format for the algorithm. For optimal results, we recommend using files exported directly from the Walk4Me system.

If you generate your own data file, please adhere to the following guidelines:
- The presence of a 'z_axis' column is mandatory, as it represents accelerometer readings along the z-axis.
- Ensure that the data rows are sorted chronologically to accurately reflect the progression of time.

Strict adherence to these standards ensures the seamless operation of the IC detection process, yielding reliable results.

## Tunable Hyperparameters

Our code allows fine-tuning through several hyperparameters to meet the unique requirements of your accelerometer data. 

```python
# Filter and original signal hyperparameters
FILTER_LEVEL_DISTANCE, FILTER_LEVEL_HEIGHT, FILTER_CUTOFF_FREQ = 30, 0.008, 0.029  # filter levels and cutoff frequency
ORI_LEVEL_DISTANCE, ORI_LEVEL_HEIGHT = 1, -1  # original signal levels for distance and height
```

While these hyperparameters provide a certain level of control, we highly recommend validating your results against a ground truth or reference data whenever you modify these parameters.

## Acknowledging Our Work

If you find our code useful, valuable, or utilize it in any way, we expect that you cite our paper in your work.

- **Automated Detection of Gait Events and Travel Distance Using Waist-worn Accelerometers Across a Typical Range of Walking and Running Speeds**\
Authors: Albara Ah Ramli, Xin Liu, Kelly Berndt, Chen-Nee Chuah, Erica Goude, Lynea B. Kaethler, Amanda Lopez, Alina Nicorici, Corey Owens, David Rodriguez, Jane Wang, Daniel Aranki, Craig M. McDonald, Erik K. Henricson

Cite using bibtex:
```bibtex
@misc{ramli2023automated,
      title={Automated Detection of Gait Events and Travel Distance Using Waist-worn Accelerometers Across a Typical Range of Walking and Running Speeds}, 
      author={Albara Ah Ramli and Xin Liu and Kelly Berndt and Chen-Nee Chuah and Erica Goude and Lynea B. Kaethler and Amanda Lopez and Alina Nicorici and Corey Owens and David Rodriguez and Jane Wang and Daniel Aranki and Craig M. McDonald and Erik K. Henricson},
      year={2023},
      eprint={2307.04866},
      archivePrefix={arXiv},
      primaryClass={eess.SP}
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
