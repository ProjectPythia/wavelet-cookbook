<img src="thumbnail.png" alt="thumbnail" width="300"/>

# Wavelet Cookbook

[![nightly-build](https://github.com/ProjectPythia/cookbook-template/actions/workflows/nightly-build.yaml/badge.svg)](https://github.com/ProjectPythia/cookbook-template/actions/workflows/nightly-build.yaml)
[![Binder](https://binder.projectpythia.org/badge_logo.svg)](https://binder.projectpythia.org/v2/gh/ProjectPythia/cookbook-template/main?labpath=notebooks)
[![DOI](https://zenodo.org/badge/475509405.svg)](https://zenodo.org/badge/latestdoi/475509405)

This Project Pythia Cookbook covers working with wavelets in Python

## Motivation
Wavelets are a powerful tool to analysis time-series data. When data frequencies vary over time, wavelets can be applied to analysis trends and overcome the time vs. frequency limitations of Fourier Transforms

## Authors

[Cora Schneck](https://github.com/cyschneck)

### Contributors

<a href="https://github.com/ProjectPythia/wavelet-cookbook/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=ProjectPythia/wavelet-cookbook" />
</a>

## Structure

This cookbook is broken into two main sections:

- Foundations
- Example Workflow

### Foundations

"Wavelet Basics" covers the motivation and background for wavelet analysis by review time-series data and the strengths and weaknesses of Fourier transform

### Example Workflows

- "PyWavelets and Jingle Bells": Learn how to use `PyWavelets`, a Python implementation of wavelet analysis, to determine the order of notes in a simple musical piece
- "Spy Keypad": Learn how to use wavelets to undercover the frequency and order of notes in an unkonwn piece of audio data
- "Atmospheric Data: nino3": Replicate the power wavelet scalogram from the original 1999 Torrence and Compo paper in Python

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

(Replace "cookbook-example" with the title of your cookbooks)

1. Clone the `https://github.com/ProjectPythia/cookbook-example` repository:

   ```bash
    git clone https://github.com/ProjectPythia/cookbook-example.git
   ```

1. Move into the `cookbook-example` directory
   ```bash
   cd cookbook-example
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
