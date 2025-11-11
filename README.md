---
layout: home
title: Raymond Development areas of interest
permalink: /
---
This site is where Raymond posts his personal solutions, developments, and prototypes of interest. Most of these are things he's developed in his spare time, addressing areas he's felt were missing while working on numerous manufacturing-related projects.

### 📂 AI for Factory Automation
In Semiconductor Industry that produce a wide variety of products in small quantities, quickly achieving yields is crucial. There's a reason most semiconductor and display factories use Oracle Database. It's virtually the only database capable of collecting massive transactions without delay and making real-time decisions.<br>
Because downloading massive amounts of data into an analytics system poses a challenge, it's necessary to immediately draw inferences using AI models already trained in the storage where the data is collected, and then determine lot movement based on those results. This requires an Oracle in-database solution, and for this purpose, we developed the Big Data Analysis Enabler.
#### ✅ Big Data Analysis Enabler (BDAE)
This is a personal project, and was created for multi-purpose use, such as replacing PL/SQL, Function, etc. with Python, R for AI work, etc., in addition to Oracle Database's role as a storage.<br>
The purpose of this is to be able to immediately infer a model using data within the Oracle Database in the fastest way possible without moving data, as it is based on collected Oracle In-Database technology, and then to perform various data transformation tasks easily using Python, etc. and return them like general SQL results.

#### ✅ OPC-UA with Prosys SDK

Semiconductors have EAP, and equipment and EAP communicate based on the SECS/GEM protocol. However, this protocol applies only to semiconductor equipment, while auxiliary equipment such as pumps do not. While communication using different protocols can result in inconsistencies, this is crucial for yield. Therefore, the OPC-UA standard protocol was created to provide these equipment with the necessary tools.<br>

### 📂 New direction and innovation
#### ✅ ROS2
As is widely known, ROS2 (Robot Operating System 2) is an open framework for robots and provides tools and libraries for developing, managing, and deploying robot software.
I recently became interested in this development because I thought it would be very effective to combine this with OPC-UA.

#### ✅ LLM + RAG + LoRA + ...
LLM may seem a bit far from the factory. That's because factories are closed spaces for security reasons, but I don't think LLM itself is unnecessary. However, it requires a unique model and RAG. Furthermore, the data is often tabular, making these aspects somewhat different. We're experimenting with these approaches.


📌 Please Refer to Side Menu for my personal solutions and works.
