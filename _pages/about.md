---
permalink: /
title: "Sepehr Karimi"
excerpt: "About Me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

## **About Me**

I am a **Machine Learning and AI researcher** currently pursuing my **PhD in Electrical and Electronic Engineering** at the **University of Adelaide**, Australia, under the supervision of **Dr. Ali Pourmousavi Kani**. My research focuses on developing **unified, data-driven frameworks** for **electricity price forecasting** and **battery energy storage system (BESS) operation** in the **Australian National Electricity Market (NEM)**.

Before starting my PhD, I completed my **Master’s degree in Computer Engineering** at the University of Tehran. My background spans **Deep Learning**, **Reinforcement Learning**, **Natural Language Processing**, and **Social Network Analysis**. As a researcher at the **NLP Lab**, I contributed to several projects involving **domain-specific question answering**, **LLM-based conversational agents**, and **multilingual chatbot systems** for low-resource languages.

I have also collaborated with research groups at **Columbia University** and **Nottingham Trent University** on projects involving **clinical NLP**, **EEG-based disease detection**, and **multimodal deep learning**, resulting in multiple publications in applied machine learning and healthcare.

My broader research interests include:

- price forecasting & energy market analytics  
- Time-series modeling and decision-making under uncertainty  
- NLP and multimodal deep learning  

I aim to bridge **machine learning**, **optimization**, and **real-world energy systems** to enable more efficient, reliable, and sustainable grid operations.

---

## **Education**
- **Ph.D. in Electrical and Electronic Engineering**, University of Adelaide (2024 – Present)  
- **M.Sc. in Computer Engineering**, University of Tehran (2021 – 2024)  
- **B.Sc. in Electrical Engineering**, Amirkabir University of Technology – Tehran Polytechnic (2016 – 2021)  

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

- **Data Scientist & Backend Engineer**, OptiGrid Pty Ltd (October 2023 – Present)  
  - Building machine learning pipelines for **electricity price forecasting**, **energy optimization**, and **battery bidding strategies**.  
  - Developing backend systems and APIs for scalable, data-driven energy analytics.  

- **Co-Founder & AI Engineer**, SofiaMind (September 2023 – Present)  
  - Developing **LLM-powered chatbots** and **RAG-based** conversational systems.  
  - Focused on multilingual and domain-specific dialogue models.  

---
## **Selected Publications**
For a complete list, visit the [Publications](/publications/) page.

- **Speech-Based Cognitive Screening: A Systematic Evaluation of LLM Adaptation Strategies**  
  Fatemeh Taherinezhad, Mohamad Javad Momeni Nezhad, **Sepehr Karimi**, Sina Rashidi, Ali Zolnouri, Maryam Dadkhah, Yasaman Haghbin, Hossein AzadMaleki, Maryam Zolnoori  
  *arXiv preprint arXiv:2509.03525*, 2025.  
  🔗 https://arxiv.org/abs/2509.03525

- **PersianMedQA: Language-Centric Evaluation of LLMs in the Persian Medical Domain**  
  Mohammad Javad Ranjbar Kalahroodi, Amirhossein Sheikholselami, **Sepehr Karimi**, Sepideh Ranjbar Kalahroodi, Heshaam Faili, Azadeh Shakery  
  *arXiv preprint arXiv:2506.00250*, 2025.  
  🔗 https://arxiv.org/abs/2506.00250

- **Deep Learning Approaches in EEG Analysis for Early Detection of Alzheimer’s Disease and Mild Cognitive Impairment: A Mini Systematic Review**  
  Tahoura Morovati, Hamed Vaezi, **Sepehr Karimi**, Md Mahmud, Michael Crook-Rumsey, Nicky Heym, et al.  
  *International Conference on Applied Intelligence and Informatics*, pp. 63–81, 2024.    
  🔗 https://link.springer.com/chapter/10.1007/978-3-032-04657-4_5

---

## **Contact**
Feel free to reach out via [email](mailto:sepkarimia@gmail.com) or explore my work on [GitHub](https://github.com/sepehr-karimi).

