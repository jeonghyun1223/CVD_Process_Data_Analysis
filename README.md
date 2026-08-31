# CVD Process Data Analysis & Report Automation
CVD(Chemical Vapor Deposition) 공정의 가상 데이터를 활용하여 공정 조건에 따른 박막 두께를 분석하고, 머신러닝 기반 예측 모델을 구축한 프로젝트입니다.

Python을 활용해 데이터 전처리 및 시각화를 수행하고, Random Forest를 이용하여 공정 조건과 박막 두께 간의 관계를 분석했습니다. 또한 생성형 AI API를 연동하여 분석 결과를 바탕으로 공정 분석 보고서 초안 작성 과정을 자동화했습니다.

# Project Overview

Project: CVD 공정 데이터 분석 및 보고서 작성 자동화
Language: Python
Data: CVD 공정 가상 데이터
Machine Learning: Random Forest
AI: Gemini API
Main Goal: 공정 데이터 분석 및 분석 보고서 작성 과정 자동화

# Workflow

CVD 공정 데이터 → 데이터 전처리 → 데이터 탐색 및 시각화 → Random Forest 모델 구축 → 공정 조건별 영향도 분석 → 분석 결과 정리 → Gemini API 연동 → 분석 보고서 초안 자동 생성

# Data Analysis

Python을 활용하여 CVD 공정 데이터를 전처리하고 주요 변수 간의 관계를 시각화했습니다.

주요 분석 항목:
데이터 전처리
변수 간 상관관계 분석
공정 조건에 따른 박막 두께 변화 분석
데이터 시각화
Feature Importance 분석

# Machine Learning

Random Forest Regression을 활용하여 CVD 공정 조건으로부터 박막 두께를 예측하는 모델을 구축했습니다.
모델을 통해 각 입력 변수의 상대적인 중요도를 분석하고, 공정 조건에 따라 박막 성장에 영향을 미치는 주요 변수를 확인했습니다.
분석 과정에서 온도 조건에 따라 주요 영향 변수가 달라지는 경향을 확인했습니다.

상대적으로 낮은 온도 조건: RF Power의 영향이 크게 나타남
상대적으로 높은 온도 조건: Deposition Time의 영향이 크게 나타남

이를 통해 전체 데이터를 하나의 관계로만 분석하기보다 조건에 따른 데이터의 특성을 구분하여 분석하는 접근을 수행했습니다.

# Report Automation

분석 결과를 바탕으로 생성형 AI API를 활용하여 공정 분석 보고서 초안을 자동으로 생성하는 기능을 구현했습니다.
기존에는 분석 결과를 확인한 후 보고서 초안을 직접 작성하는 데 약 36분이 소요되었으나, 자동화 과정을 적용한 결과 약 2분으로 단축되었습니다.
보고서 초안 작성 시간 약 94% 단축

분석 결과 → 주요 결과 추출 → Gemini API 전달 → 분석 결과 기반 보고서 초안 생성

# Technologies
Python
Pandas
NumPy
Matplotlib
Scikit-learn
Random Forest
Gemini API
Google Colab

# Key Results
데이터 분석 :	CVD 조건별 박막 두께 분석
머신러닝 :	Random Forest 기반 두께 예측
변수 분석 :	Feature Importance를 통한 주요 변수 확인
조건별 분석 :	온도 조건에 따른 영향 변수 차이 확인
보고서 자동화 :	생성형 AI API 기반 보고서 초안 생성
자동화 성과 :	작성 시간 약 36분 → 2분
시간 단축률	약 94%

# Notes

본 프로젝트에서 사용한 CVD 데이터는 분석 및 머신러닝 학습을 위한 가상 데이터입니다.
API Key와 같은 인증 정보는 GitHub에 업로드하지 않으며, 환경변수를 통해 관리합니다.

# 프로젝트 진행 단계

1. 데이터셋_전처리_시각화.ipynb
   - CVD 가상 데이터 전처리
   - 데이터 탐색 및 시각화
   - 공정 조건과 박막 두께 간 관계 분석

2. 분석_및_자동화.py
   - 분석 과정 Python 코드화
   - Random Forest 기반 박막 두께 예측
   - 분석 결과 정리
   - Gemini API를 활용한 보고서 초안 자동 생성
