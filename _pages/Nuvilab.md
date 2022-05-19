---
layout: page
title: Nuvilab
permalink: /nuvilab/
---

## 얼굴 및 식판 인식 프로그램

- 얼굴과 식판을 인식한 후 식판 사진을 찍어 서버로 보내는 프로그램
- 얼굴은 기존에 등록된(얼굴 사진이 DB에 존재하는) 사람들 중 가장 비슷한 사람으로 인식
- 식판의 depth 사진과 rgb 사진으로 음식물 분석
- 2020년 9월 4일 환경의 날 행사 참여
    - [http://ttcnews.kr/news/newsview.php?ncode=1065617893290404](http://ttcnews.kr/news/newsview.php?ncode=1065617893290404)

#### UI, test 사진

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/nuvilab/nuvilab1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/nuvilab/nuvilab2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/nuvilab/nuvilab3.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

## 카페 쿠폰 적립 키오스크

- 얼굴 인식을 활용한 카페 쿠폰 적립 키오스크
- 회사 근처 카페에서 실제 사용
    - 500명 이상의 사용자
    - 95% 정도의 정확도
- 로그 관리
    
<div class="col-sm mt-3 mt-md-0">
    {% include figure.html path="assets/img/nuvilab/nuvilab4.png" title="example image" class="img-fluid rounded z-depth-1" %}
</div>

## 얼굴 인식 정확도 비교 연구

- Azure face, KNN, SVM, Face recognition, facenet, insight face 등 여러 모델을 비교
- 데이터
    - Labeled Faces in the Wild(LFW)
    - Celebrity 한 명당 100씩 100명의 데이터 직접 수집
        - 동양인, 서양인, 남성, 여성의 비율 비슷하게 수집
- 데이터에 따라 비교
    - 안경 유무
        - 데이터의 눈 위치에 안경을 씌워 테스트
    - 남성, 여성
    - 서양인, 동양인
    - 흔들림 정도
    - 마스크 유무
- train/test 비율에 따른 비교
- 상황에 따른 최적의 모델, 데이터의 형태를 연구를 통해 알아내고 적용
    - 정확도 3~5% 상승 (90%→95%)