# AI 개발자를 위한 머신러닝·딥러닝 기초

> 파이썬 카페 키오스크에 쌓인 1년 치 주문 데이터로, 판매량 예측부터 이미지 인식과 말로 주문받기까지 직접 만들어 봅니다.

「AI 개발자를 위한 파이썬 기초」에서 만든 무인 키오스크를 이어서 똑똑하게 만드는 강좌의 실습 노트입니다. 파이썬이 처음이라면 [PythonClass](../PythonClass) 폴더의 강의를 먼저 보세요.

## 사용 방법

1. 아래 표에서 <b>Open in Colab</b> 배지를 누르면 Colab에서 바로 열립니다. 설치할 것은 없어요.
2. 열리면 먼저 <b>[파일] → [Drive에 사본 저장]</b>을 누르세요. 그래야 수정한 내용이 내 드라이브에 저장됩니다.
3. 딥러닝 실습(4강~)은 <b>[런타임] → [런타임 유형 변경] → T4 GPU</b>를 켜고 시작하세요. 방법은 1강에서 안내합니다.
4. <b>실습 노트</b>는 영상을 보며 직접 코드를 입력하는 노트예요. ✏️ 표시가 있는 칸에 입력하세요.
5. 막히거나 복습할 때는 <b>정답 노트</b>를 열어 보세요.
6. 셀은 위에서부터 순서대로 실행하세요. 연결이 끊겼다면 처음부터 다시 실행하면 됩니다.

## 강의별 실습 노트

| 강의 | 주제 | 실습 노트 | 정답 노트 |
| --- | --- | --- | --- |
| 1강 | 인공지능의 역사와 코랩 시작하기 | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jetsonai/StartClassBeginner/blob/main/MachineLearning/ml_kiosk_01.ipynb) | 실행만 하는 노트 |
| 2강 | 머신러닝 데이터 기초 (NumPy · Pandas · 그래프) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jetsonai/StartClassBeginner/blob/main/MachineLearning/ml_kiosk_02.ipynb) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jetsonai/StartClassBeginner/blob/main/MachineLearning/ml_kiosk_02_answer.ipynb) |
| 3강 | 머신러닝 (scikit-learn) | 준비 중 | 준비 중 |
| 4강 | 신경망 (PyTorch) | 준비 중 | 준비 중 |
| 5강 | CNN (이미지 · YOLO) | 준비 중 | 준비 중 |
| 6강 | RNN (시계열 · LSTM) | 준비 중 | 준비 중 |
| 7강 | 트랜스포머 (언어 · LLM) | 준비 중 | 준비 중 |

## 실습 데이터

[`kiosk_sales.csv`](kiosk_sales.csv): 파이썬 카페의 2025년 1년 치(365일) 판매 기록입니다. 실습 노트가 이 파일을 자동으로 불러오니 따로 내려받지 않아도 됩니다.

| 열 이름 | 뜻 |
| --- | --- |
| `date` | 날짜 |
| `month` | 월 (1 ~ 12) |
| `weekday` | 요일 (월 ~ 일) |
| `temp` | 최고기온(℃). 일부러 비워 둔 날이 있어요 (2강에서 채웁니다) |
| `rain` | 비 온 날 1, 아니면 0 |
| `americano` · `ice_americano` · `latte` · `oat_latte` | 음료별 판매량(잔) |
| `cheesecake` · `sandwich` · `fruit_cup` | 디저트·푸드별 판매량(개) |
| `cake_soldout` | 치즈케이크 품절 1, 아니면 0 (하루 20개 한정) |

> 강의용으로 만든 가상 데이터입니다.
