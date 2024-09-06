# Lin-Dit-Per-DiT
Here is a document about image generation models with improved attention mechanism. Diffsuion Transformer is improved mainly based on the attention mechanism of Performer and Linformer.

This project aims to study whether the improved attention mechanism can optimize the diffusion model to generate high-resolution images. Experiments are carried out from two aspects of memory occupancy and image score, and the task of DiT, Lin-DiT and Per-DiT to generate high-resolution images on the DIV2K dataset is explored.

Per-DiT.py:The attention mechanism of the Performer model is utilized. The Performer is an efficient variant of Transformer specifically designed to handle very long sequences of data, The core advantage is the use of a technique called FAVOR+ (Fast Attention Via Orthogonal Random features) to approximate the standard self-attention mechanism, which drastically reduces the computation and memory requirements. In the context of image generation, this approach can be effectively extended to high-resolution images while maintaining a reasonable computational load.

Lin-DiT.py:The Linformer attention mechanism is used. Linformer is another effective Transformer simplification that reduces model complexity and runtime by linearly projecting the dimensions of keys and values in the self-attention mechanism (instead of quadratic dimension scaling).

# Dataset

 DIV2K dataset is a high quality dataset specially designed for image Super-Resolution task. It is widely used in deep learning tasks such as image restoration, enhancement, and generation. The DIV2K dataset contains 1,000 high-resolution images at 2K resolution (that is, 2048x2048 pixels). 
