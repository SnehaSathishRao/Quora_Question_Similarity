# Quora_Question_Similarity
Quora is a place to gain and share knowledge—about anything. It’s a platform to ask questions and connect with people who contribute unique insights and quality answers. This empowers people to learn from each other and to better understand the world.  Over 100 million people visit Quora every month, so it's no surprise that many people ask similarly worded questions. Multiple questions with the same intent can cause seekers to spend more time finding the best answer to their question, and make writers feel they need to answer multiple versions of the same question. Quora values canonical questions because they provide a better experience to active seekers and writers, and offer more value to both of these groups in the long term.  
# Problem Statement: 
* Identify which questions asked on Quora are duplicates of questions that have already been asked.   
* This could be useful to instantly provide answers to questions that have already been answered.  
* We are tasked with predicting whether a pair of questions are duplicates or not.
# Business Objectives and constraints  
1. The cost of a mis-classification can be very high.  
2. You would want a probability of a pair of questions to be duplicates so that you can choose any threshold of choice.  
3. No strict latency concerns.  
4. Interpretability is partially important.  
# Data
* Size of Train.csv - 60MB  
* Number of rows in Train.csv = 404,290   
* Size of Train.csv - 60MBTrain.csv contains 5 columns : qid1, qid2, question1, question2, is_duplicate  
  - qid{1, 2}:  The unique ID of each question in the pair  
  - question{1, 2}:  The actual textual contents of the questions.  
  - is_duplicate:  The label that we are trying to predict - whether the two questions are duplicates of each other.  
