# Unlocking Nature’s Secrets: How We Taught AI to Identify Iris Flowers!

**BARATAM NIDHISHRI**


Imagine a world where **Artificial Intelligence** helps us solve everyday puzzles, even in nature! Have you ever looked at a beautiful flower and wished you could instantly know its exact species? That’s exactly what I set out to do with this project: build an **Artificial Neural Network (ANN)** to precisely classify unknown Iris flower types using an Artificial Neural Network!

This wasn’t just a coding exercise; it was a captivating journey into the heart of **classification problems** and the incredible power of deep learning.

Explore the code: [Github](https://github.com/nidhibaratam/Predicting-the-species-of-an-unknown-iris-type-flower/blob/main/predicting_the_species_of_an_unknown_iris_type_flower.ipynb) | [GoogleColab](https://colab.research.google.com/gist/nidhibaratam/790f82f4434a3027a0e4403762e437c9/predicting-the-species-of-an-unknown-iris-type-flower.ipynb)

### The “Why”: Becoming Digital Botanists

Why tackle Iris flowers? Because beneath their delicate petals lies a fascinating challenge for AI! The three Iris species — Setosa, Versicolor, and Virginica — share similarities, yet each has unique traits. My mission was to train a model to spot those subtle differences, turning raw data into a brilliant botanical detective. It’s about empowering computers to “see” and categorize the world around us, one flower at a time!

### Our Dataset: The Blossoming Basics

For this floral adventure, I utilized the legendary **Iris dataset**. It’s a perfect starter kit for anyone diving into classification. This dataset holds 150 samples, covering all three Iris species, each described by four vital measurements:

* Sepal Length (cm)
* Sepal Width (cm)
* Petal Length (cm)
* Petal Width (cm)

### Preparing Our Garden: Data Transformation & Visualization

Before our ANN could learn, the data needed a little tender loving care.

* **One-Hot Encoding:** Imagine turning flower names into secret codes the computer understands! We converted species like “Setosa” into a special numerical format (e.g., [1,0,0]) which is ideal for neural networks.
* **Train-Test Split:** To ensure our model was a true expert and not just memorizing, I split our data into training (80%) and testing (20%) sets. Learning from one, proving itself on the other!
* **Feature Scaling:** This was crucial! Our measurements varied in scale. **StandardScaler** acts like a magical equalizer, transforming all features. This ensures every measurement contributes fairly, preventing larger numbers from unfairly dominating the learning process.

The beautiful pair plots, both before and after scaling, clearly illustrated this transformation, showing how our numerical “garden” became perfectly aligned for learning.

### Building Our Botanical Brain: The Keras Blueprint

For this smart botanical brain, I relied on **TensorFlow’s Keras API** — it makes building neural networks feel incredibly intuitive, like snapping LEGO bricks together! My Artificial Neural Network was structured with purpose:

* **Input Layer:** The gateway for our 4 precisely measured flower features.
* **Hidden Layers (8 and 10 neurons):** These are the true “detectives” of our network, sifting through data to learn complex patterns. **ReLU activation functions** gave these layers the spark they needed to process information efficiently.
* **Output Layer (3 neurons):** The grand finale! Three neurons, one for each Iris species. The **Softmax activation** here confidently presented the probabilities, telling us which species was the most likely match.

My model was then “armed” with the **Adam optimizer** (our learning engine) and **categorical_crossentropy** loss function, ready to begin its training.

### The Learning Curve: Training & Validation

I sent our model to “botany school” for **75 epochs** (rounds of intensive learning!). With each epoch, it refined its understanding, steadily boosting its accuracy and minimizing its errors.

The training graphs beautifully showcased this progress: both training and validation accuracy soared, while the loss plummeted. This confirmed our model wasn’t just learning, but genuinely understanding the nuances of the Iris data.

The result? A fantastic **~93% accuracy** on unseen Iris flowers — proving our digital botanist was truly a sharp learner!

### The Reveal: Predicting the Next Bloom!

The most thrilling moment? Putting our model to the test with a completely unknown iris! Imagine providing these measurements:

* Sepal Length: 5.0 cm
* Sepal Width: 2.0 cm
* Petal Length: 1.3 cm
* Petal Width: 0.5 cm

After a quick analysis, our model confidently declared the species: **Versicolor**!

### Our Blooming Insights: What We Mastered

This project wasn’t just about code; it was about truly understanding the mechanics of AI:

* **Classification Power:** Witnessing how ANNs can categorize complex data with high accuracy.
* **Data’s Vital Role:** Grasping the absolute necessity of preprocessing steps like **Feature Scaling** and **One-Hot Encoding**.
* **Model Intelligence:** Learning to train, monitor, and evaluate an ANN to ensure it performs its best.

This experience was a beautiful fusion of nature and technology, revealing the incredible potential of machine learning to bring clarity and insight to our world. I hope it sparks your own curiosity to explore the fascinating realm of AI!
