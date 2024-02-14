"# Penguin 0.1"

[//]: # ([![License]&#40;https://img.shields.io/badge/license-MIT-blue.svg&#41;]&#40;LICENSE&#41;)
[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
[![Repository Size](https://img.shields.io/github/repo-size/marta-seq/PENGUIN.svg)](https://github.com/marta-seq/PENGUIN)
[![Python Version](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/downloads/)
[![Suggestions Welcome](https://img.shields.io/badge/Suggestions-Welcome-brightgreen.svg)](CONTRIBUTING.md)
[![Release](https://img.shields.io/github/v/release/marta-seq/PENGUIN.svg)](https://github.com/marta-seq/PENGUIN/releases/)

# PENGUIN
============

*PENGUIN* is a platform for the 

This repository contains the files for running PENGUIN and 


General view: 
![plot](figs/penguin_construction.png)
image made with image2go

## Table of Contents
- [Clone the Repository](#clone-the-repository)
- [Requirements](#requirements)
- [Getting started](#getting-started)
- [Credits](#credits)
- [License](#license)
- [Contributing](#contributing)


## Clone the Repository
To clone this repository to your local machine, use the following command:

~~~~~~~~~~~~~
git clone https://github.com/your_username/your_repository.git
~~~~~~~~~~~~~

## Requirements

## Create conda environment

Download the package and create environment or check requirements

if trouble with appeear-ome ti... and imagecodecs install no deps 

After you created the environment, and if you want to use the Jupyter notebooks

activate penguin environment and add the environment kernel to jupyter 
~~~~~~~~~~~~~
~~~~~~~~~~~~~
```bash
python -m ipykernel install --user --name=penguin
```

launch the jupyter and be sure that you are running with the penguin kernel

## Getting started

There are 2 Notebooks available. 
Use check_th_all_ch_per_image if each FOV is a stack of channels.
Use check_th_one_ch_per_image if each FOV is a directory with multiple tiffs inside ( one per each channel)

Open the notebook and click Kernel -> Restart and Run all 
For all channels in a stack it should look like this: 
![plot](figs/all_ch_image.png)

change the path to the location of your data and click 'Change Path' 
You can now change the channels to visualize,
select different percentiles and thresholds. 
Compare images tab gives you the comparison between raw and the clean image with the defined settings
Compare Zoom plots the images using Plotly library that allows for zooming some areas. 
You can change the number of images that are displayed. 

In the case of stacks of channels, your channel names should be in the page tags. Otherwise, the channel names will be
set as index numbers. 
In the case of directory with multiple files, the channel names should be in the file names. 

![plot](figs/all_ch_image_2.png)


Once you have the values for percentile and thresholds defined you can 
save your images by just clicking the save button. 
In case of a file per channel, you can save all the images of the same 
channel at once. 
In case of stacks with multiple channels per FOV, you need to define
the values per each channel in the pop up table and click save (see below). 

![plot](figs/save_table.png)

Saving images will mimick your structure and filenames (and pagetags) in the
saving directory. 


You can also use directly PENGUIN functions. Just check pipeline files. 


## Credits
If you find this repository useful in your research or for educational purposes please refer to:

## License

Developed at the Leiden University Medical Centre, The Netherlands and 
Centre of Biological Engineering, University of Minho, Portugal

Released under the GNU Public License (version 3.0).


[//]: # (.. |License| image:: https://img.shields.io/badge/license-GPL%20v3.0-blue.svg)

[//]: # (   :target: https://opensource.org/licenses/GPL-3.0)

[//]: # (.. |PyPI version| image:: https://badge.fury.io/py/propythia.svg)

[//]: # (   :target: https://badge.fury.io/py/propythia)

[//]: # (.. |RTD version| image:: https://readthedocs.org/projects/propythia/badge/?version=latest&style=plastic)

[//]: # (   :target: https://propythia.readthedocs.io/)
