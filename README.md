<h1 align="center" id="title">CATS-online-anomaly-detection</h1>

<p align="center"><img src="https://socialify.git.ci/SimArgentino/Morphing-attack-detection/image?custom_description=Empirical+evaluation+of+face+recognition+systems%27+vulnerability+to+morphing+attacks+generated+via+traditional+algorithms+and+GANs.&description=1&language=1&name=1&owner=1&theme=Light" alt="Morphing-attack-detection" width="640" height="320" /></p>

<h2>📜 Project Description:</h2>
<p>Morphing Attack is a technique used to generate a facial image that blends features from two different individuals. The resulting image can be authenticated as both people by facial recognition systems, potentially allowing identity fraud.</p>
We believe that morphing attacks represent a serious threat to the security and reliability of biometric systems, especially as generative models become more accessible and realistic. Our work aims to further investigate and validate these concerns through empirical evaluation.

<h2>🧪 Project Goals</h2>

<p>Our main objectives include:</p>

- Generating morphs using both traditional landmark-based and advanced GAN-based methods.
- Evaluating how different pre-trained face recognition networks respond to these attacks.
- Assess the impact of AI-generated faces produced with Midjourney, which at the time of the project (2022) represented a state-of-the-art generative model for realistic human faces
- Compare morphing success rates across multiple architectures and thresholds to identify strengths and weaknesses in current face recognition systems.

<h2>🧰 Morph Generation Models </h2>

To generate morphs, we used different tools depending on the approach. For both traditional and GAN-based morphing, we relied on the models and scripts provided in the official Bob ICASSP 2021 morphing paper implementation from the Idiap Research Institute.

The morphing methods used were:

  - OpenCV:
    Classic morphing using facial landmarks, Delaunay triangulation, and alpha blending.
    Implemented with OpenCV and aligned using preprocessing steps from the Bob pipeline.

  - FaceMorpher:
    A Python tool for smooth morph generation via landmark detection and image blending.

  - StyleGAN2:
    Used through the Bob pipeline to generate interpolated morphs in the latent space of StyleGAN2.

  - MipGAN-II:
    Identity-preserving GAN-based morphs using latent space optimization techniques.
    Integrated via the same Bob framework.

All morphs were generated using the reproducible pipeline from the Bob repository linked above.

Note: Since the original Bob codebase is not natively compatible with Google Colab, where our experiments were conducted, custom modifications were necessary to ensure correct execution (e.g. environment setup, path adjustments, and GPU compatibility). These adjustments are documented in Morphing-attack-detection/morphing/face_morpher.ipynb.

<h2>🧠 Face Recognition Models</h2>

<p>We tested the following popular pre-trained models:</p>

- VGG-Face
- OpenFace
- FaceNet
- FaceNet-512
- ArcFace
- SFace

Each model was evaluated at two thresholds: 0.15 and 0.20.

<h2>🖼️ Dataset and Examples</h2>

The evaluation dataset was entirely constructed for the purposes of this project and includes:

- Portrait photos of students from the Computer Engineering Master’s program at the University of Naples Federico II (ESM 2023)
- Selected celebrity images
- High-quality synthetic images generated via Midjourney, which was a state-of-the-art generative model at the time of the project (2023)

Example morphs:

![ProjectGraph](![Immagine WhatsApp 2025-05-19 ore 13 15 36_a861f31e](https://github.com/user-attachments/assets/34c77f6f-cf8c-4dfa-83eb-b029b8234ffb))


*   Kafka
*   Tensorflow
*   Streamlit
