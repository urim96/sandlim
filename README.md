 :four_leaf_clover:  SANDLIM
###### 산들림 : 여기저기 옮겨 다니면서 한 줄기씩 내리는 소나기.
<br><br>
## :blush: 프로젝트 소개 

'되어보자, 카페주인!'

'카페 하나 차려서 옆에 다같이 모여서 놀자'

'6개월 간의 노력, 짧게 느껴졌지만 두번의 계절이 바뀔 시간. 제각기 다른 삶을 살다가 여기에 모인 우리들의 앞으로의 시간 속에서 이 6개월을 뒤돌아 봤을때 '그때 좋았지' 하고 떠올릴 수 있는 기간이었으면 좋겠다는 기원를 담아,
산들림이라는 이름의 카페를 만들어보게 되었습니다. 
<br><br><br>

## :date: 개발 기간
- 2024.04.26 ~ 2024.05.23
- 인원 : 7명
<br><br><br>

## :bulb: 주요 기능
#### 일반 회원 기능
- 회원가입(전화번호 인증, 이메일 인증), 카카오/네이버 회원가입
- 로그인, 카카오/네이버 로그인
- 아이디찾기, 비밀번호 찾기
- 회원정보 수정
- 회원 탈퇴
- __나의 주문 내역 확인, 취소__
- 리뷰 작성
- __상품 리스트 조회__
- 장바구니 담기
- __주문(결제 API사용)__
#### 관리자 기능
- __상품 조회, 등록, 수정, 삭제__
- __주문 내역 조회__
- __주문 상태 변경__
- __결제 취소__
- 공지사항 조회, 작성, 수정, 삭제
- 리뷰 조회, 삭제
- 게시판 조회, 작성, 수정, 삭제
- 매출 통계
<br><br><br>

## :wrench: 사용 기술
![사용기술](https://github.com/urim96/urim96final/assets/157820470/18ebbdbe-988a-4fe1-8aa7-29fce689025e)
<br><br><br>
## :movie_camera: 프로젝트 결과
<br>

### :coffee: 메인 화면

![메인1](https://github.com/urim96/SANDLIMfinal/assets/157820470/79e3ee3a-d824-4d0f-b10f-760dd3db2bf9)

![메인2](https://github.com/urim96/SANDLIMfinal/assets/157820470/0fc50e85-fb95-4417-a46f-7355b0311300)
<br><br><br><br>
### :cake: 상품 페이지

- 사용자의 편리성을 위하여 스크롤 기능을 추가하였습니다.
- 검색 기능과 카테고리별 메뉴는 Ajax를 사용하여 페이지 리로드 없이 비동기 호출되도록 구현하였습니다. 
<br>

![스크롤](https://github.com/urim96/SANDLIMfinal/assets/157820470/c45df98b-c888-4749-91d6-d74a566e0841)

![검색기능](https://github.com/urim96/SANDLIMfinal/assets/157820470/d20edef0-5a54-4ccf-8044-c84b3e92019a)

![키워드](https://github.com/urim96/SANDLIMfinal/assets/157820470/49a8b249-c089-42e4-a546-c0e1b760700e)
<br><br><br><br>
## :star: 상품 페이지 반응형

- 다양한 기기, 화면에서도 렌더링 되도록 미디어 쿼리를 사용하여 반응형 웹 설계/구현을 하였습니다.

https://github.com/urim96/SANDLIMfinal/assets/157820470/6487c12a-2ff0-4f7f-bc4f-64f59b6d770d

<br><br><br><br>
### :money_with_wings: 결제

- 결제는 포트원 API를 사용하였습니다.
- https://developers.portone.io/docs/ko/pg/payment-gateway/danal?v=v1 참고
<br>

https://github.com/urim96/SANDLIMfinal/assets/157820470/2a9e0dc9-fd2d-4eae-8d82-dadbdd532a21

https://github.com/urim96/SANDLIMfinal/assets/157820470/8ee33a0b-1af9-4f00-96a1-0417c08557c7

<br><br><br><br>
### :page_with_curl: 나의 결제 내역 조회, 결제 취소

- 결제 내역은 진행중인 결제 내역과 전체기간 결제 내역 조회가 가능하며 주문확인중인 결제 건에 한하여 주문자가 직접 결제를 취소할 수 있도록 하였습니다.
<br>

https://github.com/urim96/SANDLIMfinal/assets/157820470/434efbf8-510a-4f02-b89f-6658df3bb3b6

<br><br><br><br>
### :bell: 관리자 : 주문 상태 변경 

- 새로운 주문이 접수되면 관리자는 주문 관리 페이지에서 주문 내역을 조회, 상태 변경, 결제 취소를 할 수 있습니다.
- 관리자가 주문 상태 변경 시 주문자의 주문 내역 페이지에서도 변경된 상태로 실시간 업데이트 됩니다.
- 관리자는 모든 주문 상태에서 취소가 가능합니다.
<br>

![상태변경](https://github.com/urim96/SANDLIMfinal/assets/157820470/451bd0a7-b23c-4bbf-ab3d-ae8f205f0776)

<br><br><br><br>
### :cookie: 관리자 : 상품 수정 / 삭제 

- 상품의 상세 정보를 수정할 수 있습니다.
- 이미지 파일 수정 시 기존 이미지와 새로운 이미지를 동시에 확인 할 수 있습니다.
- 상품 수정 페이지에서는 베스트 메뉴, 품절 메뉴, 판매 종료 등 상품의 상태를 변경 할 수 있습니다.
- 상품 삭제는 DELETE가 아닌 UPDATE 처리로 판매 종료 처리하여 사용자 페이지에서는 보이지 않고 관리자 페이지에서만 확인 가능합니다.
<br>

https://github.com/urim96/SANDLIMfinal/assets/157820470/0ae72a85-6b9e-44a0-a51c-be95f079bbdb

<br><br><br><br>
### :birthday: 관리자 : 상품 추가

- 새로운 상품 추가 시 이미지 업로드가 가능합니다.
<br>

https://github.com/urim96/SANDLIMfinal/assets/157820470/43a08b25-9205-494c-890c-9108fda14d04


<br><br><br><br>
상품 이미지 출처 : (주)더쉐프 텐퍼센트커피 / 영상 출처: 카페 나크타