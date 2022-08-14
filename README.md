# KDD22 Tutorial: Data-Centric Epidemic Forecasting 

Survey paper companion: [PDF](https://arxiv.org/abs/2207.09370)

Slides PART 1: [PDF](https://github.com/AdityaLab/kdd-22-epi-tutorial/blob/main/Part1.pdf)

Slides PART 2: [PDF](https://github.com/AdityaLab/kdd-22-epi-tutorial/blob/main/part2.pdf)

Website: [adityalab.cc.gatech.edu/talks/22-kdd-epi-tutorial.html](https://adityalab.cc.gatech.edu/talks/22-kdd-epi-tutorial.html)

## Tutorial abstract

The recent COVID-19 pandemic has brought forth the importance of epidemic forecasting to equip decision makers in multiple domains, ranging from public health to economics. However, forecasting the epidemic progression remains a non-trivial task as the spread of diseases is subject to multiple confounding factors spanning human behavior, pathogen dynamics, weather and environmental conditions, etc. Research interest has been fueled by the increased availability of rich data sources capturing previously unobservable facets of the epidemic spread and initiatives from government public health and funding agencies like forecasting challenges, symposia, and funding calls. This has resulted in a spate of work covering different aspects of epidemic forecasting. In particular, data-centered solutions have shown potential in enhancing our forecasting capabilities by leveraging non-traditional data sources as well as recent innovations in AI and machine learning. 

This tutorial will delve into various data-driven methodological and practical advancements. First, we will enumerate epidemiological datasets and novel data streams that are relevant to epidemic forecasting capturing various factors like symptomatic online surveys, retail and commerce, mobility and genomics data. Next, we discuss methods and modeling paradigms with a focus on the recent data-driven statistical and deep-learning based methods as well as novel class of hybrid models that combine domain knowledge of mechanistic models with the effectiveness and flexibility of statistical approaches. We also discuss experiences and challenges that arise in real-world deployment of these forecasting systems including decision-making informed by forecasts. Finally, we highlight some challenges and open problems found across the forecasting pipeline.

## Tutorial outline

1. **Overview of Epidemic Forecasting.**
We provide a brief introduction and various examples to motivate the impact and importance of epidemic forecasting. Then, we formalize various problems associated with epidemic forecasting including common targets and their temporal and spatial scales. We also discuss some evaluation metrics for each of the tasks and how they are connected with decisions. We will go over a variety of relevant datasets used including traditional clinical surveillance indicators like case rates, recent digital data streams like social media, online surveys as well as novel relatively unexplored sources like wastewater samples and genomics. 
This section will be structured as follows: (1) Task and targets; (2) Datasets; (3) Evaluation.

2. **Mechanistic models.**
We go over the past literature on traditional and recent mechanistic models that encode mechanisms of epidemic spread. Mass-Action compartment models model movement of individuals across compartments via an ODE. We also look at metapopulation models that have more-fine grained modeling of heterogeneity in population and incorporate information such as human behavior and mobility. We finally look at agent-based models that simulate individuals' behaviors and their relations via contact networks. This section will be structured as follows: (1) Mass-action; (2) Metapopulation; (3) Agent-based.

3. **Statistical models.** 
In this part of the tutorial, we discuss the influential and state-of-art statistical and deep learning models that have shown effectiveness and flexibility to leverage a wide variety of data sources including online search queries, text from social media as well as satellite images. We go over various regression approaches starting with linear regression models and discussing complex and hierarchical regression methods. We then focus on leveraging recent advances in deep learning to learn from large datasets with high dimensional feature space and learn rich feature representation and incorporate multimodal data and spatio-temporal structures. We finally discuss traditional and neural-based density estimation models that learn distribution over forecast targets and help deal with quantifying uncertainty. This section will be structured as follows: (1) Regression; (2) Language and vision; (3) Deep learning; (4) Density estimation.

4. **Hybrid models.**
We discuss various paradigms of hybrid models that incorporate expert priors of mechanistic models with flexible learning power of statistical and deep learning approaches. We look at techniques such as data assimilation, learn parameters of mechanistic models using statistical methods, regularizing statistical learning algorithms with mechanistic priors. We also touch upon wisdom of crowds and finally using ensembles of models that typically provide robust results in practice.  This section will be structured as follows: (1) Mechanistic model with statistical components; (2) Priors from mechanistic models inform statistical model; (3) Wisdom of crowds.

5. **Epidemic forecasting in practice.**
We discuss various important collaborative initiatives to further research and practice of epidemic forecasting that are headed by national agencies like CDC and IARPA. We discuss the important challenges encountered during real-time deployment of these models and methodological solutions to these challenges by top-performing models. Finally, look at recent works that try to inculcate decision making with forecasting to aid in better long-term strategic and short-term tactical interventions in face of uncertainty for various applications from public health to supply chain management. This section will be structured as follows: (1) Collaborative initiatives; (2) Real-time Deployment Experiences; (3) Bridging forecasting with decision making.

6. **Closing remarks**

## Bio of presenters

**[Alexander Rodríguez](https://sites.cc.gatech.edu/~acastillo41/)** is a PhD student in the College of Computing at Georgia Tech. He received a M.S. in Data Science from the University of Oklahoma, and a B.S. in Mechatronics Engineering from the National University of Engineering, Peru. His research interests include data science and AI, with emphasis on time-series and real-world networks problems motivated from epidemiology and community resilience. In response to COVID-19, he has been the student lead at his research group in forecasting the progression of the pandemic, and these predictions have been featured in the CDC’s website and FiveThirtyEight.com. His work has led to publications in AAAI, NeurIPS, ICLR, WWW, and BigData and was awarded the 1st place in the Facebook/CMU COVID-19 Challenge and the 2nd place in the C3.ai COVID-19 Grand Challenge. He has also served as organizer/PC chair of multiple symposiums and workshops including BPDM @ KDD 2017 and epiDAMIK @ KDD 2021. The University of Chicago Data Science Institute named him a ‘Rising Star in Data Science’ in 2021.

**[Harshavardhan Kamarthi](https://www.harsha-pk.com)** is PhD student in the College of Computing at Georgia Tech. He received a B.Tech and M.Tech in CSE from Indian Institute of Technology (IIT) - Madras in 2020. His research interests include time-series forecasting, deep probabilistic, generative modelling and deep learning with applications to problems in epidemiology. His work has been published in NeurIPS, ICLR, WWW and AAMAS and was nominated for best student paper award at AAMAS 2020. He also received Alumni Association Award for best Academic performance and Lakshmi Ravi award for the best Masters thesis at IIT Madras. 

**[B. Aditya Prakash](https://www.cc.gatech.edu/~badityap/)** is an Associate Professor in the College of Computing at the Georgia Institute of Technology (“Georgia Tech”). He received a Ph.D. from the Computer Science Department at Carnegie Mellon University in 2012, and a B.Tech (in CS) from the Indian Institute of Technology (IIT) -- Bombay in 2007. He has published one book, more than 80 papers in major venues, holds two U.S. patents and has given several tutorials at leading conferences. His work has also received multiple best-of-conference, best paper and travel awards. His research interests include Data Science, Machine Learning and AI, with emphasis on big-data problems in large real-world networks and time-series, with applications to computational epidemiology/public health, urban computing, security and the Web. He received a Facebook Faculty Award in 2015, was named as one of ‘AI Ten to Watch’ 2017 by IEEE, and received the NSF CAREER award in 2018. His work has been highlighted by several media outlets/popular press e.g. FiveThirtyEight.com and has also been awarded in multiple data science challenges (e.g the CMU/Facebook COVID19 Symptom Challenge). He was a track chair for the AI for COVID track at AAAI 2021, a Proceedings co-chair for SIGKDD 2020, a Demo Chair for ICDM 2015, a Publicity Chair for SIAM SDM 2016, the Tutorial Chair for SDM 2019, and a PC-vice chair for IEEE BigData 2019. He is also a co-organizer for the SDM E-Commerce Analytics workshop 2020/21 (apart from the epiDAMIK series for the first three iterations). He was also the invited lead organizer of the NSF National PREVENT symposium on pandemic prevention and prediction. 

## Cite our work
If you find our work useful, please cite our work:
- Alexander Rodríguez, Harshavardhan Kamarthi, and B. Aditya Prakash. 2022. Epidemic Forecasting with a Data-Centric Lens. In Proceedings of the 28th ACM SIGKDD Conference on Knowledge Discovery and Data Mining (KDD ’22), August 14–18, 2022, Washington, DC, USA. ACM, New York, NY, USA, 2 pages. https://doi.org/10.1145/3534678.3542620

```
@inproceedings{rodriguez2022epidemic,
  title={Epidemic Forecasting with a Data-Centric Lens},
  author={Rodr\'iguez, Alexander and Kamarthi, Harshavardhan and Prakash, B. Aditya},
  booktitle={Proceedings of the 28th ACM SIGKDD Conference on Knowledge Discovery and Data Mining (KDD ’22)},
  year={2022}
}
