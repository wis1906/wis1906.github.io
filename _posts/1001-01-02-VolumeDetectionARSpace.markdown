---
layout: post
title: 실내 공간 볼륨 검출 기반 증강현실 게임
period:   2021.04 - 2021.07
image:  /assets/images/blog/VolumeDetectionARSpace/title.png
author: K.S. KIM
tags:   연구 개발
portfolio-type:
    - type: "research and development"
---

<h4 class="text-bold">구면 파노라마 영상 기반 실내 공간에 대한 점군의 볼륨 검출을 통해 구성한 증강현실 공간 기반의 게임</h4>

⯀ 프로젝트명: 실내 공간 볼륨 검출 기반 증강현실 게임<br>
⯀ 개발 인원: 1인 개발<br>
⯀ 장르: R&D<br>
⯀ 플랫폼: Windows PC<br>
⯀ 개발 기간: 2021.04 - 2021.07<br>
⯀ 개발 환경: Unreal Engine, C++<br>
⯀ 소스 공개 여부: O<br>
⯀ 프로젝트 링크: <a href = "https://github.com/wis1906/cuboid-volume-ar-space" target = "parent" >[깃허브 레포지토리]</a>
<br><br><br><br><br><br><br><br><br><br><br><br>

<h4 class="text-bold text-center">- 소개 -</h4>
증강현실 공간을 구축하기 위해서는 점군, 오브젝트, 평면 등 실제 공간의 유의미한 인식 과정이 필요합니다.<br>
기존의 실내 공간 인식 방법은 철저하게 관측 가능한 공간에 대해서만 평면 검출이 가능하며, 밀도와 노이즈의 변화에 민감합니다.<br>
이는 증강현실이 활용되는 실내 공간의 특성을 이해하여 극복할 수 있습니다.<br>
증강현실이 활용되는 대부분 실내 공간은 방이며, 대부분의 방은 직육면체 모양입니다.<br>
<br>
<div class="text-center">
    <div class="text-center text-bold" style="height:500px; border:4px outset purple; display:inline-block; margin-right:5px; padding:5px;">
        <img class="scalezoom_small" src="/assets/images/blog/VolumeDetectionARSpace/introduce_ARSpace.png" alt="볼륨 검출 기반 AR 공간" height="90%">
        <figcaption>볼륨 검출 기반 AR 공간</figcaption></div>
    <div class="text-center text-bold" style="height:500px; border:4px outset purple; display:inline-block; margin-right:5px; padding:5px;">
        <img class="scalezoom_small" src="/assets/images/blog/VolumeDetectionARSpace/introduce_ARGame.png" alt="AR 공간을 기반으로 한 게임 콘텐츠 구현" height="90%">
        <figcaption>AR 공간을 기반으로 한 게임 콘텐츠 구현</figcaption></div>
    <div style="clear:both;"></div>
</div>
본 연구 프로그램은 직육면체 방 형태의 실내 공간에서 점군 데이터 기반 직육면체 볼륨 검출을 통해 빠르고 정확하게 AR 게임 공간을 구성하는 방법을 제안합니다.<br>
제안 방법은 기존의 평면 검출 알고리즘에서 벗어나 Oriented Bounding Box (OBB) 검출 방법을 기반으로 한 Top-Down 방식을 활용합니다.<br>
또한, 공간 인식의 효율을 극대화하고 표현의 자유도를 높이기 위해 구면 파노라마 비디오를 기반으로 합니다.<br>
<br><br>


<h4 class="text-bold text-center">- 성과 -</h4>
<div class="text-center">
    <div class="text-center text-bold" style="height:400px; border:4px outset purple; display:inline-block; margin-right:5px; padding:5px;">
        <img class="scalezoom_big" src="/assets/images/blog/VolumeDetectionARSpace/reward_paper_kcgsc.jpg" alt="한국게임학회 논문 게재" height="85%">
        <figcaption>한국게임학회 논문 게재</figcaption></div>
    <div class="text-center text-bold" style="height:400px; border:4px outset purple; display:inline-block; margin-right:5px; padding:5px;">
        <img class="scalezoom_big" src="/assets/images/award_certificate/price_2021_kcgscs.jpg" alt="우수논문발표상 수상" height="85%">
        <figcaption>우수논문발표상 수상</figcaption></div>
    <div style="clear:both;"></div>
