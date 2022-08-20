## Workshop on Deep Learning (develop to deploy for starters)

### Optimization:

__Post training quantization :__

_Improve latency, reduce model size with a little degradation in model accuracy_

![](/home/kingeng/Desktop/codes/myGit_DLCourse/001-mosquito_develop_deploy/images/optimization_mehtods.png)

* __Dynamic Range Quantization:__
  * _Simplest form (90% of cases)_
  * _Quantize only the weights from floating point to integer (8-bit)_
  * _Inference :_ weights converted from $8$-bit to float (done once and cached to reduce latency)
    * perform computations with $8$-bit weights and activations.
