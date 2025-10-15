---
layout: home
title: Raymond Development areas of interest
permalink: /
---
본 사이트는 Raymond 의 개인 솔루션 및 관심있는 개발 및 프로토타입 등에 대한 것들을 게시하는 사이트입니다.


## ✅<span style="color:#034299"> Big Data Analysis Enabler(BDAE) for Oracle Database

### ✅<span style="color:#034299"> 개요
이것은 개인 작품으로, Oracle Database 를 저장소 역할 이외에 R, Python 를 이용한 AI 작업 등과 PL/SQL, Function 등을 R, Python 으로 대체할 다목적인 용도로 만들어졌습니다. (본 제품은 상용 제품입니다.)<br>

Oracle R Enterprise(ORE) 개념 자체에 큰 영향을 받았지만, 실질적으로 Oracle Database 관련 API 사용한 것을 빼면 전혀 관계는 없습니다.
<br>
BDAE 는 Python, R, JAVA 를 지원하고 R 의 경우 ORE 의 R 과 또 다릅니다.  BDAE 는 오픈소스 R 을, ORE 는 Oracle 자체적인 
많은 수정이 이뤄진 Oracle R 엔진을 사용합니다. <br> 또한 BDAE 는 R 보다 Python 을 권장합니다.  그 이유는 여러분들이 아는 그대로입니다. <br><br>
BDAE 는 ORE 처럼 알고리즘만 수행하는 목적으로 만든 것이 아니라, Oracle PL/SQL 및 Function 의 한계를 Python, R 등의 업무 중심의 언어로 극복하고 데이터의 이동없이 데이터의 변환 및 AI 작업을 SQL 문으로 실행하고 그 결과를 일반적인 SQL Query 로 받기 위한 가벼운 툴을 목표로 개발 했습니다.<br><br>

Oracle In-Database 기술을 사용하기 때문에 일반적이 어플리케이션이 아니며 Shared Library(.so) 형태를 띄고 있고, Oracle Database 가 필요 시 자동으로 실행시켜 주는 형태이며, 개발 관련 예제가 거의 없기 때문에 만드는데 오랜 시간이 걸렸습니다.<br>

구현 및 설치 구성은 Shared Library (C/C++ 기반), Oracle PL/SQL, Function, Type, View 등으로 구성되어 있으며 Embedded SQL 을 위한 별도의 테이블 함수를 제공합니다.<br><br>



### 💡 활용
BDAE 는 단지 AI 업무(ML,DL,..)만을 목적으로 하지 않습니다.  기존 PL/SQL 등을 Python 으로 작성하거나, 백앤드의 여러 번의 DB Call 을 Python, R 등으로 한번으로 처리하는 등의 작업을 손쉽게 합니다.<br>
Big Data Analysis Enabler (BDAE) 는 개발 당시의 배경을 암시합니다.  Oracle Database 나 Exadata 는 Big Data 를 핸들링하는데 부족함은 없습니다.  ROI 도 왠만한 오픈소스 보다 낫습니다. 인건비가 가장 큰 비용이기 때문입니다.<br>
<br>
PL/SQL 문이나 Table 함수를 Python, R 로 작성하여 Dynamic SQL 로 호출하면 개발 생산성이 매우 뛰어나며 유지보수성이 증가합니다.<br>

Anaconda 의 가상화 환경에서 다양한 Python 버전과 패키지들의 구성에 따라 선택적으로 환경을 구성할 수 있습니다.<br>
R 역시 Anaconda 에서 가상화 환경에서 설치가 가능해서 통합적으로 운영될 수 있습니다.<br><br>
자세한 사항은 좌측 메뉴를 참조하시면 됩니다.


## ✅<span style="color:#034299"> OPC-UA with Prosys SDK

