This final project was undertaken as part of my undergraduate studies in Digital Medical technologies at HIT College in Holon, Israel.

The objective of this project was to develop a machine-learning algorithm that serves as the foundation for creating a decision support system tailored for radiologists. The system is designed to leverage patient information and will be implemented within Change HealthCare, a technology health company based in the USA.

Currently, the process of prioritizing the interpretation of patient examinations is done manually by radiologists, relying on a score known as "urgency". This score is determined based on a set of rules that vary among Change HealthCare's different clients. However, this manual process carries inherent risks, necessitating the need for optimization and automation.

The initial goals of this project were to create a system that benefits the patient, improves the quality of treatment provided, and enhances the workflow of radiologists. These goals were pursued through the development of a machine-learning model capable of automatically prioritizing patient examinations. The model uses input parameters to define urgency and returns the corresponding urgency score as output.

To meet the requirements set by the company, the developed model emphasizes explainability, ensuring that it does not operate as a "black box" and can provide insights into its results.

The project's deliverables include four models for predicting the urgency score, which can be implemented by the company across its various clients. Additionally, an algorithm for generating artificial data and a hierarchical model for grouping data based on common characteristics were developed.
The algorithms were implemented using Python and are shared as part of this project.

The order of the files is: 
(1) Data_Generation- due to limited access to actual data, we employed a synthetic data generation approach using probabilities and values provided by the company to simulate realistic data in the absence of direct data access.
(2) Atlantic&Avera- data preparation and exploration of data we received.
(3) Hierarchical_Model- data preparation for a hierarchical model intended to cluster patient samples based on shared characteristics. The aim of this is to uncover patterns and similarities without depending on predefined rules that typically serve as ground truth for predictive models, since such rules were not consistently available.
(4) Models- development of regression and classification models to predict the urgency score of patient samples.
