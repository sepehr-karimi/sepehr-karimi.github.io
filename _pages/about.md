---
permalink: /
title: "Sepehr Karimi Arpanahi"
excerpt: "About Me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

## **About Me**

I recently got my **Master's degree in Computer Engineering** at the [ECE School of the University of Tehran](https://ece.ut.ac.ir/en/ece), Iran. My research interests lie at the **Natural Language Processing (NLP)**, **Social Network Analysis** and **Applied Machine Learning** techniques for solving real-world problem. As a **Research Assistant** at the Social Networks Laboratory, I work under the mentorship of **Dr. Masoud Asadpour** to investigate cutting-edge techniques in predictive modeling and user interaction analysis on social media platforms. This lead to my **Master's thesis**, titled *"Retweet Prediction using Graph Neural Networks and Representation Learning,"* focuses on predicting user interactions, such as retweets, on platforms like X (formerly Twitter). By leveraging **Graph Neural Networks (GNNs)** and **Representation Learning**, my research aims to improve the understanding of content diffusion and user behavior in dynamic, large-scale social networks.

I am also involved in collaborative research projects with **Columbia University** and **Nottingham Trent University**, exploring the use of **Large Language Models (LLMs)** for **clinical decision support** and the **early detection of Alzheimer's Disease**. In these projects, I apply **EEG signal analysis**, **deep learning**, and **multimodal data** to develop predictive models with potential applications in healthcare.


## **Education**
- **M.Sc. in Computer Engineering**, University of Tehran (2021 – 2024)  
- **B.Sc. in Electrical Engineering**, Amirkabir University of Technology - Tehran Polytechnic (2016 – 2021)  

<!-- ---

## **RECENT Research Experience**
- **Research Assistant**, Social Network Laboratory, University of Tehran (October 2021 – Present)  

  - Developing models for interaction prediction on Twitter (X) using **graph-based embeddings** and **textual features**.  
  - Focused on leveraging Graph Attention Networks for network representation learning.  

- **Research Assistant**, Columbia University, USA (January 2024 – Present)  

  - Developing LLM-based pipelines for real-time **clinical decision support** systems.  
  - Researching the optimization of in-context learning for **diagnostic applications**.

- **Research Assistant**, Nottingham Trent University, UK (February 2024 – Present)  

  - Conducting a **systematic review** of deep learning methods applied to EEG data for detecting Alzheimer’s Disease.  
  - Collaborating with multidisciplinary teams for neurodegenerative disease research.  

- **Research Assistant**, Computational Intelligence Laboratory, Amirkabir University (January 2021 – September 2021)  
  - Explored **Deep Reinforcement Learning** (Deep RL) approaches for differential game solutions.   -->


---
## **Recent News**

{% include base_path %}
{% capture written_year %}'None'{% endcapture %}
{% for post in site.blog reversed %}
  {% capture year %}{{ post.date | date: '%Y' }}{% endcapture %}
  {% if year != written_year %}
  
  {% capture written_year %}{{ year }}{% endcapture %}
  {% endif %}
  {% include archive-single.html %}
{% endfor %}



---

## **Professional Experience**
- **Co-Founder and AI Engineer**, SofiaMind Chatbot (September 2023 – Present)  
  - Building an **intelligent chatbot** powered by **LLMs** and Retrieval-Augmented Generation (RAG).  
  - Integrating cutting-edge NLP techniques for real-time customer support.  

- **Data Scientist and Backend Developer**, OptiGrid Pty Ltd (October 2023 – Present)  
  - Developing APIs for data-driven energy optimization.  
  - Performing data analysis to enhance system efficiency.  

---
## ** Recent Publications**
For a complete list of my publications, visit the [Publications](/publications/) section.  
- **Deep Learning Approaches in EEG Analysis for Early Detection of Alzheimer's Disease and Mild Cognitive Impairment: A Mini Systematic Review**  
  Authors: Tahoura Morovati\*, Hamed Vaezi\*, **Sepehr Karimi\***, et al.  
  Published in: International Conference on Applied Intelligence and Informatics (Accepted, 2024).  

<!-- - **Enhancing Alzheimer's Detection with Reasoning-Augmented In-Context Learning**  
  Authors: MohammadJavad Momeni\*, **Sepehr Karimi\***, Dr. Maryam Zolnoori  
  Status: Under preparation.   -->

---


---


Feel free to reach out to me via [email](mailto:sepkarimia@gmail.com) or explore my [GitHub](https://github.com/sepehr-karimi).