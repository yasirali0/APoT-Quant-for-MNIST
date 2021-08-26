# Additive Powers of Two Quantization

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

```
self.weight_quant = weight_quantize_fn(w_bit=self.bit, power=True)
self.act_alq = act_quantization(self.bit, self.act_grid, power=True)
```

Use `power=False` in the above two lines in `QuantConv2d` class in `quant_layer.py` to switch to the uniform quantization, results:

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
