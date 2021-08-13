

# tp_2

# 팀프로젝트 2

## 조원 : 김민성(조장), 이세령, 김병헌, 최현수



### **21.08.12 프로젝트 2 회의록**

#### 오늘 과업

* 웹 구현
  * https://meet.google.com/exv-oiwb-yyz
  * : 민성, 병현
  * 홈페이지 / 프로젝트 소개 / 시각화 / 추천 강의
  * 로그인(회원가입) 후 HomePage로
* DB 구축
  * https://meet.google.com/zic-mfzr-rve
  * : 현수, 세령

#### 진행상황 공유 드라이브

* https://colab.research.google.com/drive/1VRvaA2MPfpJyzuIAc0RljlsHSyqWlokN#scrollTo=J9BI63St3WMz





### **21.08.11 프로젝트 2 회의록**

#### 기술과제

* 어떤 머신러닝 기법을 사용해야할지?
  * 독립변수(대학|어학성적|나이) -> 종속변수 (미취업, 취업 산업 분야) <다중 분류 - xgboost, lgbm, catboost, randomforest>
  * [브레인스토밍]이러한 산업군에 취업을 하려면 어떤 노력을 더 해야할지?
  * 종속변수에 가장 영향을 주는 독립변수를 하나 뽑아내는 과정 필요



* 특정산업군에 취업하기 위해서는 어떤 스펙이 좀더 필요한지? <<

* 유저가 특정 데이터셋을 입력해서 출력했을때 변수 중요도가 - 데이터에 박혀있다?

* 취업 방향? 회귀분석 / 군집을 나눠서 다시 군집을 분류

* 타겟 수치화 

* 어떤분야로 가는지/ 취업하냐마냐x/ (취업을 잘 하게 하기위해서 역량에 대한 분석)종속변수에 가장 영향을 미치는게


#### 변수 설정

* 독립변수
  * [1]학교 유형 : G181SCHOOL
  * [2] 전공 : G181MAJOR_N
  * [3] 졸업날짜 : G181GRADUY
  * [4] 연령 : G181AGE
  * [5] 인턴여부: G181A060
  * [6] 토익점수: G181I022
  * [7] (토스등급: G181I036)
  * [8] 총 취업 훈련 시간 : G181L016
  * [9] 졸업전 후 구직활동 경험 유무 : G181K001
  * [10] 자격증 개수: G181M002
* 종속변수
  * 현 직장(일자리) 종사상 지위 - G181A021
  * A3. 현 직장(일자리) 산업 대분류 CODE_10차 분류: g181a004_10





### **21.08.10 프로젝트 2 회의록**

* 변수 설정
  * 독립변수 : 노력해서 바꿀 수 있는 변수
    * 학교 유형: G181SCHOOL
    * 전공: G181MAJOR_N
    * 졸업날짜: 
    * 출생날짜: 
    * 인턴여부: G181A060
    * 토익점수: G181I022
    * (토스등급: G181I036)





### 3조 곰스 기획안 피드백

* 일단 또 PT 반칙이라고 하심.
* 딴생각 하셧대요. 비주얼이 너무 강해서 내용에 집중 못하게 됨.
* 데이터 베이스 활용에 대해 물어보심. 잔인함.  자격증 수료 -> 바뀌게 되나요?
* 시스템전체가 부정적인 상황 또는 부정적인 서비스 형태로 가게되면 안좋은 인식이 남음.
* 포지티브로 바꾸는게 좋을것 같음. 분석 자체는 좋은데 어떻게 활용해야하나.
* 잡코리아 사람인 등 -> 보인의 정보를 입력하여 맞춤 기업이 나오므로 좀 비슷하여, 거시기 한데... 라고 하심.
* 데이터를 활용하는것은 좋은데 그것을 가지고 분석을 하는 것은 취업이 되요 안되요 라는 극단적인 방향보다는, 어느쪽으로 취업을 추천한다라는 식으로
* ~~  분야로 갈수 있습니다 이렇게 되면, 나중에 잡코리아 인크루트 이런 사이트에서 웹크롤링을 통해서 본인이 이러이러한 회사로 갈 수 있다라는것을 나아가서 연동 및 구성할 수 있다.
* 결론: 프로젝트의 전체적인 방향이 네거티브한 쪽으로 갔다. 방향성을 다시한번 잡아봐라.
* 



![image-20210809153405889](../typora/image/image-20210809153405889.png)

![image-20210809153416884](../typora/image/image-20210809153416884.png)





### **21.08.09 프로젝트 2 회의록**

* 기술 과제
  * 사이트 로그인 구현
    * DB에 테이블이 3개 (회원정보 | 독립변수 | 종속변수)
  * 시나리오
    * 로그인(member_info 테이블)
    * 독립변수(독립변수 table에 입력) 입력
    * 종속변수(SELECT 보여지고 종속변수 테이블 저장) 확인
  * 독립변수 설정
    * supported (경제적 지원을 받는 여부)
      * O / X / 무응답
      * 월 지원 금액
      * 부모님 월 평균 소득
    * 대학관련
      * univ_type(전문대학, 4년제 대학, 교육대)
      * univ_major(졸업한 전공 계열)
      * univ_area(졸업 대학의 소재지)
    * 직장을 선택할 때 근로 소득의 중요도





### **:: 주말 과제**

