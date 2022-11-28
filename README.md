# Dataset for the ICPE 2023 Data Challenge track

Information about the track:
[https://icpe2023.spec.org/tracks-and-submissions/data-challenge-track/](https://icpe2023.spec.org/tracks-and-submissions/data-challenge-track/)

The dataset contains performance measurements of JMH microbenchmarks from 30 Java open source projects. The list of projects, along with the revision at which the microbenchmarks were executed, can be found in [benchmarks_revision.csv](benchmarks_revision.csv).

The measurements are organized in time series available in the [timeseries](timeseries) folder. Morevover, the raw samples (JMH output) in JSON format can be found on [https://zenodo.org/record/5961018](https://zenodo.org/record/5961018) (~65GB when unpacked).

Questions about the dataset can be asked by opening issues on this repository, or by sendind an e-mail to icpe2023-data-challenge@easychair.org.

## Usage example

In the python script [example_viz.py](example_viz.py) you can find an example of how to read the data and generate a simple plot for a random benchmark in the dataset. The script requires `pandas` and `matplotlib`:
```
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
python example_viz.py
```

---

The dataset was originally created for the paper:

Luca Traini, Vittorio Cortellessa, Daniele Di Pompeo, Michele Tucci  
**Towards effective assessment of steady state performance in Java software: Are we there yet?**  
Empirical Software Engineering (EMSE) - 28, 13 (2023)  
[https://doi.org/10.1007%2Fs10664-022-10247-x](https://doi.org/10.1007%2Fs10664-022-10247-x)  
[https://github.com/SEALABQualityGroup/steady-state](https://github.com/SEALABQualityGroup/steady-state)
