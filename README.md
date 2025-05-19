<h1 align="center" id="title">CATS-online-anomaly-detection</h1>

<p align="center"><img src="https://socialify.git.ci/SimArgentino/Morphing-attack-detection/image?custom_description=Empirical+evaluation+of+face+recognition+systems%27+vulnerability+to+morphing+attacks+generated+via+traditional+algorithms+and+GANs.&description=1&language=1&name=1&owner=1&theme=Light" alt="Morphing-attack-detection" width="640" height="320" /></p>

<h2>📜 Project Description:</h2>
Morphing Attack is a technique used to generate a facial image that blends features from two different individuals. The resulting image can be authenticated as both people by facial recognition systems, potentially allowing identity fraud.

<p>This project was inspired by a paper by Venkatesh et al., which explores the vulnerability of face recognition systems to GAN-based morphs compared to traditional methods. https://arxiv.org/abs/2012.05344</p>

We believe that morphing attacks represent a serious threat to the security and reliability of biometric systems, especially as generative models become more accessible and realistic. Our work aims to further investigate and validate these concerns through empirical evaluation.




<h2>🧪 Project Goals</h2>
Our main objectives include:

- Generating morphs using both traditional landmark-based and advanced GAN-based methods.
- Evaluating how different pre-trained face recognition networks respond to these attacks.
- Assess the impact of AI-generated faces produced with Midjourney, which at the time of the project (2022) represented a state-of-the-art generative model for realistic human faces
- Compare morphing success rates across multiple architectures and thresholds to identify strengths and weaknesses in current face recognition systems.



<h2>📊 Project Graph: </h2>
  
  ![ProjectGraph](https://github.com/SimArgentino/CATS-online-anomaly-detection/assets/93777986/617f1036-a83a-4aff-9444-5c033e9b20ea)



<h2>🛠️ Installation Steps:</h2>


<p>1. Install requirements</p>

```
pip install -r ./CATS-online-anomaly-detection/Streamlit_result_visualization/requirements.txt
```

<p>2. Run the streamlit app</p>

```
streamlit run ./CATS-online-anomaly-detection/Streamlit_result_visualization/app.py
```

<h2>🫵 Build your model </h2>
You can swap the model by changing the model section in the notebook.
After you save the model, move it in the following path:    

```
CATS-online-anomaly-detection/Streamlit_result_visualization/models/
```

<h2>💻 Built with</h2>

Technologies used in the project:

*   Kafka
*   Tensorflow
*   Streamlit
