This project explores the use of Generative Adversarial Networks (GANs) to generate realistic images of pistachios. The main objective was to experiment with different model setups (baseline vs. modified) and evaluate their performance in producing high-quality synthetic images. GANs are powerful deep learning models capable of learning data distributions and generating new, synthetic samples. In this project, we trained GANs on a dataset of pistachio images to learn their visual characteristics such as shape, texture, and color.

Two model variations were implemented:
1. Baseline GAN (fully standard architecture)
2. Modified GAN (improved with architectural and training adjustments, followed by fine-tuning)

The models were compared using the Fréchet Inception Distance (FID), which measures how close the generated images are to real ones.

Methodology
1. Dataset Preparation: pistachio image dataset was preprocessed (resized, normalized).
2. Model Development
   - Baseline GAN: Standard generator and discriminator architectures.
   - Modified GAN: Adjusted architecture and hyperparameters for better stability and image quality.
   - Fine-tuning was performed on the modified GAN, though results showed the original modified version already performed best.
3. Training & Evaluation:
  - Models trained with Adam optimizer and tuned hyperparameters.
  - Generated images compared visually and quantitatively using FID scores.
  - Best-performing model: Modified GAN, achieving an FID score of 147.40.

Key Findings
1. The baseline model could generate images but suffered from lower quality and instability.
2. The modified model significantly improved performance and stability.
3. Fine-tuning did not improve results beyond the original modified architecture.
4. The final modified model achieved the lowest FID score (147.40), making it the most effective in producing realistic pistachio images.
