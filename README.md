# Machine Learning in Network Intrusion Detection Systems (IDS)

This repository contains the code and findings of our research project investigating the application of machine learning algorithms to network intrusion detection. The project involves setting up a Windows server, generating and collecting network traffic logs, and then applying machine learning techniques for intrusion detection.

## Introduction

Machine learning algorithms have a wide array of applications, one of the most crucial being detecting cyber attacks and malware. Our aim in this project is to investigate different machine-learning algorithms for network intrusion detection and IP traffic filtering.

## Setup & Requirements

### Software Requirements

This project uses Python, and it requires the following Python libraries:

- `numpy`
- `pandas`
- `scikit-learn`

You can install these libraries using pip:

```bash
pip install numpy pandas scikit-learn
```

## Setting Up Windows Server and Collecting Network Logs

This project involves setting up a Windows Server in a VM and generating network traffic for analysis. Here are the steps involved:

1. Install Windows Server on a Virtual Machine.
2. Configure the Windows Server with the necessary roles and features.
3. Setup a network monitoring tool, such as Wireshark, to collect network logs.
4. Generate network traffic and collect logs.

For a detailed guide on setting up a Windows Server and collecting network logs, please refer to [this guide](./Windows_Server_Setup.md).

## Datasets

The datasets used for training and testing the machine learning models include the generated network logs and the NSL-KDD dataset. The NSL-KDD dataset can be downloaded from [this link](https://www.unb.ca/cic/datasets/nsl.html). After downloading, please place it in the same directory as the Python script.

## Methodology

The project compares the performance of J48 Decision Tree and Random Forest machine learning algorithms. Both models are trained using the NSL-KDD dataset and the generated network logs, and then evaluated on the basis of accuracy, Matthews correlation coefficient, precision, recall, and F1-score. We also perform cross-validation and hyperparameter tuning for a more comprehensive evaluation.

## Running the Code

To run the code, navigate to the project directory and run:

```bash
python ml_algorithms_ids.py
```

The output will display the performance metrics for each algorithm and the best parameters found for Random Forest.

## Results

For a detailed analysis and discussion of our results, please refer to our poster presentation, [Machine Learning Algorithms in network intrusion detection system (IDS)](https://www.researchgate.net/publication/359504591_Machine_Learning_Algorithms_in_network_intrusion_detection_system_IDS).

According to the results, the Random Forest Algorithm had higher performance than J48. It had better accuracy, detection rate, lower False Alarm Rate, and better Matthews Correlation Coefficient (MCC), indicating its superiority for binary classifications in this particular use-case.

## Conclusion

Implementing machine learning models for intrusion detection systems and assessing their performance is a valuable step towards advanced cyber defense. However, certain limitations exist, particularly the difficulty of detecting Advanced Persistent Threat (APT) attacks. Future work will focus on improving the detection of such sophisticated threats and optimizing the application of machine learning in cyber security.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

## Acknowledgments

- I would like to thank my advisor, Dr. Dean Hougen, for his guidance and support throughout this project.
- This work was conducted in the Robotics, Evolution, Adaptation, and Learning Laboratory (REAL Lab) at the School of Computer Science, Gallogly College of Engineering, University of Oklahoma.
