## Enhanced Defect Segmentation in X-ray Images of Copper Pipe Welds via Multi-scale Representation and Kolmogorov-Arnold Networks
This is the implementation of our paper "Enhanced Defect Segmentation in X-ray Images of Copper Pipe Welds via Multi-scale Representation and Kolmogorov-Arnold Networks"

<p align="middle">
    <img src="images/Fig.1.png">
</p>

## Usage

### 1. Datesets

Use the [preprocessed data](https://drive.google.com/drive/my-drive?dmr=1&ec=wgc-drive-hero-goto) for research purposes.

### 2. Environment

Please prepare an environment with python=3.9, and then use the command "pip install -r requirements.txt" for the dependencies.

### 3. Train/Test

- Run the train script on synapse dataset. The batch size can be reduced to 12 or 6 to save memory (please also decrease the base_lr linearly), and both can reach similar performance.

```bash
CUDA_VISIBLE_DEVICES=0 python train.py
```

- Run the test script on synapse dataset. It supports testing for both 2D images and 3D volumes.

```bash
python test.py
```
## Reference
* [TransUNet](https://github.com/Beckschen/TransUNet)
* [Kolmogorov-arnold networks](https://github.com/KindXiaoming/pykan)
* [segmentation_models.pytorch](https://github.com/qubvel/segmentation_models.pytorch)
