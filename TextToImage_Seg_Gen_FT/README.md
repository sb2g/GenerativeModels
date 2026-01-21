## Overview:
- This repo covers some techniques & concepts on Text to Image generation & Prompting Engineering Vision Models, along with my example notebooks from https://learn.deeplearning.ai/courses/prompt-engineering-for-vision-models/.
- It covers how to perform:
    - Image Segmentation with Pixel-coordinates or Bbox
        - Using 
            - SAM / FastSAM (Segment anything model): Bbox/Pixel-coordinates -> Mask
    - Object Detection & Segmentation with natural language
        - Using
            - OWL-ViT: Text prompt -> Bbox
            - MobileSAM: Bbox -> Mask
    - Image Inpainting
        - Using 
            - Stable Diffusion
                - Original image
                - Image mask (for area to replace)
                - Prompt description on what to inpaint
            - Hyperparameter tuning
                - Guidance scale
                - Strength
                - Negative prompt
    - Fine-tuning diffusion model on a small dataset
        - Using:
            - Dreambooth
                - Instance loss
                - Prior preservation loss
            - Dataset
                - New: Instance image + Prompt (with new token for new object)
                - Old: Class image dataset + Prompt 

# Reference:
1. https://learn.deeplearning.ai/courses/prompt-engineering-for-vision-models/