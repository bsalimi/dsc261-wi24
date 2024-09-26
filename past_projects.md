# DSC 261 Winter 24 Projects

## Causality

### Causal Discovery for Aerosol-Cloud Interactions
This study aims to use purely data-driven causal discovery algorithms to assess
and compare physics-based causal links in the field of climate science. Our dataset
involves various measured and latent, non-linear and non-gaussian variables related
to aerosol-cloud interactions. Our objective is to investigate unaccounted-for links
that were previously unidentified and assess domain assumed links that may not be
detected when applying causal discovery techniques to the raw dataset. Further-
more, we seek to delineate the discoverable aspects and identify the limitations
inherent in these causal discovery algorithms with simulated data with a known
ground truth. We use four different causal discovery algorithms that use differ-
ent methodologies for causal discovery including structural equation based, deep
learning based, conditional independence based, and score based methods. This
exploration may lead to potential modifications and enhancements to better tailor
these algorithms for non-linear, noisy datasets commonly encountered in climate
datasets, as well as prove to be useful for further in-depth analysis in this field.



## Explainability

### Exploring Double Descent Phenomenon in Neural Networks using LIME on MNIST Dataset
This project delves into the intriguing phenomenon of double descent in machine
learning, specifically within neural networks, utilizing the MNIST dataset. We aim
to investigate how these factors influence model performance by manipulating both
data points and model complexity. Employing SHAP, LIME and Saliency Maps
as our analytical tools, we elucidate the interpretability and reliability of neural
networks at various points along the double descent curve. Our hypothesis suggests
that when the number of parameters (d) is close to the feature vector size (n), the
performance reduces due to overfitting. By examining model explanations, we
want to determine and explore whether the predictions are meaningful or driven
by spurious correlations at various points of the double descent. We also want
to look at various different analytical tools and compare them qualitatively. This
project aims to provide insights into the relationship between model complexity
and generalization, with potential implications for developing more interpretable
and reliable neural networks in real-world applications.

### Explainability of Multimodal Models
In the era of artificial intelligence, multimodal models have emerged as a pivotal technology for interpreting complex data across various domains, including
healthcare, autonomous navigation, and content recommendation. These models
process and analyze multiple forms of data—text, images, audio, and video to
make predictions or decisions. Despite their vast potential, a significant challenge
persists: the explainability of these models. Our project addresses this challenge
by enhancing the transparency and understandability of multimodal models. We
suggest an approach that integrates both tabular and textual data in a unified multi-
modal framework, leveraging a custom masking strategy for explainability. This
technique not only provides deeper insights into how different data modalities
influence model predictions but also overcomes the limitations of current state-of-
the-art explainability methods, which often focus on single modalities.

###  Interpretability of Deep Neural Network Decisions in the Audio Domain
Inspired by the work of Becker et al[ 2], this project aims to enhance the inter-
pretability of deep neural network decisions in the audio domain. Despite the high
accuracy of deep learning models in audio classification, their "black box" nature
poses significant challenges in understanding their decision-making processes. This
is particularly problematic in critical applications where trust and transparency are
paramount. We leverage Layer-wise Relevance Propagation technique to identify
significant features by two deep neural networks, namely AlexNet and AudioNet
that process audio data in the forms of Spectrograms and Waveforms, respectively.
We apply these models for three tasks: Sex, Digit Spoken and Accent classification
on the AudioMNIST dataset. Along with traditional visual explanations, we have
explored audible explanations using audible heatmaps. We assessed the effective-
ness of LRP using systematic input data perturbation. By introducing audible
explanations and comparing them with traditional visual explanations, we aim to
significantly improve the interpretability of audio classification models, making
their decisions more accessible and trustworthy to humans.

