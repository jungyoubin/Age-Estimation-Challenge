# Age-Prediction-Challenge
#### link: https://www.kaggle.com/competitions/2023-final/overview
- 2023 딥러닝기초 기말프로젝트
- 최종: 2위/36명

## Data Description
* 얼굴 이미지 (200x200)와 각 이미지에 대한 연령대 클래스로 구성 <br>
  - 0: 1세 ~ 10세 <br>
  - 1: 11세 ~ 20세 <br>
  - 2: 21세 ~ 30세 <br>
  - 3: 31세 ~ 40세 <br>
  - 4: 41세 ~ 50세 <br>
* 추가적으로, 나이, 성별, 인종에 대한 정보가 이미지 파일 이름에 포함

## Data Structure
* dataset: 학습을 위한 이미지 폴더
* data.csv: 데이터셋의 요약 정보를 포함한 CSV 파일
* testset: 테스트를 위한 이미지 폴더
* testdata.csv: 테스트셋의 요약 정보를 포함한 CSV 파일

## Dataset Details
* Train 이미지: '[age]_[gender]_[race]_[date&time].jpg' 형태로 구성
  - age: 정확한 나이
  - gender: 성별로, 0 (남자) 또는 1 (여자)
  - race: 인종으로, 0 (백인), 1 (흑인), 2 (아시아인), 3 (동남아인), 4 (기타, 히스페닉, 라틴, 중동 등)
  - date&time: 이미지 생성 날짜와 시간 (형식: yyyymmddHHMMSSFFF)
 
* Dataset.csv: 총 7340개의 이미지가 포함되어 있으며, 다음과 같은 열 존재:
  - Image: 이미지 파일 이름
  - Label: 해당 클래스
  - Age: 정확한 나이
  - Gender: 성별
  - Race: 인종

## Testset Details
* Test 이미지: '[gender]_[race]_[date&time].jpg' 형태로 구성
  - gender: 성별로, 0 (남자) 또는 1 (여자)
  - race: 인종으로, 0 (백인), 1 (흑인), 2 (아시아인), 3 (동남아인), 4 (기타, 히스페닉, 라틴, 중동 등)
  - date&time: 이미지 생성 날짜와 시간 (형식: yyyymmddHHMMSSFFF)

* Testset.csv: 총 822개의 이미지가 포함되어 있으며, 다음과 같은 열 존재:
  - Image: 이미지 파일 이름
  - Gender: 성별
  - Race: 인종
