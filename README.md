# DIU
---
![image](https://user-images.githubusercontent.com/86638109/142369431-311b9a27-a4cc-401a-96b2-e39be596f434.png)

## 아이템 개요(요약)

#### 개발 목적

1. 일반 소비자가 인테리어 소품 구매시 고민을 줄이기 위함
2. 소비자가 인테리어를 바꾸고자 할 때 시공업체와 소비자간의 원할한 소통을 위함과 상담시간을 단축시키기 위해서
3. 공간에 어울리는 인테리어를 미리 확인할 수 있도록 하기 위해서

- 아이템소개 : 공간에 어울리는 인테리어 소품 배치 및 추천
1. 핵심 기능 : 본인이 주거하고 있는 공간을 인테리어 소품 변경
2. 사용처 : 인테리어 관련 업체, 인테리어를 바꾸고자 하는 일반 소비자 또는 회사
3. 사용자층 : 리모델링 또 새로 인테리어를 하고자 하는 사람들, 인테리어에 관심이 많은 일반 소비자, 거처를 새롭게 옮기게 되신 분들,

→ 사용자층은 범위는 다양함

- 아이템의 차별성 : 특정 기업에 맞춰져있는 가구뿐 아니라 고객이 원하는 아이템을 폭넓게 제공할 수 있다.

 

- 이미지
- 레퍼런스

### 1. 문제인식

- 개발 목적

인테리어 소비자의 수고를 줄여주기 위해

- 관련기술 동향

 제공된 평면도를 검색 → 해당 평면도 기반으로 가구배치

오늘의집 3d가구 시뮬레이터 : [https://ohou.se/3d_intro](https://ohou.se/3d_intro)

어반베이스 : [https://urbanbase.com/](https://urbanbase.com/)

평면도 작성 → 가구배치

플로어 플래너 : [https://floorplanner.com/](https://floorplanner.com/)

플래너 5d : [https://planner5d.com/use](https://planner5d.com/use)

(**Intelligent AUTO Furnishing → 작성한 3d 도면을 사진처럼 출력 / 개발중)**

아키 스케치 : [https://www.archisketch.com/brand-finder](https://www.archisketch.com/brand-finder) (오늘의집 시뮬레이터 소스, 브랜드 추천 기능 / 베타)

시숲 : [https://www.seesoop.com/](https://www.seesoop.com/) (선호하는 인테리어 사진 선택 → ai기반 인테리어 상담서비스)

- 개발아이템의 독창성

이미지 기반 추천?

### 2. 개발 및 연구내용

1. 개발 내용 상세

- 관련 연구 문헌을 통한 연구 및 개발 내용 상세
    - 생성모델링 (노드13번참고)
        - pix2pix : [https://arxiv.org/pdf/1611.07004.pdf](https://arxiv.org/pdf/1611.07004.pdf)
        - CycleGAN :
    - Dall-e : [https://arxiv.org/pdf/2102.12092.pdf](https://arxiv.org/pdf/2102.12092.pdf)(논문리뷰[https://littlefoxdiary.tistory.com/74](https://littlefoxdiary.tistory.com/74))
    - Furnishing Your Room by What You See논문; [https://arxiv.org/pdf/1911.09299.pdf](https://arxiv.org/pdf/1911.09299.pdf)
    - gtp3: [https://littlefoxdiary.tistory.com/44](https://littlefoxdiary.tistory.com/44)
    - [https://greeksharifa.github.io/nlp(natural language processing) / rnns/2020/08/14/OpenAI-GPT-3-Language-Models-are-Few-Shot-Learners/](https://greeksharifa.github.io/nlp(natural%20language%20processing)%20/%20rnns/2020/08/14/OpenAI-GPT-3-Language-Models-are-Few-Shot-Learners/)
    - [https://inforience.net/2021/02/09/clip_visual-model_pre_training/](https://inforience.net/2021/02/09/clip_visual-model_pre_training/)
    - [https://wdprogrammer.tistory.com/50](https://wdprogrammer.tistory.com/50) (object detection)
    - 제로샷
    - 
- 해커톤3에서 이를 바탕으로 수행할 것을 고려하여 전체 개요 및 세부 개발 목차 작성
    - 전체개요
    - 세부개발목차
    

- 미니 해커톤에서 개발 혹은 구현할 모델에 대한 상세 정보

1. 개발목표
- 목표하는 결과에 대한 세부적인 지표를 정량적으로 작성

### 3. 실현 가능성

1. 개발 전략 : 데이터셋 구축 → GAN모델 학습 (방 사진 데이터 학습 후 생성) → 오브젝트 디텍션 → 객체 치환(유사이미지)

1. 해커톤 수행 일정 

[간트차트](https://www.notion.so/1c1418ac47614051aac1490721329dfb)

### 4. 팀 구성

1. 팀장 및 팀원의 역할 분배
    - 팀장 현황 및 역량
    - 필요한 팀원 및 각 역할 상세
    

### 5. Reference

- 데이터셋
    1. 인스타그램 크롤링 데이터
    2. 

- 모델학습