* 부트 스트랩 골라오기 2개씩(각 로컬에 돌려보는 것 까지)

  현수님 

  *  https://html5up.net/editorial
  * https://themewagon.com/themes/free-responsive-html5-admin-dashboard-template-next-angular-8/

  민성님 
  병현님 
  세령님

  * https://startbootstrap.com/theme/creative
    https://themewagon.com/themes/free-bootstrap-5-html5-commercial-template-purple-buzz/

* 머신러닝 기법 골라오기 



### **21.08.06 프로젝트 2 회의록**

* 2차 프로젝트 진행 일정
  * 8/9 (월) 오후 4시에 테스트
  * 8/9 - 20 세미2차 프로젝트
  * 8/10 (화) 기획서 발표
  * 8/20 (금) 최종발표
  * 8/21 (토) 멘토링

* 시나리오
  * 김개똥, 4년제, 부모님 소득 연 2억, 인문 - > 취업을 할지 안할지
  * 디시전트리, 랜덤포레스트,
  * 부수적 : goms - 태블로로 시각화
  * 최종 : 마리아DB(T1 : 구직자 정보, T2 : goms) - 머신러닝 - 서버(파이썬 애니웨어) - 장고(웹 구현)

* 강의 리스트
  * https://www.inflearn.com/course/%ED%8C%8C%EC%9D%B4%EC%8D%AC-%EB%A8%B8%EC%8B%A0%EB%9F%AC%EB%8B%9D-%EC%99%84%EB%B2%BD%EA%B0%80%EC%9D%B4%EB%93%9C#curriculum]
  * (https://www.inflearn.com/course/파이썬-머신러닝-완벽가이드#curriculum)https://www.inflearn.com/course/%EC%BA%90%EA%B8%80-%EB%A8%B8%EC%8B%A0%EB%9F%AC%EB%8B%9D-%EC%9E%85%EB%AC%B8
  * 머신러닝 유튜브, 책 -> kaggle code vote수 titanic , 데이콘 (머신러닝,
  * 분류: [https://dacon.io/competitions/official/235713/overview/description

* 강사님 질문 리스트
  * 꼭 결과물이 웹 서비스 이어야 하는지?
    * 머신러닝 시스템을 어떻게 활용할 것인가 하는 아이디어를 내자는 것!
    * 고민을 해서 프로젝트 화 해야함. 현업....
    * 파이썬 애니웨어를 통해서 mysql을 받을 수 있음.
    * 마리아db, 머신러닝을 어떻게 엮어서…
    * 은행에서 대출을 하는데 모델에다 돌렸더니 연체할 수 있는 사람인지 아닌지여부가 나옴. 상수와 계수화가 만들어지면 군집으로 만들어냄.
    * 머신러닝을 가르쳐주실 예정….
    * 미래 해야할 프로젝트의 축소판
  * 관련 포트폴리오 예시 주세요!
    * 없음.
  * sk 플래닛 의 readme 작성법
    * 저





### **21.08.05 프로젝트 2 회의록**

* 자격증현수님 : 정처기
* 세령님 : 정처기병현님 : 정처기
* 민성님 : adsp, 정치기
* 빅분기 실기 사이트 : https://www.datamanim.com/dataset/03_dataq/main_p1.html





### **21.08.04 프로젝트 2 회의록**

* 이번 프로젝트의 주제 :
  * 마리아db - 장고 연동 - 머신러닝 - 웹 구현
    * 분과
      * DB 구축 분과
        * 마리아DB 구축 : DB모델링
        * {이것을 통해 무엇을 해야할지?}
      * 웹 분과
        * 장고 웹페이지를 구현
        * 보여지는 것!
      * 데이터 분과
        * 데이터 수집
        * 데이터 전처리
      * 머신러닝 분과
        * {우리는 무엇을 배울 것이며, 무엇을 하게 될 것인가?}





### **21.08.02 프로젝트 2 회의록**

* 머신러닝을 기반으로 주제 정하기

* 브레인스토밍
  * 취업 경로 조사 데이터[https://survey.keis.or.kr/goms/goms01.jsp**
    **](https://survey.keis.or.kr/goms/goms01.jsp)**![img](https://lh5.googleusercontent.com/DYzLkhLDUOpqqm4Gf04NT8AoHZASTSMLkFJd3e9lM7F6jYaqAH0XtcgkGQ2mjnDzfvNWH3DscAJNuhFJW4bk-sULxcGyfyLCoGMkXzGs-wn84LULxIKmgn3aiBiCUx3X6htJZj5N)**





### **21.07.30 프로젝트 2 회의록**

* 각자 이메일 주소
  * 민성님 : [msio900@gmail.com](mailto:msio900@gmail.com)
    *  31 데이터사이언스
    * 01049266036
    * 데이터 수집, 시각화(태블로), ppt
  * 세령님 : [leesa4350@gmail.com](mailto:leesa4350@gmail.com)
    *  24 통계학과
    * 카카오톡 ID : lla9
    * 데이터 전처리, 시각화 (플랏틀리), 데이터 분석
  * 병현님 : [kimqudgus@gmail.com](mailto:kimqudgus@gmail.com)
    *  27 전기전자학과
    * 카카오톡 ID : kimqudgus
    * ppt 제작, 장고 서버, 전처리 분석
  * 현수님 : [hakdjhakdj@gmail.com](mailto:hakdjhakdj@gmail.com)
    *  30 물리학과 물리학대학원
    *  TEL: 010-2969-9601 톡방
    * 코드 작성, 웹 크롤링, 웹 구현

* 주제 키워드 : 마리아DB - DB모델링 - 파이썬 하고 장고
