# 일상 기록 미니 AI SNS 카메라


## 개요

라즈베리 파이 제로와 카메라모듈을 사용하여 일정 시간 간격으로 사진을 촬영하고, NIMA를사용하여 좋은 품질의 사진을 필터링한 후, LLM을 이용해 SNS 게시글을 자동으로 생성하고 게시

## 주요 기능

1. **사진 촬영**
   - 라즈베리 파이 제로에 연결된 웹캠을 이용하여 주기적(설정 가능)으로 사진 촬영
   - 촬영된 사진은 저장되고 WIFI를 사용하여 전송됨

2. **이미지 필터링**
   - NIMA를 통한 이미지 평가 (0~10의 실수 값으로 표현) 후 사용자의 별점으로 필터링
   

3. **텍스트 생성**
   - 사진과 텍스트가 있는 SNS게시물에서 BLIP을 이용해 캡션을 얻고 DB에 저장함으로써 사용자가 업로드 할 사진이 구성된 텍스트를 얻음
   - 웹 사용자 인터페이스를 만들어 글에 담아낼 감정 (긍정, 부정 등) , 또는 키워드를 입력하여 상황에 어울리는 게시글로 사용자 입맛에 맞게 구성
   - 사진의 내용과 특징을 반영하여 LLM을 활용한 글을 생성

4. **SNS 게시**
   - 생성된 텍스트를 SNS API 또는 공유 기능을 통해 게시
   - SNS서비스의 API를 사용하여 트윗을 작성하여 게시물 업로드

## 구조
<!--![스크린샷 2024-06-20 142024](https://github.com/NooriDoori/cam/assets/112747810/dad0e2a6-3c6b-45d5-8386-f15983ea17e1)-->

<!--![image](https://github.com/user-attachments/assets/5c26c429-50da-4e99-9d8a-f854e3f96a94)-->

<!-- https://github.com/user-attachments/assets/fd980b3c-f727-4d7c-80f2-799ebbe4699b -->

![image](https://github.com/user-attachments/assets/06df9af1-d069-4634-a153-a5207bf1ae59)

https://github.com/user-attachments/assets/7f6a3bde-5f38-4238-bd8c-ebced596342a

https://github.com/user-attachments/assets/4f27f2a1-c790-4a50-b9a1-c6d356ab4590






## 조원
- 유정훈 ( 메인 개발 ) 
- 최우성 ( 하드웨어 개발 )
- 성명훈 ( 이미지 평가 소프트웨어 개발 )
- 박재선 ( 사용자 웹 인터페이스 개발 )

