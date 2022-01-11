---
layout: post
title:  텍스쳐 자동 분석 증강현실 FPS 게임
period:   2020.11
image:  /assets/images/blog/AutoTextureRecogFPS/title.png
author: K.S. KIM
tags:   연구 개발
portfolio-type:
    - type: "research and development"
---

<h4 class="text-bold">구면 파노라마 영상을 기반으로 영상처리를 통해 텍스쳐를 분석하여 자동으로 효과음을 생성하는 FPS 게임</h4>

⯀ 프로젝트명: 텍스쳐 자동 분석 증강현실 FPS 게임<br>
⯀ 개발 인원: 1인 개발<br>
⯀ 장르: R&D<br>
⯀ 플랫폼: Windows PC<br>
⯀ 개발 기간: 2020.11<br>
⯀ 개발 환경: Unreal Engine, C++<br>
⯀ 소스 공개 여부: O<br>
⯀ 프로젝트 링크: <a href = "https://github.com/wis1906/spherical-fps" target = "parent" >[깃허브 레포지토리]</a>
<br><br><br><br><br>


<hr width="100%" color="white" size="3" align="center">


<h4 class="text-bold text-center">⦁ 소개 ⦁</h4>
구면 영상을 활용하는 게임 공간은 사용자에게 극대화된 현실감을 줄 수 있습니다.<br>
FPS 게임은 높은 몰입감과 현실감이 중요한 게임 장르입니다.<br>
구면 영상을 활용한 배경 공간은 현실감을 강조하는 FPS 게임에 적합한 기술입니다.<br>
그러나, FPS 게임에 구면 영상을 배경으로 적용할 때에는 공간의 깊이 파악, 다양한 재질에 따른 역동적인 변화 등 고려해야 할 점들이 있습니다.<br>
<br>
<div class="text-center">
    <div class="text-center text-bold" style="height:500px; border:4px outset purple; display:inline-block; margin-right:5px; padding:5px;">
        <img class="scalezoom_small" src="/assets/images/blog/AutoTextureRecogFPS/intro_gamespace.png" alt="제작한 FPS 게임 공간" height="90%">
        <figcaption>제작한 FPS 게임 공간</figcaption></div>
    <div style="clear:both;"></div>
</div>
본 연구 프로그램은 구면 파노라마를 활용한 배경 공간을 배경으로 하는 FPS 게임에서 질감을 고려하여 역동적인 충돌 효과음을 생성하는 방법을 제안합니다.<br>
제안 방법은 깊이맵을 통해 공간감을 형성하고, 총알의 충돌 지점 주변 재질을 분석하여 역동적인 충돌 효과음을 생성합니다.<br>
제안 방법을 구면 공간을 사용하는 FPS 게임에 적용하여 실험한 결과 다양한 충돌 효과음을 효과적으로 생성됨을 보였습니다.<br>


<br><br>
<hr width="100%" color="white" size="3" align="center">


<h4 class="text-bold text-center">⦁ 성과 ⦁</h4>
<div class="text-center">
    <div class="text-center text-bold" style="height:400px; border:4px outset purple; display:inline-block; margin-right:5px; padding:5px;">
        <img class="scalezoom_big" src="/assets/images/blog/AutoTextureRecogFPS/reward_paper.jpg" alt="한국게임학회 논문 게재" height="85%">
        <figcaption>한국게임학회 논문 게재</figcaption></div>
    <div class="text-center text-bold" style="height:400px; border:4px outset purple; display:inline-block; margin-right:5px; padding:5px;">
        <img class="scalezoom_big" src="/assets/images/award_certificate/price_2020_kcgscf.jpg" alt="우수논문발표상 수상" height="85%">
        <figcaption>우수논문발표상(넥슨코리아상) 수상</figcaption></div>
    <div style="clear:both;"></div>
</div>
⯀ 2020년도 한국게임학회 추계학술발표대회에 '구면 파노라마 배경의 FPS 게임에서의 질감을 고려한 효과음 생성'에 대한 논문 게재<br>
⯀ 2020년도 한국게임학회 추계학술발표대회에서 우수발표상(넥슨코리아상) 수상<br>


<br><br>
<hr width="100%" color="white" size="3" align="center">


<h4 class="text-bold text-center">⦁ 상세 설명 ⦁</h4>
<div class="text-center">
    <div class="text-center text-bold" style="height:300px; border:4px outset purple; display:inline-block; margin-right:5px; padding:5px;">
        <img class="scalezoom_small" src="/assets/images/blog/AutoTextureRecogFPS/intro_lbp.png" alt="LBP의 원리 소개" height="85%">
        <figcaption>LBP의 원리 소개</figcaption></div>
    <div class="text-center text-bold" style="height:300px; border:4px outset purple; display:inline-block; margin-right:5px; padding:5px;">
        <img class="scalezoom_small" src="/assets/images/blog/AutoTextureRecogFPS/intro_cslbp_histogram.png" alt="CS-LBP 히스토그램을 활용한 재질 분석 프로세스" height="85%">
        <figcaption>CS-LBP 히스토그램을 활용한 재질 분석 프로세스</figcaption></div>
    <div style="clear:both;"></div>
</div>
설계한 시스템은 구면 파노라마 이미지를 기반으로 큐브맵 스카이박스를 생성합니다. 이는 증강현실 공간으로 활용됩니다.<br>
시스템은 총알 충돌 지점의 주변 이미지 영역을 파악하여 재질을 분석하고, 사전에 입력된 재질 데이터와 비교하여 적절한 충돌 효과음을 생성합니다.<br>
이를 위해서 총알 충돌 지점 주변의 이미지 패치를 획득하고, 사전에 입력된 재질 데이터와의 이진 특성값 CS-LBP를 분석합니다.<br>
사전 입력된 재질 데이터의 CS-LBP는 히스토그램으로 나타낼 경우 각각 고유의 특성을 지니고 있습니다.<br>
충돌 지점의 히스토그램과 사전 입력된 재질에 관한 히스토그램을 비교할 경우, 해당 지점에서 출력해야 할 충돌음을 파악할 수 있습니다.<br>
더욱 자세한 내용은 하단의 버튼을 통해 확인하실 수 있습니다.<br>
<div class="text-center">
    <a href="/assets/images/blog/AutoTextureRecogFPS/paper.pdf" class="btn btn-xs btn-primary">논문 원문 보기</a>
</div>


<br><br>
<hr width="100%" color="white" size="3" align="center">


<h4 class="text-bold text-center">⦁ 참고 영상 ⦁</h4>
<div class="text-center">
    <div class="text-center text-bold" style="border:4px outset clear; display:inline-block; margin-right:10px;">
        <iframe width="540" height="320" src="https://www.youtube.com/embed/y3ajHxs-sT8" frameborder="0" allowfullscreen></iframe>
        <figcaption>게임 시연 영상</figcaption></div>
    <div class="text-center text-bold" style="border:4px outset clear; display:inline-block; margin-right:10px;">
        <iframe width="540" height="320" src="https://www.youtube.com/embed/1d743HR3tv4" frameborder="0" allowfullscreen></iframe>
        <figcaption>학술대회 발표 영상</figcaption></div>
    <div style="clear:both;"></div>
</div>