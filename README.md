## 영화 리뷰 감성 분석

### ✔ 주제

: 한국어 문장인 영화 리뷰를 입력받아 감성(긍정, 부정) 분석을 하는 모델 빌드 및 학습

### ✔ 데이터

- 오픈소스 데이터: [train](https://raw.githubusercontent.com/e9t/nsmc/master/ratings_train.txt), [test](https://raw.githubusercontent.com/e9t/nsmc/master/ratings_test.txt)
- [네이버 영화 리뷰 페이지](https://movie.naver.com/movie/point/af/list.naver?&page=1)에서 크롤링

### ✔ 수행 방법

1. 오픈소스 데이터 다운로드
2. 결측치 확인 및 제거
3. 리뷰 문장에 대한 형태소 분석, 형태소:숫자 매칭 사전 생성, 문장을 벡터로 변환
4. 벡터 길이 통일
5. 모델 생성 (Embedding, LSTM, Dense 레이어)
6. 모델 학습
7. 네이버 영화 리뷰 데이터 크롤링
8. 모델 추가 학습

### ✔ 사용 라이브러리

: Os, Datetime, Multiprocessing, Matplotlib, Pandas, Numpy, Konlpy, Tensorflow, Keras

