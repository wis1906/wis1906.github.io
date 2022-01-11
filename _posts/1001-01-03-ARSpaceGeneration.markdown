---
layout: post
title: 구면 비디오 기반 실내 기하 검출을 통한 증강 게임 공간 생성
period:   2021.07 - 2021.12
image:  /assets/images/blog/ARSpaceGeneration/title.png
author: K.S. KIM
tags:   연구 개발
portfolio-type:
    - type: "research and development"
---

<h4 class="text-bold">구면 파노라마 영상 기반 실내 직육면체형 기하와 다중 객체 영역 검출을 통한 증강 게임</h4>

⯀ 프로젝트명: 구면 비디오 기반 실내 기하 검출을 통한 증강 게임 공간 생성<br>
⯀ 개발 인원: 1인 개발<br>
⯀ 장르: R&D<br>
⯀ 플랫폼: Windows PC<br>
⯀ 개발 기간: 2021.07 - 2021.12<br>
⯀ 개발 환경: Unreal Engine, C++<br>
⯀ 소스 공개 여부: O<br>
⯀ 프로젝트 링크: <a href = "https://github.com/wis1906/letsgo-ar-space-generation" target = "parent" >[깃허브 레포지토리]</a>
<br><br><br><br><br><br><br><br><br><br><br><br>



<hr width="100%" color="white" size="3" align="center">


<h4 class="text-bold text-center">⦁ 소개 ⦁</h4>
오늘날의 증강 게임은 더욱 섬세한 상호작용과 시각적 표현을 위해 주변 공간의 구체적인 기하 정보가 필요합니다.<br>
기존의 실내 공간 인식 방법은 점군의 밀도와 노이즈에 취약하고, 미완성된 기하 정보만을 검출합니다.<br>
따라서 주요 평면의 완전한 인식이 어렵고, 실세계 속 객체의 부피나 구체적인 영역 등은 파악할 수 없습니다.<br>
직육면체 형태의 공간의 특성을 고려한 공간 인식은 대부분의 실내 공간에서 활용할 수 있습니다.<br>
직육면체 공간에서 실내의 특성을 고려한 기하 검출 방법을 통해 많은 영역을 비교적 정확하게 검출할 수 있습니다.<br>
<br>
<div class="text-center">
    <div class="text-center text-bold" style="height:500px; border:4px outset purple; display:inline-block; margin-right:5px; padding:5px;">
        <img class="scalezoom_small" src="/assets/images/blog/ARSpaceGeneration/introduce_ARSpace.png" alt="기하 검출을 통한 증강 게임 공간 구성" height="90%">
        <figcaption>기하 검출을 통한 증강 게임 공간 구성</figcaption></div>
    <div class="text-center text-bold" style="height:500px; border:4px outset purple; display:inline-block; margin-right:5px; padding:5px;">
        <img class="scalezoom_small" src="/assets/images/blog/ARSpaceGeneration/introduce_advence.jpg" alt="게임 공간 속 세밀한 기하 예측" height="90%">
        <figcaption>게임 공간 속 세밀한 기하 예측</figcaption></div>
    <div style="clear:both;"></div>
</div>
본 연구 프로그램은 직육면체 형태의 실내 공간에서 증강 게임 공간을 구성하는 방법을 제안합니다.<br>
제안 알고리즘은 빠른 공간 인식과 응용 콘텐츠 개발 다양화의 폭을 넓히기 위해 구면 파노라마 비디오를 입력으로 하여 모든 시야각을 활용합니다.<br>
제안 알고리즘은 기존의 평면 검출 기반의 접근 방법에서 벗어나 Oriented Bounding Box (OBB) 검출을 통한 접근 방법으로 실내 표면 기하를 검출합니다.<br>
또한, 제안 알고리즘은 계층적 유클리드 군집화와 군집 간소화 및 조정을 통해 다중 객체 영역을 검출합니다.<br>
제안하는 검출 알고리즘은 점군의 밀도 변화에 강건하고, 실내 표면이나 객체에 대한 완전한 기하 정보를 검출할 수 있습니다.<br>
<br>
<div class="text-center">
	<div class="text-center text-bold" style="height:500px; border:4px outset purple; display:inline-block; margin-right:5px; padding:5px;">
		<img class="scalezoom_small" src="/assets/images/blog/ARSpaceGeneration/introduce_contents.png" alt="증강 게임 공간을 기반으로 한 콘텐츠 구현" height="90%">
		<figcaption>증강 게임 공간을 기반으로 한 콘텐츠 구현</figcaption></div>
    <div style="clear:both;"></div>
</div>


<br><br>
<hr width="100%" color="white" size="3" align="center">


<h4 class="text-bold text-center">⦁ 성과 ⦁</h4>
<div class="text-center">
    <div class="text-center text-bold" style="height:400px; border:4px outset purple; display:inline-block; margin-right:5px; padding:5px;">
        <img class="scalezoom_big" src="/assets/images/blog/ARSpaceGeneration/reward_paper_thesis.png" alt="석사학위논문 제출" height="85%">
        <figcaption>석사학위논문 제출</figcaption></div>
    <div class="text-center text-bold" style="height:400px; border:4px outset purple; display:inline-block; margin-right:5px; padding:5px;">
        <img class="scalezoom_big" src="/assets/images/blog/ARSpaceGeneration/reward_paper_kipscf.jpg" alt="한국정보처리학회 논문 게재" height="85%">
        <figcaption>한국정보처리학회 논문 게재</figcaption></div>
    <div class="text-center text-bold" style="height:400px; border:4px outset purple; display:inline-block; margin-right:5px; padding:5px;">
        <img class="scalezoom_big" src="/assets/images/blog/ARSpaceGeneration/reward_paper_kcgscf.jpg" alt="한국게임학회 논문 게재" height="85%">
        <figcaption>한국게임학회 논문 게재</figcaption></div>
    <div class="text-center text-bold" style="height:400px; border:4px outset purple; display:inline-block; margin-right:5px; padding:5px;">
        <img class="scalezoom_big" src="/assets/images/award_certificate/price_2021_kcgscf.jpg" alt="우수논문발표상 수상" height="85%">
        <figcaption>우수논문발표상 수상</figcaption></div>
    <div style="clear:both;"></div>
