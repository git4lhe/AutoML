# Orientation task 1

# Task 1
- marketing subscribes
- binary classification 
- categorical and numerical datasets
- condition
- 1) pass input arguments through command-line options
- 2) report for prediction values/evaluation as csv file

# Dataset
- train:validation = 0.64:0.37
- N of train : 15292
- N of valdiation : 8982
- N of test : 9043

# Traning and validation results
- best parameters :  {'kernel': 'poly', 'gamma': 'scale', 'C': 1}
- training time : 46.2391s

# Experiment settings
- train, data files
- data name
- optimization
- split ratio
- classifier
- report and prediction csv file
- model save

# Test results
tn:7786 fp:166 fn:772 tp:319
Precision:0.6577
Recall   :0.2924
Accuracy :0.8963
F1-score :0.4048

# variables
- age: 나이
- job: 직종
- marital_status: 결혼여부
- education: 최종학위
- default: 부도여부
- balance: 통장잔고
- housing_loan: 주택대출여부
- personal_loan: 개인대출여부
- contact_channel: 은행에서 고객에게 연락을 취한 방식
- last_contact_day: 마지막 연락일
- last_contact_month: 마지막 연락월
- contact_duration: 고객과의 통화시간
- campaign: 고객과의 연락횟수
- gap_between_campaigns: 마지막 연락이후 경과기간
- previous: 현재 캠페인 이전에 연락한 횟수
- outcome_previous_campaign: 이전 마케팅 성공여부
- "insurance_subscribe: 상품구독여부(1: yes, 0: no)"

# Method
- SVM for solution
- parameter optimization 

# Class
- build-up for additional future work
- Datasource : preprocessing, visualization, 
- Algorithm : svm

## Train
- python main.py --purpose train --train "marketing_train.csv"

## Test
- python main.py --purpose test --test "marketing_test.csv" --prediction "pred.csv" --report "report.csv"
 