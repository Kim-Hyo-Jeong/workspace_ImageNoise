# 🖼️ 이미지에 노이즈 추가로 학습 방지하기

**이 코드는 글레이즈(Glaze)나 나이트쉐이드(Nightshade) 같은 프로그램을 사용하기 어려운 분들을 위해 작성되었습니다.**

그림에 "노이즈"를 추가하여 AI가 학습하기 어렵게 만드는 간단하고 가벼운 도구입니다.

노이즈는 그림에 육안으로는 거의 보이지 않는 작은 변화를 넣어, 그림의 원래 느낌은 유지하면서도 AI의 학습을 방해하는 역할을 합니다.

<br/>

다음과 같은 4가지 노이즈를 제공합니다.

-   **Gaussian 노이즈** : 그림 전체에 미세한 점처럼 고르게 변화를 추가합니다.  
-   **Salt-and-Pepper 노이즈** : 랜덤하게 밝은 점(소금)과 어두운 점(후추)을 추가합니다.  
-   **Correlated 노이즈** : 주변 색과 연관된 더 부드러운 변화를 추가합니다.  
-   **Striped 노이즈** : 수평 또는 수직으로 일정한 간격의 강한 패턴(스트라이프)의 선을 추가합니다.  

Gaussian과 Salt-and-Pepper 노이즈를 섞어서 함께 적용할 수 있는 기능도 제공합니다.

<br/>

노이즈 강도를 직접 조절할 수 있어 원본 느낌을 최대한 유지하거나 더 강한 변화를 줄지 선택할 수 있습니다.

<br/>

이 도구는 컴퓨터 성능이 높지 않아도 작동하므로, 전문 프로그램을 사용하기 어렵거나 사양 제한이 있는 분들에게 적합합니다. Google Colab에서 간단히 실행할 수 있습니다.

---

## 🎯 주요 기능
- **노이즈 유형**  
  - Gaussian 노이즈 : 이미지에 흐릿한 점들을 추가  
  - Salt-and-Pepper 노이즈 : 이미지에 검은 점(후추)과 흰 점(소금)을 추가  
  - Correlated 노이즈 : 이미지에 상관된 노이즈를 추가하여, 픽셀 간에 상관관계를 유지하는 노이즈를 생성  
  - Striped 노이즈 : 수평 또는 수직으로 일정한 간격의 강한 패턴(스트라이프)의 선을 추가  
  - 복합 노이즈 : Gaussian 노이즈와 Salt-and-Pepper 노이즈를 결합하여 두 가지 노이즈의 효과를 동시에 생성  
- **노이즈 강도 조절**  
  - 슬라이드바를 통해 노이즈 강도를 자유롭게 설정 가능
- **결과 확인**  
  - 원본과 노이즈 적용된 이미지들을 비교할 수 있음  
- **저장 및 다운로드**  
  - 원하는 노이즈를 적용한 이미지를 파일로 저장할 수 있음

---

## 📌 결과 미리보기  

노이즈가 적용된 이미지는 다음과 같습니다.  

|원본 이미지|Gaussian 노이즈 이미지|Salt-and-Pepper 노이즈 이미지|
|:---:|:---:|:---:|
|![sample](https://github.com/user-attachments/assets/60f148b9-c6d8-435a-ab44-c09a1de6d6cb)|![Gaussian](https://github.com/user-attachments/assets/030f71b7-5589-4a1e-a419-4837528f0356)|![Salt-and-Pepper](https://github.com/user-attachments/assets/e92e510e-6826-437b-88ea-d5df7c0e70ce)|

|Correlated 노이즈 이미지|Striped 노이즈 이미지|Gaussian + Salt-and-Pepper 노이즈 이미지|
|:---:|:---:|:---:|
|![Correlated](https://github.com/user-attachments/assets/333b390a-99dc-4e2b-aff9-a1104440e042)|![Striped](https://github.com/user-attachments/assets/7d0a2070-2a1f-4fb6-bd67-93b702f21581)|![Gaussian_Salt-and-Pepper](https://github.com/user-attachments/assets/e9cee12b-3988-4cf8-b3d5-f046b07b3dce)|