</div>
⯀ '구면 비디오 기반 실내 증강 게임 공간 생성'에 대한 논문 석사학위논문 제출<br>
⯀ 2021년도 한국정보처리학회 추계학술발표대회에 '점군 클러스터링 기반 실내 공간의 다중 개체 영역 검출'에 대한 논문 게재<br>
⯀ 2021년도 한국게임학회 추계학술발표대회에 '실내 공간의 장애물 인식을 통한 AR 게임 공간 속 이동 가능 영역 검출'에 대한 논문 게재<br>
⯀ 2021년도 한국게임학회 추계학술발표대회에서 우수논문상 수상<br>


<br><br>
<hr width="100%" color="white" size="3" align="center">


<h4 class="text-bold text-center">⦁ 상세 설명 ⦁</h4>
<div class="text-center">
    <div class="text-center text-bold" style="height:400px; border:4px outset purple; display:inline-block; margin-right:5px; padding:5px;">
        <img class="scalezoom_small" src="/assets/images/blog/ARSpaceGeneration/detail_pipeline_detection.png" alt="실내 기하 검출 과정 파이프라인" height="85%">
        <figcaption>실내 기하 검출 과정 파이프라인</figcaption></div>
    <div class="text-center text-bold" style="height:400px; border:4px outset purple; display:inline-block; margin-right:5px; padding:5px;">
        <img class="scalezoom_small" src="/assets/images/blog/ARSpaceGeneration/detail_pipeline_gamespace.png" alt="증강 게임 공간 구성을 위한 파이프라인" height="85%">
        <figcaption>증강 게임 공간 구성을 위한 파이프라인</figcaption></div>
    <div style="clear:both;"></div>
</div>
실내 기하 검출 과정은 전처리, 실내 표면 직육면체 검출, 다중 객체 영역 검출의 3개의 주요 과정으로 구성됩니다.<br>
먼저, 전처리 과정에서는 구면 파노라마 기반 Vision SLAM을 통해 실시간 점군 데이터를 획득하고, KDTree를 통해 이웃점과 거리가 먼 이상점을 제거합니다.<br>
다음으로, 실내 표면 직육면체 검출 과정에서는 점군에 대한 최적의 OBB를 획득하고, 조정 과정을 통해 표면 기하를 갱신합니다.<br>
마지막으로, 다중 객체 영역 검출 과정에서는 실내 점군에 대한 유클리드 클러스터링을 통해 영역을 산정하고, 조정 과정을 통해 객체 영역을 획득합니다.<br>
<br>
기하 검출 과정 이후에는 가상세계 구조물 구축, 다면 텍스처 투영 과정으로 구성됩니다.<br>
가상세계 구조물 구축 과정에서는 검출하였던 기하 정보를 가상세계에 반영하고, 실세계와 동일 시점의 플레이어를 가상세계에 배치합니다.<br>
다면 텍스처 투영 과정에서는 기하 구조물의 각 면에 부분적인 핀홀 투영을 통해 최종적인 1인칭 합성 장면을 획득합니다.<br>
더욱 자세한 내용은 하단의 버튼을 통해 확인하실 수 있습니다.<br>
<div class="text-center">
    <a href="/assets/images/blog/ARSpaceGeneration/paper_kipscf.pdf" class="btn btn-xs btn-primary">한국정보처리학회 논문 보기</a>
    <a href="/assets/images/blog/ARSpaceGeneration/paper_kcgscf.pdf" class="btn btn-xs btn-primary">한국게임학회 논문 보기</a>
</div>


<br><br>
<hr width="100%" color="white" size="3" align="center">


<h4 class="text-bold text-center">⦁ 참고 영상 ⦁</h4>
<div class="text-center">
    <div class="text-center text-bold" style="border:4px outset clear; display:inline-block; margin-right:10px;">
        <iframe width="360" height="240" src="https://www.youtube.com/embed/1cy6iVrJ-ys" frameborder="0" allowfullscreen></iframe>
        <figcaption>핵심 시연 영상</figcaption></div>
    <div class="text-center text-bold" style="border:4px outset clear; display:inline-block; margin-right:10px;">
        <iframe width="360" height="240" src="https://www.youtube.com/embed/GzRL_0rAjWo" frameborder="0" allowfullscreen></iframe>
        <figcaption>전체 시연 영상</figcaption></div>
    <div class="text-center text-bold" style="border:4px outset clear; display:inline-block; margin-right:10px;">
        <iframe width="360" height="240" src="https://www.youtube.com/embed/Z5Ebk5OpnTw" frameborder="0" allowfullscreen></iframe>
        <figcaption>학술대회 발표 영상</figcaption></div>
    <div style="clear:both;"></div>
</div>