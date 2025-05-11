<div align="center">

# IIL-CLSF

# Improving Incremental Learning: A Closer Look at the Softmax Function

</div>



We implement our work (IIL-CLSF) on FACIL framework. The implementation of our method (IIL-CLSF) as well as the rest of our configured versions can be found on [IIL-CLSF/src/approach](https://github.com/Zhangjl128/IIL-CLSF/tree/master/src/approach)

# Abatract

In this work, we investigate the limitations of the widely adopted softmax cross-entropy loss in incremental learning scenarios. Specifically, we highlight how the shift-invariant property of this loss function can lead to multiple optimal solutions and imbalanced weights across different tasks, which exacerbates catastrophic forgetting. To address these issues, we propose two key modifications to the objective function: (1) replacing or regularizing the original joint distillation loss with a summation of task-specific distillation losses, and (2) utilizing a shift-sensitive prediction loss function, such as binary cross-entropy loss. Our numerical experiments validate the effectiveness of these modifications, demonstrating improved prediction accuracy and a significant reduction in forgetting.

# Environment

The environment we use is consistent with FACIL. You can refer to FACIC for environment configuration.

# Datasets

- Training datasets
  1. CIFAR-100: 
     CIFAR-100 dataset will be auto-downloaded.
  2. ImageNet-100:
     ImageNet-100 is a subset of ImageNet. ImageNet100 Refer to [ImageNet-100-datasets: ](https://github.com/TerryLoveMl/ImageNet-100-datasets)

# Launching an experiment

## To run the basic code:
```
`python3 -u src/main_incremental.py
```

More options are explained in the [src](https://github.com/Zhangjl128/IIL-CLSF/tree/master/src)

# Results

## Cifar100



<div align=center>
<img src="https://github.com/Zhangjl128/IIL-CLSF/blob/master/pictures/cifar-100.jpg" > 
</div>

## ImageNet-100



<div align=center>
<img src="https://github.com/Zhangjl128/IIL-CLSF/blob/master/pictures/imagenet-100.jpg" > 
</div>

# Acknowledgement

Thanks for the great code base from https://github.com/mmasana/FACIL.



# IIL-CLSD-Improving-Incremental-Learning-A-Closer-Look-at-the-Softmax-Function
