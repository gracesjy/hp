---
layout: home
title: Raymond Development areas of interest
permalink: /
---
This site is where Raymond posts his personal solutions, developments, and prototypes of interest. Most of these are things he's developed in his spare time, addressing areas he's felt were missing while working on numerous manufacturing-related projects.

### ✅ AI for Factory Automation
In foundries that produce a wide variety of products in small quantities, quickly achieving yields is crucial. There's a reason most semiconductor and display factories use Oracle Database. It's virtually the only database capable of collecting massive transactions without delay and making real-time decisions.<br>
Because downloading massive amounts of data into an analytics system poses a challenge, it's necessary to immediately draw inferences using AI models already trained in the storage where the data is collected, and then determine lot movement based on those results. This requires an Oracle in-database solution, and for this purpose, we developed the Big Data Analysis Enabler.
#### ✅ Big Data Analysis Enabler (BDAE)
This is a personal project, and was created for multi-purpose use, such as replacing PL/SQL, Function, etc. with Python, R for AI work, etc., in addition to Oracle Database's role as a storage.<br>
The purpose of this is to be able to immediately infer a model using data within the Oracle Database in the fastest way possible without moving data, as it is based on collected Oracle In-Database technology, and then to perform various data transformation tasks easily using Python, etc. and return them like general SQL results.

#### 💡 활용
BDAE 는 단지 AI 업무(ML,DL,..)만을 목적으로 하지 않습니다.  기존 PL/SQL 등을 Python 으로 작성하거나, 백앤드의 여러 번의 DB Call 을 Python, R 등으로 한번으로 처리하는 등의 작업을 손쉽게 합니다.<br>
Big Data Analysis Enabler (BDAE) 는 개발 당시의 배경을 암시합니다.  Oracle Database 나 Exadata 는 Big Data 를 핸들링하는데 부족함은 없습니다.  ROI 도 왠만한 오픈소스 보다 낫습니다. 인건비가 가장 큰 비용이기 때문입니다.<br>
<br>
PL/SQL 문이나 Table 함수를 Python, R 로 작성하여 Dynamic SQL 로 호출하면 개발 생산성이 매우 뛰어나며 유지보수성이 증가합니다.<br>

Anaconda 의 가상화 환경에서 다양한 Python 버전과 패키지들의 구성에 따라 선택적으로 환경을 구성할 수 있습니다.<br>
R 역시 Anaconda 에서 가상화 환경에서 설치가 가능해서 통합적으로 운영될 수 있습니다.<br><br>
자세한 사항은 좌측 메뉴를 참조하시면 됩니다.


### ✅<span style="color:#034299"> OPC-UA with Prosys SDK

이 제품은 개인 제품으로, JAVA 로 구현된 IOT 분야의 국제 프로토콜인 OPC-UA 를 상용 SDK 인 Prosys 사의 JAVA OPC-UA SDK 및 PLC 라이브러리로 만든 OPC-UA Server 입니다. (본 제품은 상용 제품입니다.)<br><br>
Eclipse Milo 프로젝트의 OPC-UA Server SDK 를 가지고 최초 버전을 만들었지만, Alarm & Condition 기능 등이 아직 구현이 안되어 상용 제품(Prosys)을 사용했으며, 또한 다양한 PLC 들에 대한 대응도 역시 상용 제품을 사용했습니다.<br>

OPC-UA Server 를 제공하지 않는 다양한 제조 장비, 부가 장비들을 산업 표준의 OPC-UA 프로토콜을 가능케 하고 Data Access, Historical Data, Event, Alarm & Condition 등의 OPC-UA 의 기본 기능을 충실하게 가능케 합니다. <br><br>

다만 JAVA 기반이므로 많은 Tag 에 대한 Latency 가 있을 수 있으며 이는 GC 때문입니다.<br>
3,000 개 Tag 들의 150ms 미만의 Latency 까지가 최대 Performance 입니다.<br>
물론 이는 ARM 4 core, 4GB 기반에서 였으며 이를 클라우드화 하면 더 좋은 성능을 보일 수 있습니다. <br>

자세한 사항은 좌측 메뉴를 참조하시면 됩니다.


### ✅<span style="color:#034299"> ROS2
널리 알려진 바와 같이 ROS2 (Robot Operating System 2) 는 로봇을 위한 개방형 프레임워크이며 로봇 소프트웨어를 개발, 관리, 배포하기 위한 도구 및 라이브러리를 제공합니다.<br><br>
ROS2 를 전문적으로 하지는 않았습니다만, 그 구성은 그 동안 해 왔던 일들과 무관하지만은 않은 점이 있습니다. <br>
IoT 를 위한 OPC-UA 와 ROS2 Topic 의 Pub/Sub 은 마치 MQTT/OPC-UA 변환 구현과 흡사한 모습을 띄고 있고 호환되어야 할 부분이 있으며 앞의 Big Data Analysis Enabler 의 AI 를 위한 Deep Learning, Machine Learning 의 실시간 추론과도 관련이 없다고 할 수 없습니다.<br><br>

무엇보다 이것을 구현하기 위해서는 C++ 또는 Python 으로 하는 것이므로 개발 맥락이 닿아 있습니다. <br><br>

참고로 실험적인 부분은 좌측 메뉴를 참조하시면 됩니다.<br>

### ✅<span style="color:#034299"> LLM + RAG + LoRA + ...
LLM 은 특별한 산업의 기준정보 프로젝트에서 관심을 가지게 되었습니다. <br>
기존 생산에 사용된 문서에 MES, SPC, RMS 등이 50 여개 공정별 문서로 구분되어 있었으며, 이를 자동화 하는 프로젝트였습니다.<br><br>
통상적으로 기준정보는 메타 데이터가 존재해야 하는데 모두 문서로 되어 있었고 이를 DB 화하는 작업을 했습니다. <br>
그 과정에서 유사도를 기반으로 추천하는 간단한 것부터 시작했고, ChatGPT 등의 LLM 이 활성화 되면서 RAG 를 알게 되었고, 결국 LLM 모델을 파인튜닝하는 것까지 실험적으로 해 보고 있습니다.<br><br>

RAG 를 구현하는데 FastAPI, MCP, Flask, LangChain, LangGraph 등을 해 보고 있으며 문제는 데이터를 기술하는 것에 대한 맥락을 AI 측면에서 생각하지 않으면 안된다는 것을 알게 되었습니다.<br>

파인 튜닝은 Google CoLab 이 아닌 데스크 탑의 GPU (VRAM : 12GB) 를 사용하여 실험적으로 접근하고 있으며, 전문적으로 하지 않기 때문에 하이퍼파라미터들이나 학습 데이터 자체에 대한 고도화를 테스트 하고 있습니다. <br><br>


📌 Please Refer to side menu for my personal solutions.