</div>
⯀ 2021년도 한국게임학회 춘계학술발표대회에 '실내 구면 파노라마에서의 볼륨 검출을 통한 AR 게임 공간 구성'에 대한 논문 게재<br>
⯀ 2021년도 한국게임학회 춘계학술발표대회에서 우수논문상 수상<br>
<br><br>


<h4 class="text-bold text-center">- 상세 설명 -</h4>
<div class="text-center">
    <div class="text-center text-bold" style="height:400px; border:4px outset purple; display:inline-block; margin-right:5px; padding:5px;">
        <img class="scalezoom_small" src="/assets/images/blog/VolumeDetectionARSpace/detail_pipeline_volume.png" alt="볼륨 검출 과정 파이프라인" height="85%">
        <figcaption>볼륨 검출 과정 파이프라인</figcaption></div>
    <div class="text-center text-bold" style="height:400px; border:4px outset purple; display:inline-block; margin-right:5px; padding:5px;">
        <img class="scalezoom_small" src="/assets/images/blog/VolumeDetectionARSpace/detail_pipeline_gamespace.png" alt="검출된 볼륨 데이터 기반 게임 환경 구축 파이프라인" height="85%">
        <figcaption>검출된 볼륨 데이터 기반 게임 환경 구축 파이프라인</figcaption></div>
    <div style="clear:both;"></div>
</div>
볼륨 검출 과정은 3개의 주요 과정으로 구성됩니다.<br>
먼저, 구면 파노라마 기반의 Vision SLAM을 통해 실시간으로 점군 데이터를 획득하고, KDTree를 구성해 이웃점과 거리가 먼 이상점을 제거합니다.<br>
다음으로, 점군 데이터를 감싸는 최적의 OBB를 검출합니다.<br>
마지막으로, 생성된 OBB 볼륨의 품질을 정량적으로 평가하고, 실시간으로 좋은 품질의 OBB로 생산합니다.<br>
<br>
볼륨 검출 과정 이후에는, 먼저 구면 파노라마의 왜곡을 제거하기 위해 3차원 큐브맵 이미지로 변환합니다.<br>
큐브맵 이미지는 거대한 스카이박스처럼 가상 세계 안에 매우 큰 정육면체 형태로 배치합니다.<br>
다음으로, 가상 세계 안에서의 카메라의 위치 및 자세를 플레이어와 큐브맵 정육면체에 반영합니다.<br> 
마지막으로, 볼륨 검출 과정을 통해 획득한 OBB의 6개의 평면을 가상 세계에 배치합니다.<br>
더욱 자세한 내용은 하단의 버튼을 통해 확인하실 수 있습니다.<br>
<div class="text-center">
    <a href="/assets/images/blog/VolumeDetectionARSpace/paper_kcgsc.pdf" class="btn btn-xs btn-primary">한국게임학회 논문 원문 보기</a>
</div>
<br><br>


<h4 class="text-bold text-center">- 참고 영상 -</h4>
<div class="text-center">
    <div class="text-center text-bold" style="border:4px outset clear; display:inline-block; margin-right:10px;">
        <iframe width="360" height="240" src="https://www.youtube.com/embed/fcC7243f1eo" frameborder="0" allowfullscreen></iframe>
        <figcaption>볼륨 검출 기반 AR 공간 영상</figcaption></div>
    <div class="text-center text-bold" style="border:4px outset clear; display:inline-block; margin-right:10px;">
        <iframe width="360" height="240" src="https://www.youtube.com/embed/thdIbGphfOk" frameborder="0" allowfullscreen></iframe>
        <figcaption>AR 공간을 기반으로 한 게임 콘텐츠 구현 영상</figcaption></div>
    <div class="text-center text-bold" style="border:4px outset clear; display:inline-block; margin-right:10px;">
        <iframe width="360" height="240" src="https://www.youtube.com/embed/-oYKQRguhfQ" frameborder="0" allowfullscreen></iframe>
        <figcaption>학술대회 발표 영상</figcaption></div>
    <div style="clear:both;"></div>
</div>