# Pytorch Implementation for the Additive Powers of Two Quantization

## Dataset -> MNIST

|   Model   | Precision | Hyper-Params                          | Accuracy |
| :-------: | --------- | ------------------------------------- | -------- |
| ResNet-18 | 5-bit     | batch128_lr0.01_wd0.0001_25epoch      |     |
| ResNet-18 | 4-bit     | batch128_lr0.01_wd0.0001_25epoch      |     |
| ResNet-18 | 3-bit     | batch128_lr0.01_wd0.0001_25epoch      |     |
| ResNet-18 | 2-bit     | batch128_lr0.01_wd0.0001_25epoch      |     |
| ResNet-34 | 5-bit     | batch128_lr0.01_wd0.0001_25epoch      |     |
| ResNet-34 | 4-bit     | batch128_lr0.01_wd0.0001_25epoch      |     |
| ResNet-34 | 3-bit     | batch128_lr0.01_wd0.0001_25epoch      |     |
| ResNet-34 | 2-bit     | batch128_lr0.01_wd0.0001_25epoch      |     |
| ResNet-50 | 5-bit     | batch128_lr0.01_wd0.0001_25epoch      |     |
| ResNet-50 | 4-bit     | batch128_lr0.01_wd0.0001_25epoch      |     |
| ResNet-50 | 3-bit     | batch128_lr0.01_wd0.0001_25epoch      |     |
| ResNet-50 | 2-bit     | batch128_lr0.01_wd0.0001_25epoch      |     |

### Compared with Uniform Quantization

Pass the value `0` to the argument `power` to switch to uniform quantization
Results:

|   Model   | Precision | Hyper-Params                      | Accuracy | Compared with APoT |
| :-------: | --------- | --------------------------------- | -------- | ------------------ |
| ResNet-18 | 5-bit     | batch128_lr0.01_wd0.0001_25epoch  |     |            |
| ResNet-18 | 4-bit     | batch128_lr0.01_wd0.0001_25epoch  |     |            |
| ResNet-18 | 3-bit     | batch128_lr0.01_wd0.0001_25epoch  |     |            |
| ResNet-18 | 2-bit     | batch128_lr0.01_wd0.0001_25epoch  |     |            |
| ResNet-34 | 5-bit     | batch128_lr0.01_wd0.0001_25epoch  |     |            |
| ResNet-34 | 4-bit     | batch128_lr0.01_wd0.0001_25epoch  |     |            |
| ResNet-34 | 3-bit     | batch128_lr0.01_wd0.0001_25epoch  |     |            |
| ResNet-34 | 2-bit     | batch128_lr0.01_wd0.0001_25epoch  |     |            |
| ResNet-50 | 5-bit     | batch128_lr0.01_wd0.0001_25epoch  |     |            |
| ResNet-50 | 4-bit     | batch128_lr0.01_wd0.0001_25epoch  |     |            |
| ResNet-50 | 3-bit     | batch128_lr0.01_wd0.0001_25epoch  |     |            |
| ResNet-50 | 2-bit     | batch128_lr0.01_wd0.0001_25epoch  |     |            |