### Analyzing and Calibrating Learning Preference of Relation Extraction Models Using Adversarial Attack and Counterfactual Analysis
There have been significant advancements in relation extraction (RE) that have
resulted in impressive benchmark accuracy. However, there is still significantly
more to be explored when it comes to understanding the learning preferences in RE.
In this work, we start by discussing the use of adversarial attacks to explore the
model’s learning preference and robustness. Following this analysis, we implement
a different counterfactual calibration method to adjust the prediction results of the
RE model during testing thus reducing the over-dependency issue. This involves
calculating the counterfactual prediction results by excluding the component that
the model heavily relies on. Extensive experiments in multiple datasets indicate
the necessity of introducing tuning-based methods in RE to further address the
over-dependency issue.

### A Comparative Analysis of Interpretability of Models for Sentiment Analysis
Sentiment analysis, a critical task in Natural Language Processing (NLP), is em-
ployed to classify tweets related to stocks by their positive or negative sentiments.
While deep learning-based models, particularly BERT, achieve high accuracy in
this domain, their inherent black-box nature hinders the understanding of how
sentiment classification is performed. In this study, we apply BERT-based models
to a dataset of stock-related tweets and explore their interpretability using Local
Interpretable Model-agnostic Explanation (LIME) and SHapley Additive exPlana-
tions (SHAP). By analyzing the attention weights and feature importance scores,
we aim to shed light on the decision-making process of BERT models, especially in
financial sentiment analysis. Additionally, we compare the performance of BERT
with rule-based models such as Logistic Regression and Naive Bayes which offers
transparency but sacrifice accuracy.

### Counterfactual Explanation Algorithms for Behavioral and Textual Data
This project aims to develop advanced counterfactual explanation algorithms for
behavioral and text data to enhance the transparency and accountability of AI
systems, addressing the growing need for understandable AI decisions in critical
sectors such as healthcare, finance, and human resources. This endeavor is pivotal
as it directly responds to the challenge of making complex AI models explainable
to non-expert users, thereby fostering trust and facilitating ethical AI practices.
The task is inherently difficult due to the complexity of underlying AI models, the
nuanced nature of behavioral and text data, and the challenge of generating explana-
tions that are both accurate and easily comprehensible to humans. Existing methods
often struggle to balance these aspects, particularly in providing actionable insights
that are directly relevant to the users’ context. To overcome these challenges, our
approach integrates cutting-edge techniques in natural language processing, causal
inference, and optimization to create more precise, context-aware counterfactual
explanations. By refining and extending current methodologies, the project aims to
offer novel contributions that not only improve the clarity and relevance of expla-
nations but also enhance the ability of AI systems to be scrutinized and improved,
ensuring that they align more closely with human values and regulatory standards.

### Relational Deep Learning and Explainability of Graph Neural Networks
Predictive problems across various domains involve decision-making processes
that rely on machine learning models built from relational data spread across mul-
tiple tables. However, constructing machine learning models faces challenges in
operating seamlessly across these relational structures, often requiring laborious
manual processes of data joining and aggregation. To address these limitations, a
Relational Deep Learning approach directly learns from data spread across multiple
tables in data warehouses by viewing them as a heterogeneous graph. This transfor-
mation serves as the basis for developing Graph Neural Network (GNN) predictive
models. Given the inherent complexity of GNNs, the integration of explainability
models becomes crucial, providing transparent insights into their decision-making
processes. This project underscores the pivotal role of explainability in enhancing
trust, identifying errors, and facilitating continuous improvement, ensuring that
GNNs are not only accurate but also interpretable for real-world applications and
regulatory compliance. Here, we will construct a GNN on the heterogeneous graph
for a regression task and explain the predictions made by the model by attributing
the prediction to its input features using four attribution methods namely Integrated
Gradients, Saliency, Deconvolution, and Guided Backpropagation.

### Counterfactual Explainable Recommendation using LLMs
Recommendation systems have become an integral part of various online platforms,
enhancing user experience by providing personalized content. However, there is
a growing need for more transparent and interpret able recommendation systems
to address user trust issues. This project focuses on counterfactual reasoning
for explainable recommendation. The design of evaluation metrics is from two
viewpoints: 1) user’s perspective and 2) model’s perspective. In this project we will
experiment with different Large Language Models (LLMs) both open source and
proprietary(till no cost limit) like GPT3.5, Llama2, Mistral to extract aspects and
sentiments, and further compare it with the approach used by the paper (Sentires).

