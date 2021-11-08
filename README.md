# 2021년(제2회) NH투자증권 빅데이터 경진대회
- 예선 통과, 본선 진행 중
<br>

## 분석 주제
주식 보유기간 예측 및 서비스 아이디어 제안
- 예선 : 다양한 데이터를 활용하여 고객이 보유한 주식 종목 별 보유기간 예측
- 본선 : AI/빅데이터 분석 및 기술을 통한 서비스 아이디어 제안
<br>

## 분석 설명
### 1. 분석의 범주
> 분석 대상은 매수가 된 날의 주식 정보만을 이용해 모델을 학습시키기 위해 매수일자와 기준일자 값이 같은 것만을 분석 대상으로 삼았음
<br>

### 2. 모델링 진행 및 중요한 가정들
> 결측치가 유의미하게 많은 변수를 선택해 전처리 진행 
  - 투자 종목 시가총액규모유형 결측치 전처리 
    - 기존 대형주, 중형주, 소형주, 기타로 분류된 변수를 대형주, 중형주, 소형주, 펀드 or 파생상품, 우량주, 기타 카테고리로 세분화함 

  - 고객의 투자성향 결측치 KNN을 이용하여 전처리
    - 고객 투자성향의 결측치는 약37%로, 10000개 중 3687개 임을 확인하며, 2687개의 결측값을 이 외의 약6천여개의 데이터로 KNN 모델링하여 대체 

> LGBM Regressor 모델을 사용하여 모델링 진행
<br>

## 예선 제출 자료

- [코드](https://github.com/sihyeon3523/2021-2nd-NH-Investment-Securities-Big-Data-Competition/blob/e2313ac880d09b2b3df0a3ec4178573eba56deb6/%EB%AA%A8%EB%8D%B8_%EC%BD%94%EB%93%9C.py) 
- [개발 설명서](https://github.com/sihyeon3523/2021-2nd-NH-Investment-Securities-Big-Data-Competition/blob/e2313ac880d09b2b3df0a3ec4178573eba56deb6/%EB%AA%A8%EB%8D%B8_%EC%84%A4%EB%AA%85.ipynb)

## 본선 제출 자료
- [아이디어 제안서](https://github.com/sihyeon3523/2021-2nd-NH-Investment-Securities-Big-Data-Competition/blob/b96ab76366752dbba72cc10d17d032a9fc1aafb3/%EB%AF%BC%ED%8A%B8%EB%A7%9B%EB%B3%B4%EB%9D%BC.pdf)
