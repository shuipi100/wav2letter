# wav2letter++

[![CircleCI](https://circleci.com/gh/facebookresearch/wav2letter.svg?style=svg)](https://circleci.com/gh/facebookresearch/wav2letter)

wav2letter++ is a fast, open source speech processing toolkit from the Speech team at Facebook AI Research built to facilitate research in end-to-end models for speech recognition. It is written entirely in C++ and uses the [ArrayFire](https://github.com/arrayfire/arrayfire) tensor library and the [flashlight](https://github.com/facebookresearch/flashlight) machine learning library for maximum efficiency. Our approach is detailed in this [arXiv paper](https://arxiv.org/abs/1812.07625).

This repository also contains pre-trained models and implementations for various ASR results including:
- [Likhomanenko et al. (2019): Who Needs Words? Lexicon-free Speech Recognition](recipes/models/lexicon_free/README.md)
- [Hannun et al. (2019): Sequence-to-Sequence Speech Recognition with Time-Depth Separable Convolutions](recipes/models/seq2seq_tds/README.md)

The previous iteration of wav2letter (written in Lua) can be found in the [`wav2letter-lua`](https://github.com/facebookresearch/wav2letter/tree/wav2letter-lua) branch.

## Building wav2letter++
See [Building Instructions](docs/installation.md) for details.

## Full documentation
- [Data Preparation](docs/data_prep.md)
- [Training](docs/train.md)
- [Testing / Decoding](docs/decoder.md)

To get started with wav2letter++, checkout the [tutorials](tutorials) section.

We also provide complete recipes for WSJ, Timit and Librispeech and they can be found in [recipes](recipes) folder.

Finally, we provide [Python bindings](bindings/python) for a subset of wav2letter++ (featurization, decoder, and ASG criterion).

## Citation

If you use the code in your paper, then please cite it as:

```
@article{pratap2018w2l,
  author          = {Vineel Pratap, Awni Hannun, Qiantong Xu, Jeff Cai, Jacob Kahn, Gabriel Synnaeve, Vitaliy Liptchinsky, Ronan Collobert},
  title           = {wav2letter++: The Fastest Open-source Speech Recognition System},
  journal         = {CoRR},
  volume          = {abs/1812.07625},
  year            = {2018},
  url             = {https://arxiv.org/abs/1812.07625},
}
```

## Join the wav2letter community
* Facebook page: https://www.facebook.com/groups/717232008481207/
* Google group: https://groups.google.com/forum/#!forum/wav2letter-users
* Contact: vineelkpratap@fb.com, awni@fb.com, qiantong@fb.com, jcai@fb.com, jacobkahn@fb.com, gab@fb.com, vitaliy888@fb.com, locronan@fb.com

See the [CONTRIBUTING](CONTRIBUTING.md) file for how to help out.

## License
wav2letter++ is BSD-licensed, as found in the [LICENSE](LICENSE) file.
