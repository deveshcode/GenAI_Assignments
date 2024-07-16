# Latent Diffusion Assignment

This folder contains the assignment on exploring Latent Diffusion Models (LDMs) with CLIP, VAE, and UNet. The objective is to understand the architecture and training process of Latent Diffusion Models, focusing on their components and integration for high-quality image synthesis.

## Files

- **latent-diffusion-devesh.ipynb:** Jupyter Notebook with the complete code and analysis.
- **Latent_Diffusion.pptx:** PowerPoint presentation summarizing the findings.

## What are Latent Diffusion Models (LDMs)?

Latent Diffusion Models operate in the latent space of pre-trained autoencoders to achieve high-quality image synthesis while addressing the computational challenges of traditional Diffusion Probabilistic Models (DPMs).

### Two Phases of Training

1. **Perceptual Image Compression:** Pretrained autoencoders encode images into a latent space.
2. **Latent Diffusion:** Sequential denoising and refining steps in the latent space utilizing cross-attention layers.

## Role of VAEs (Variational Autoencoders)

- **Structure and Function:** Consists of an encoder and decoder. The encoder compresses input images into a latent space, and the decoder reconstructs the original images.
- **Perceptual Compression:** Aims to preserve human perceptually relevant information through a balance in the VAE loss function.
- **Integration with LDMs:** Operates within the reduced-dimensional space created by the VAE.

## No Diffusion without “U”(nets)

- **U-Net Architecture:** A CNN architecture that serves as a core component for denoising in LDMs.
- **Role in LDMs:** Adapts to work with latent representations and incrementally denoises through the diffusion process.
- **Skip Connections:** Preserve context by carrying detailed information directly from the contracting path to the expanding path.

## Enhancing LDMs with CLIP

- **CLIP Integration:** Bridges textual and visual data to generate images that align closely with natural language descriptions.
- **Role in Text-to-Image Synthesis:** Ensures that generated images match textual prompts accurately.
- **Semantic Guidance and Conditioning:** Provides semantic understanding and guides the generation process.

## Latent Diffusion Model Components

1. **Diffusion:** Defines the Latent Diffusion model for text-to-image translation.
2. **Autoencoder (VAE):** Implements an encoder-decoder structure for image and latent space conversion.
3. **CLIP:** Utilizes the CLIP model for converting text prompts into embeddings.
4. **UNet:** Constructs a UNet architecture specifically designed for diffusion tasks.
5. **Prompt to Image:** Initializes a text-to-image class, setting up model and sampling configurations.

## Instructions

1. Open the Jupyter Notebook `latent-diffusion-devesh.ipynb` to view and run the code.
2. Review the PowerPoint presentation `Latent_Diffusion.pptx` for a summary of the assignment.

## Additional Resources

- [High-Resolution Image Synthesis with Latent Diffusion Models](https://arxiv.org/pdf/2112.10752.pdf)
- [Latent Diffusion GitHub Repository](https://github.com/CompVis/latent-diffusion)
- [Stable Diffusion Using Hugging Face](https://towardsdatascience.com/stable-diffusion-using-hugging-face-501d8dbdd8)
- [OpenAI's CLIP Research](https://openai.com/research/clip)
- [Latent Diffusion Models Review Part I](https://sertiscorp.medium.com/latent-diffusion-models-a-review-part-i-d0feacc4906)
- [Annotated Deep Learning Paper Implementations](https://github.com/labmlai/annotated_deep_learning_paper_implementations)

