
# Full Data Set
The code in this directory is used when using the entire data set for the selected county. 

## Installation and Running
The code in this repository was developed for Python 3.5 and above. To install dependency
packages, run the following. 

```bash
pip install -r requirements.txt
```


For the most up-to-date forecasting employing SIRNet, run the script `scripts/forecast.py` after
installation. Parameters within can be modified for different counties, states, countries, etc.
The changes are made in the forecast.py script on lines 454-456.


Example usage:

```bash
./forecast.py --country "United States" --state "Texas" --county "Bexar County"
```

For help on all command line options:

```bash
./forecast.py --help
```

## Forecasting the Reach of the COVID-19 Disease
We use the worldwide daily case, mobility, hospital, population, and other data factors
to forecast the number of cases. One model is a hybrid Susceptible-Infected-Recovered (SIR)
& deep learning architecture and the other is a custom Long Short-Term Memory (LSTM)
architecture. The code can be run from the scripts in the `scripts` directory.

## Citation
This work is based on the work in the preprint referenced below.

_N Soures, D Chambers, Z Carmichael, A Daram, DP Shah, K Clark, L Potter, and D Kudithipudi.
"SIRNet: Understanding Social Distancing Measures with Hybrid Neural Network Model for COVID-19
Infectious Spread." Proceedings of the International Joint Conference on Artificial Intelligence,
(IJCAI), Disease Computational Modeling Workshop (2020)_ -
[arxiv.org/abs/2004.10376](https://arxiv.org/abs/2004.10376)

