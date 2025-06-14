# 시각장애인을 위한 과자봉지 식별 프로젝트

![image](https://github.com/user-attachments/assets/1d5dd9b1-5e21-40f8-94a6-fbc66b46e3ca)
- 우연히 유튜브 쇼츠를 보다가 시각장애인 유튜버 ‘원샷한솔’님이 편의점에서 과자를 고르지 못하는 모습을 보고 아이디어를 구상해보았습니다.
- 유튜브 쇼츠 : https://youtube.com/shorts/Hcx6VTEUBsk?si=7GdP_sr5rGu0gHU5
<img width="343" alt="image" src="https://github.com/user-attachments/assets/b6496490-7d36-4cfd-b287-11041c287714">

# 페이지 구성
- 앱 온보딩뷰에 파란색 장미를 띄운 이유는 파란색 장미의 꽃말이 ‘불가능’, ’기적’ 이기 때문입니다.
- 시각장애인이 편의점에서 과자 고르는 일을 ‘불가능’에서 ‘가능’으로 만들어 기적을 만들어내고 싶었습니다.
- Flutter를 사용하였습니다.

|<img width="142" alt="image" src="https://github.com/user-attachments/assets/9558282d-0d6e-4c80-aa51-0dfb561ae284">|<img width="143" alt="image" src="https://github.com/user-attachments/assets/e94011c4-e15d-4da6-bf69-eb2ef06b88e2">|<img width="141" alt="image" src="https://github.com/user-attachments/assets/df3a0aba-a777-4760-94b6-97d5849ad2c2">|<img width="138" alt="image" src="https://github.com/user-attachments/assets/4628d876-400b-4046-bc16-b91dcd33227a">|<img width="137" alt="image" src="https://github.com/user-attachments/assets/405682dd-713d-44f6-9ab5-42bad30f6f03">|
|:---:|:---:|:---:|:---:|:---:|
|로딩페이지|카메라기능|게시판페이지|게시판에 글 작성 모습|장애인을 위한 LLM 챗봇

# AI - YOLOv5 사용
- YOLOv5를 이용해 과자식별AI를 만들어 정확도를 올리는데 집중하였습니다.
- 정확도를 올리기 위해 data argumentation을 이용하여 이미지 개수를 늘렸습니다.
- jubyter notebook환경에서 이미지 데이터를 shift, rotate하는 코드를 직접 구현하였습니다.

<img width="422" alt="image" src="https://github.com/user-attachments/assets/eb5b33ec-eced-4600-abd1-1909c5d52726">

- data argumentation(shift, reverse) 후 mAP50
<img width="610" alt="image" src="https://github.com/user-attachments/assets/9fccc8a2-17a9-4591-af9f-8559271eac1c" />

- 데이터 이미지셋 shuffle 후 mAP50
<img width="612" alt="image" src="https://github.com/user-attachments/assets/eb101bb8-c678-4c1e-8db4-d993faf21df9" />



- shift, reverse, shuffle 적용에 따른 PR그래프 차이!

<img width="612" alt="image" src="https://github.com/user-attachments/assets/7db4eae4-dcdb-4e80-9144-66e9c71855d0" />


# LLM 챗봇
<img width="720" alt="image" src="https://github.com/user-attachments/assets/67dc9b3d-ee1e-4332-b1a2-9ac8135826cd">
