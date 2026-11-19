# 딥러닝 완전 정복

『딥러닝 완전 정복』(김영희 지음)의 예제 코드입니다. 책의 각 장에서 따라 입력하는 코드가 장별 폴더에 노트북으로 들어 있습니다.

## 책 소개

신경망을 넘파이로 직접 만들고 파이토치로 옮기면서, 시드와 설정에 따라 달라지는 숫자를 재고 적는 방법을 함께 배웁니다. 역전파와 자동 미분, 옵티마이저와 규제, 합성곱·순환 신경망, 어텐션과 트랜스포머, 사전 학습과 미세 조정, 해석, 보정, 실험 기록과 최종 평가까지 4부 16장입니다. 『머신러닝 완전 정복』 다음에 읽는 책입니다.

- 지은이: 김영희
- 발행: 2026년 11월, 주식회사 부크크
- 판형: B5, 856쪽

## 폴더 구성

| 부 | 장 | 제목 | 노트북 |
|---|---|---|---|
| 1부 신경망의 구조와 학습 | 1 | 선형 모델에서 신경망으로 | `ch01/ch01_from_linear_models_to_neural_networks.ipynb` |
|  | 2 | 역전파: 넘파이로 신경망 구현하기 | `ch02/ch02_backpropagation.ipynb` |
|  | 3 | 파이토치와 자동 미분 | `ch03/ch03_pytorch_and_autograd.ipynb` |
|  | 4 | 학습이 불안정해지는 이유 | `ch04/ch04_why_training_becomes_unstable.ipynb` |
| 2부 최적화와 일반화 | 5 | 미니배치와 옵티마이저 | `ch05/ch05_minibatch_and_optimizers.ipynb` |
|  | 6 | 신경망의 규제 | `ch06/ch06_regularization.ipynb` |
|  | 7 | 과적합을 다시 보기: 이중 하강 | `ch07/ch07_double_descent.ipynb` |
|  | 8 | 표 자료에서의 신경망 | `ch08/ch08_neural_networks_on_tabular_data.ipynb` |
| 3부 구조가 있는 자료 | 9 | 합성곱 신경망 | `ch09/ch09_convolutional_neural_networks.ipynb` |
|  | 10 | 순서가 있는 자료: 순환 신경망 | `ch10/ch10_recurrent_neural_networks.ipynb` |
|  | 11 | 임베딩과 어텐션 | `ch11/ch11_embeddings_and_attention.ipynb` |
|  | 12 | 트랜스포머 | `ch12/ch12_transformer.ipynb` |
| 4부 사전 학습과 평가 | 13 | 사전 학습 모델과 미세 조정 | `ch13/ch13_pretraining_and_finetuning.ipynb` |
|  | 14 | 신경망의 해석 | `ch14/ch14_interpreting_neural_networks.ipynb` |
|  | 15 | 신경망 예측의 보정과 불확실성 | `ch15/ch15_calibration_and_uncertainty.ipynb` |
|  | 16 | 실험 기록과 최종 평가 | `ch16/ch16_experiment_records_and_final_evaluation.ipynb` |

## 실행 방법

구글 코랩에서 노트북을 열고, 첫 칸의 안내대로 내려받은 파일을 왼쪽 파일 창에 올린 다음 위에서부터 차례로 실행합니다. 런타임 유형은 기본값인 CPU로 둡니다. 자기 컴퓨터에서 실행할 때는 파일을 노트북과 같은 폴더에 둡니다. 노트북에는 실행 결과를 넣지 않았습니다. 결과는 직접 실행해서 책의 출력과 비교합니다.

모든 노트북은 GPU 없이 CPU에서 실행합니다. 각 노트북의 첫 칸에 적힌 시간(2분에서 30분쯤)은 책을 쓴 컴퓨터에서 잰 것입니다. 코랩의 CPU에서는 세 배쯤 걸립니다. 가장 오래 걸리는 13장이 코랩에서 70분쯤이었습니다. 책의 숫자는 파이썬 3.13, 넘파이 2.5, 파이토치 2.15(CPU, 스레드 2개)에서 얻은 것입니다. 환경이 다르면 같은 시드로도 숫자가 조금 다를 수 있습니다. 그 크기는 책의 16.2절에서 잽니다.

책 본문에는 그래프를 그리는 코드를 싣지 않았습니다. 그래프 코드는 노트북에서 첫 줄이 `# 그림 N-n`인 셀에 있습니다.

## 자료

이 저장소에는 자료 파일을 넣지 않았습니다. 모두 누구나 내려받을 수 있는 자료입니다.

| 장 | 자료 | 받는 곳 |
|---|---|---|
| 1~7, 10, 15 | 시간별 전국 전력수요량 (2023년, 2025년) | [공공데이터포털](https://www.data.go.kr/data/15065266/fileData.do) |
| 1~7, 15 | 종관기상관측(ASOS) 시간자료 (2023년, 2025년) | [기상자료개방포털](https://data.kma.go.kr/data/grnd/selectAsosRltmList.do?pgmNo=36) |
| 1, 8, 16 | 아파트 매매 실거래가 (서울, 2023~2024년 계약분) | [국토교통부 실거래가 공개시스템](https://rt.molit.go.kr) |
| 9, 14, 15, 16 | Fashion-MNIST 학습용 파일 `train-images-idx3-ubyte.gz`, `train-labels-idx1-ubyte.gz` | [zalandoresearch/fashion-mnist](https://github.com/zalandoresearch/fashion-mnist) |
| 11, 12, 13, 14, 16 | NSMC 학습용 파일 `ratings_train.txt` | [e9t/nsmc](https://github.com/e9t/nsmc) |
| 16 | Fashion-MNIST 시험용 파일 `t10k-images-idx3-ubyte.gz`, `t10k-labels-idx1-ubyte.gz`, NSMC 시험용 파일 `ratings_test.txt` | 위와 같은 곳 |

시험용 파일 세 개는 16장에서만 씁니다. 1장부터 15장까지는 읽지 않습니다. 공공 파일은 수정될 수 있으므로 받은 날짜가 다르면 책의 숫자와 소수 끝자리가 다를 수 있습니다. Fashion-MNIST 파일이 책과 같은 파일인지는 16.1절의 `fingerprint`로 확인할 수 있습니다.

영화평 자료에는 거친 표현이 들어 있는 글이 있습니다. 책에 실은 예문은 그런 표현이 없는 것을 골랐습니다.