### Unfooling LIME and SHAP
In response to the widespread integration of machine learning models in sensitive
domains, our project addresses the need for interpretability in machine learning
models. Leveraging post-hoc model-independent explanation techniques like
LIME and SHAP, we aim to address the demonstrated vulnerability of these
methods to deception, which effectively conceals inherent biases. If left
unaddressed, these biases could erode trust in machine learning models, potentially
resulting in misguided decisions with significant consequences. In this project,
we explore the initial idea behind fooling LIME and SHAP, analyze existing
techniques that are being used to counter it. We also propose using CT-GAN as a
data generating technique to augment current methods of "Unfooling".

## Privacy

### Enabling LLMs To Generate Text With Citation On Private Data
This research project introduces a novel Large Language Model (LLM) framework
designed to operate on locally stored user data, enabling personalized information
retrieval and question-answering with direct citations from the user’s own datasets.
Unlike traditional cloud-based LLMs, our approach ensures data privacy and rele-
vance by processing information directly on the user’s device, mitigating concerns
related to data security and internet dependency. By harnessing the capabilities
of advanced natural language processing and machine learning algorithms, the
proposed LLM dynamically generates accurate, contextually relevant responses
with citations, enhancing the reliability and traceability of information. This local
execution model not only addresses the challenge of hallucination in text generation
but also significantly improves the utility of LLMs for users with specialized data
needs or those working in privacy-sensitive environments. The outcome of this
research paves the way for a new generation of LLM applications, where data
sovereignty and personalized knowledge extraction are paramount.

## Data Cleaning and Debiasing

### Automated data debiasing pipeline for unstructured textual data
This project aims to compare automated debiasing pipelines and qualitative debias-
ing approaches for unstructured textual data, focusing on hate speech detection in
online platforms. The challenge lies in the complexity of debiasing, particularly in
handling linguistic variations and dialects, such as African American Vernacular
English (AAVE), which are often misrepresented or mislabeled in training data,
leading to biased outcomes. By leveraging novel debiasing techniques informed by
subgroup linguistic characteristics, and using diverse data sources like Twitter and
specialized datasets for underrepresented dialects, we plan to enhance the accuracy
and fairness of hate speech detection systems. This contribution addresses the
pressing need for adaptable and ethical debiasing methods that can keep pace with
the evolving landscape of online discourse.

### FairTrain: FAIRness-aware Data Processing and TRAINing
In this project, we propose different methodologies to integrate fairness metrics
into machine learning pipelines, addressing the challenge of biased data. This
is crucial as data-driven decisions increasingly impact society and making this
integration is challenging due to the complex nature of fairness in data. The
methodology involves directly integrating fairness constraints into the existing data-
cleaning/ model-training frameworks like AutoML, AlphaClean and XGBoost. The
experiments validate this approach on biased datasets like UCI Statlog (German
Credit) and UCI Adult, aiming to balance data quality and fairness, contributing
significantly to responsible AI development.

### Advancing Data Integrity and Fairness: Cleaning for Enhanced ML Accuracy
In this project, we explore how to improve machine learning (ML) models by
cleaning and filling in missing data using different methods: mean, KNN, iterative
imputation, and an advanced tool called AlphaClean. We want to see which
method works best because good data quality is key to making accurate and fair
predictions with ML. This challenge is tricky because every dataset has its own
unique problems, and there’s no one-size-fits-all solution for fixing errors or filling
gaps in the data. Our approach tests these methods by deliberately adding errors
to our data, then cleaning it up and seeing how well the ML models perform
afterward. We found out that while all methods have their strengths, understanding
your specific data’s needs is most important. Our work helps show which data
preparation methods might be best for different kinds of datasets, making it easier
for people working with ML to get reliable and fair results from their models.

