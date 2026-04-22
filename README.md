# R-Genie: Reasoning-Guided Generative Image Editing
[![](https://img.shields.io/badge/Project-Page-blue)](https://dongzhang89.github.io/RGenie.github.io/)

## ⭐Introduction
R-Genie addresses the challenges that current image editing methods remain constrained by explicit textual instructions and limited editing operations, lacking deep comprehension of implicit user intentions and contextual reasoning. R-Genie is a reasoning-guided generative image editor, which synergizes the generation power of diffusion models with advanced reasoning capabilities of multimodal large language models. R-Genie incorporates a reasoning-attention mechanism to bridge linguistic understanding with visual synthesis, enabling it to handle intricate editing requests involving abstract user intentions and contextual reasoning relations.
![Figure3](https://github.com/user-attachments/assets/8eda9dd7-0f22-4951-b0ee-51f497777173)


## ⭐Dataset Samples

![Figure2](https://github.com/user-attachments/assets/34e9f165-972c-4ac8-b801-054c576c29a7)

## ⭐Results

![Figure4](https://github.com/user-attachments/assets/ca778024-3d26-457f-82ff-883cf788894b)

## 🔧Requirements
**Download datasets:**

You can download our datasets on [BaiduCloud](https://pan.baidu.com/s/1eN0YdcnxqmxgcrQjzyyw-Q?pwd=pzpz).

-Note that you have to rewrite the dataloader file to adapt the rearranged dataset file structure.

Other components of our model can also be download from huggingface, as follows:
- [Show-o](https://huggingface.co/showlab/show-o)
- [MAGVIT-V2](https://huggingface.co/showlab/magvitv2)
- [Phi-1.5](https://huggingface.co/microsoft/phi-1_5)

## 🔨How to train
```
deepspeed --master_port=24999 training/train_edit.py config=your_train_config_path
```

