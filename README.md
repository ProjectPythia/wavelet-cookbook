<img src="thumbnail.png" alt="thumbnail" width="300"/>

# Wavelet Cookbook

[![nightly-build](https://github.com/ProjectPythia/wavelet-cookbook/actions/workflows/nightly-build.yaml/badge.svg)](https://github.com/ProjectPythia/wavelet-cookbook/actions/workflows/nightly-build.yaml)
[![Binder](https://binder.projectpythia.org/badge_logo.svg)](https://binder.projectpythia.org/v2/gh/ProjectPythia/wavelet-cookbook/main?labpath=notebooks)
[![DOI](https://zenodo.org/badge/815311051.svg)](https://zenodo.org/badge/latestdoi/815311051)

This Project Pythia Cookbook covers how to work with wavelets in Python

## Motivation
Wavelets are a powerful tool to analyze time-series data. When data frequencies vary over time, wavelets can be applied to analysis trends and overcome the time/frequency limitations of Fourier Transforms

## Authors

[Cora Schneck](https://github.com/cyschneck)

### Contributors

<a href="https://github.com/ProjectPythia/wavelet-cookbook/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=ProjectPythia/wavelet-cookbook" />
</a>

## Structure

This cookbook is broken into two main sections:

- Foundations
- Example Workflows

### Foundations

- _"Wavelet Basics"_ covers the motivation and background for wavelet analysis by reviewing time-series data and the strengths and weaknesses of other signal analysis tools like Fourier Transform
- _"PyWavelets and Jingle Bells"_: Learn how to use `PyWavelets`, a Python implementation of wavelet analysis, to determine the order of notes in a simple musical piece
- _"Spy Keypad"_: Learn how to use wavelets to undercover the frequency and order of notes in an unknown piece of audio data

### Geoscience Workflows

- _"Atmospheric Data: Nino 3 SST Index"_: Learn how to apply wavelets to real atmospheric and oceanic data to generate a power wavelet scalogram, similar to the 1999 paper ["A Practical Guide to Wavelet Analysis"](https://psl.noaa.gov/people/gilbert.p.compo/Torrence_compo1998.pdf) by Torrence and Compo in Python

## Running the Notebooks

You can either run the notebook using [Binder](https://binder.projectpythia.org/) or on your local machine.

### Running on Binder

The simplest way to interact with a Jupyter Notebook is through
[Binder](https://binder.projectpythia.org/), which enables the execution of a
[Jupyter Book](https://jupyterbook.org) in the cloud. The details of how this works are not
important for now. All you need to know is how to launch a Pythia
Cookbooks chapter via Binder. Simply navigate your mouse to
the top right corner of the book chapter you are viewing and click
on the rocket ship icon, (see figure below), and be sure to select
“launch Binder”. After a moment you should be presented with a
notebook that you can interact with. I.e. you’ll be able to execute
and even change the example programs. You’ll see that the code cells
have no output at first, until you execute them by pressing
{kbd}`Shift`\+{kbd}`Enter`. Complete details on how to interact with
a live Jupyter notebook are described in [Getting Started with
Jupyter](https://foundations.projectpythia.org/foundations/getting-started-jupyter.html).

### Running on Your Own Machine

If you are interested in running this material locally on your computer, you will need to follow this workflow:

1. Clone the `https://github.com/ProjectPythia/wavelet-cookbook` repository:

   ```bash
    git clone https://github.com/ProjectPythia/wavelet-cookbook.git
   ```

1. Move into the `wavelet-cookbook` directory
   ```bash
   cd wavelet-cookbook
   ```
1. Create and activate your conda environment from the `environment.yml` file
   ```bash
   conda env create -f environment.yml
   conda activate cookbook-dev
   ```
1. Move into the `notebooks` directory and start up Jupyterlab
   ```bash
   cd notebooks/
   jupyter lab
   ```
