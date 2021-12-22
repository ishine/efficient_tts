# EfficientTTS
## Unofficial Pytorch implementation of "EfficientTTS: An Efficient and High-Quality Text-to-Speech Architecture"([arXiv](https://arxiv.org/abs/2012.03500)).


## Updates

2020/12/23: [Mandarin Chinese Samples](https://github.com/liusongxiang/efficient_tts/tree/main/egs/DataBaker/checkpoint-330000steps_LJ_vocoder) uploaded. The experiment setting is exactly the same with the LJSpeech example. A complete description of the usage will be soon uploaded.

2020/12/20: Using the HifiGAN finetuned with Tacotron2 GTA mel spectrograms can increase the quality of the generated samples, please see the newly [generated-samples](https://github.com/liusongxiang/efficient_tts/tree/main/egs/lj/checkpoint-320000steps)

## Current status
- [x] Implementation of EFTS-CNN + HifiGAN

## Setup with virtualenv

```
$ cd tools
$ make
# If you want to use distributed training, please run following
# command to install apex.
$ make apex
```

Note: If you want to specify Python version, CUDA version or PyTorch version, please run for example:

```
$ make PYTHON=3.7 CUDA_VERSION=10.1 PYTORCH_VERSION=1.6
```

## Training
Please go to egs/lj folder, and see run.sh for example use.

## Acknowledgement
The code framework is from https://github.com/kan-bayashi/ParallelWaveGAN


