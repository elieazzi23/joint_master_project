# JOINT MASTER PROJECT: Multi-Rate Entropy coding for Learned Image Compression

## Project setup

> Download and install anaconda with python>=3.8

> Create a dedicated anaconda environment for the project

> Within the created environment run `pip install -r requirements.txt` to install all the required dependencies

> **Note** I have included a small dataset for debugging/testing the models but we will have a much bigger dataset for training incase we need to do so.

run

`cd learned_image_compression` then
`python run.py`.

If the model starts training then everything is okay upto this point.

> The training outputs and logs are in the `logs/` directory under coded timestamps.

## Elements

### Learned Image Compression

This is the model training sandbox where we will build and evaluate our network components and incrementally build the entropy coding tools.

> I have included a basic implementation of the checkerboard entropy coding technique.

> Your goal is to understand and experiment with the model, see how it works and explore the entropy coding tools that are already included.

> Subsequently, we will work on including the elements that enable multi-bitrate coding with a single model. <Note that in the configuration file, we have a single value for lambda so each model you train now will only work for a single RD point>

**GOAL**

> Train a multi-bitrate model with efficient entropy coding

### BenchMarking

This is the work area for testing and evaluating learned image compression models.

> At the moment we have benchmarking code from [CompressAI](https://github.com/InterDigitalInc/CompressAI) so feel free to visit their github for detailed documentation when you need it.

> It includes access to about 6 pretrained models used in image compression with examples of how to use them.

> Your main objective is to build a standalone access interface for running multiple models simultaneously and evaluating their performance based on a number of quality assessment metrics. Beside the metrics included, you may have to integrate other image quality assessment techniques such as Perceptual loss, VIF and VMAF.

**GOAL**

> Comprehensive image quality assessment for learned image compression models, identifying the limitations of each metric and the level of correlation to human perception.
