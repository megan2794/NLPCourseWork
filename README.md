# NLPCourseWork

Code Contributed by Megan Parker and Muhammad Saleem.

# Part 1: Topic Modelling in Python
Python (Gensim) was used to perform Latent Dirichlet Allocation (LDA) on government regulations Hierarchical Dirichlet Process (HDP) was used to determine the optimal number of topics.
# Part 2: Visualizations for Topic Modeling Using Elasticsearch/ELK Stack
Logstash was used to ingest the data from the topics determined in Part 1 and the data is stored in elastic for fast aggregations. Then kibana is used to provide visualizations on the data.

# Part 1 Details:

# Part 2 Details:
Setup - Download version 6.7.0 of Elasticsearch, Logstash, Kibana from https://www.elastic.co/
Files:
1. df_regulations_project_final.csv - This is the data file for the topics (can be replaced with another file if preferred)
2. nlpproject.conf - Logstash configuration file, add this file under the logstash home folder. Ensure you replace the following tag with the correct path for the data file (df_regulations_project_final.csv) path => ["/mnt/c/ELK/df_regulations_project_final*"]
3. export.json - This file can be imported using the Kibana GUI to create the nlp.finalproject-* topic, all visualizations and all dashboards created in this project. The following steps will be needed to import this file: Go to the management tab in Kibana - Saved Objects - Import - Then upload export.json
