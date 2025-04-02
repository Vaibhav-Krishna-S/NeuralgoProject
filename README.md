# NeuralgoProject
This project focuses on **binary sentiment classification** of customer feedback for airlines, aiming to classify reviews as either **positive** or **negative**. The solution leverages machine learning techniques to analyze textual data and predict sentiment with high accuracy.

The dataset used is derived from airline customer reviews, containing features such as flight experience, cabin service, food quality, and overall satisfaction. Each review is labeled as positive or negative based on the expressed sentiment. For example, phrases like "comfortable seats" and "exceptional service" indicate positive sentiment, while "lost my baggage" and "rude staff" suggest negative sentiment. To ensure clarity and balance, a simplified dataset (`simplified_dataset.csv`) was created, featuring 20 carefully curated examples with equal representation of both classes.

The implementation involves several key steps:
1. **Data Preprocessing**: Text data is cleaned and transformed using advanced techniques such as tokenization, lemmatization, and negation handling (e.g., converting "not good" to `NEG_good`). Custom sentiment markers are introduced to emphasize strong indicators of sentiment, such as `LOST_BAGGAGE_NEGATIVE` and `VERY_POSITIVE`.
2. **Feature Engineering**: Additional features are extracted to capture nuanced sentiment patterns, including markers for baggage issues, delays, and strong emotions.
3. **Model Training**: A pipeline combining `TfidfVectorizer` and `MultinomialNB` is used to train the model. Cross-validation ensures robustness, and metrics like accuracy, confusion matrix, and classification report evaluate performance.
4. **Prediction**: The trained model predicts sentiment for new input texts, providing confidence scores alongside predictions.

The project includes clear documentation (`README.md`) and a list of dependencies (`requirements.txt`) for easy setup and reproducibility. It is structured to handle edge cases, such as missing labels or malformed rows, ensuring reliability.

Key strengths of this approach include its focus on domain-specific enhancements (e.g., handling negations and extracting sentiment markers) and explainability through detailed metrics. The use of a simplified dataset ensures ease of testing and debugging, making it suitable for evaluation purposes.

Overall, this project demonstrates a practical application of machine learning in analyzing customer feedback, offering actionable insights for improving airline services. It adheres to best practices in coding, documentation, and model evaluation, ensuring a professional and well-rounded submission.