이 제품은 개인 제품으로, JAVA 로 구현된 IOT 분야의 국제 프로토콜인 OPC-UA 를 상용 SDK 인 Prosys 사의 JAVA OPC-UA SDK 및 PLC 라이브러리로 만든 OPC-UA Server 입니다. (본 제품은 상용 제품입니다.)<br><br>
Eclipse Milo 프로젝트의 OPC-UA Server SDK 를 가지고 최초 버전을 만들었지만, Alarm & Condition 기능 등이 아직 구현이 안되어 상용 제품(Prosys)을 사용했으며, 또한 다양한 PLC 들에 대한 대응도 역시 상용 제품을 사용했습니다.<br>

OPC-UA Server 를 제공하지 않는 다양한 제조 장비, 부가 장비들을 산업 표준의 OPC-UA 프로토콜을 가능케 하고 Data Access, Historical Data, Event, Alarm & Condition 등의 OPC-UA 의 기본 기능을 충실하게 가능케 합니다. <br><br>

다만 JAVA 기반이므로 많은 Tag 에 대한 Latency 가 있을 수 있으며 이는 GC 때문입니다.<br>
3,000 개 Tag 들의 150ms 미만의 Latency 까지가 최대 Performance 입니다.<br>
물론 이는 ARM 4 core, 4GB 기반에서 였으며 이를 클라우드화 하면 더 좋은 성능을 보일 수 있습니다. <br>

자세한 사항은 좌측 메뉴를 참조하시면 됩니다.


## ✅<span style="color:#034299"> ROS2
널리 알려진 바와 같이 ROS2 (Robot Operating System 2) 는 로봇을 위한 개방형 프레임워크이며 로봇 소프트웨어를 개발, 관리, 배포하기 위한 도구 및 라이브러리를 제공합니다.<br><br>
ROS2 를 전문적으로 하지는 않았습니다만, 그 구성은 그 동안 해 왔던 일들과 무관하지만은 않은 점이 있습니다. <br>
IoT 를 위한 OPC-UA 와 ROS2 Topic 의 Pub/Sub 은 마치 MQTT/OPC-UA 변환 구현과 흡사한 모습을 띄고 있고 호환되어야 할 부분이 있으며 앞의 Big Data Analysis Enabler 의 AI 를 위한 Deep Learning, Machine Learning 의 실시간 추론과도 관련이 없다고 할 수 없습니다.<br><br>

무엇보다 이것을 구현하기 위해서는 C++ 또는 Python 으로 하는 것이므로 개발 맥락이 닿아 있습니다. <br><br>

참고로 실험적인 부분은 좌측 메뉴를 참조하시면 됩니다.<br>

## ✅<span style="color:#034299"> LLM + RAG + LoRA + ...
LLM 은 특별한 산업의 기준정보 프로젝트에서 관심을 가지게 되었습니다. <br>
기존 생산에 사용된 문서에 MES, SPC, RMS 등이 50 여개 공정별 문서로 구분되어 있었으며, 이를 자동화 하는 프로젝트였습니다.<br><br>
통상적으로 기준정보는 메타 데이터가 존재해야 하는데 모두 문서로 되어 있었고 이를 DB 화하는 작업을 했습니다. <br>
그 과정에서 유사도를 기반으로 추천하는 간단한 것부터 시작했고, ChatGPT 등의 LLM 이 활성화 되면서 RAG 를 알게 되었고, 결국 LLM 모델을 파인튜닝하는 것까지 실험적으로 해 보고 있습니다.<br><br>

RAG 를 구현하는데 FastAPI, MCP, Flask, LangChain, LangGraph 등을 해 보고 있으며 문제는 데이터를 기술하는 것에 대한 맥락을 AI 측면에서 생각하지 않으면 안된다는 것을 알게 되었습니다.<br>

파인 튜닝은 Google CoLab 이 아닌 데스크 탑의 GPU (VRAM : 12GB) 를 사용하여 실험적으로 접근하고 있으며, 전문적으로 하지 않기 때문에 하이퍼파라미터들이나 학습 데이터 자체에 대한 고도화를 테스트 하고 있습니다. <br><br>


Please Refer to side menu for my personal solutions.
