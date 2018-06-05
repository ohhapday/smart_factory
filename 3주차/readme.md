# NEXT 공장 자동화
## 공장 자동화 (Automatic Factory)
#### 1. 정의
  - 물류센터나 공장 내에서 로봇이나 인공지능, 드론 등을 통해 사람을 줄이고 생산성을 높이는 것
  - 제어 시스템과 다른 정보기술을 조화롭게 사용하여 산업 기계류와 공정을 제어, 사람이 관여할 필요를 줄이는 것이다.
#### 2. 자동화 규모
LEVEL     | 영역     | 정의 | 시스템
--------| ------- | ----| -----:
ERP급 | 휴먼     | **전사적** 자원 관리   |  ERP, SAP
MES급 | 휴먼     | 통합 **생산관리** 시스템   |  MES, LIMS
SCADA급 | 휴먼   | 감시 제어 및 **데이터** 취득  | SCADA, DCS
PLC급 | 머신     | 자동제어 및 감시  | PLC, DCS  
Sensors급 | 머신 | 외부상태 수집  | Sensors, Hardware  

* HMI: Human-Machine Interface
  ![aa](http://www.addixa.net/wp-content/uploads/2012/11/Piramide_Ingles.png)

## 스마트 팩토리 (Smart Factory)
#### 1. 정의
  - 기존 자동화된 공장에 ict(IT)기술을 접목
  - ~~스마트 팩토리는 기획, 설계, 생산, 유통, 판매 등 전 생산과정을 정보통신기술(ICT)로 통합해 최소의 비용과 시간으로 고객 맞춤형 제품을 생산하는 진화된 공장을 의미~~ <-- ERP급에만 해당
#### 2. 사례(가칭)
  - Sensors급
      - MQTT 송출 가능 센서들의 집합
      - 스마트 농장의 센서들
  - PLC급
      - 스프링쿨러 제어와 화재위치를 무선랜을 통해 알려 주는 화재경보 센서
  - SCADA급
      - 콘크리트에 Sensor를 묻어 데이터 취득
      - 스마트 농장의 데이터 집계 서버
      - 호퍼 시스템
  - MES급
      - 지멘스 - 설비에 센서를 부착해 기계 이상을 감지. 공정 데이터를 분석해 공장 최적화 유지
      - [이마트 김포 물류센터](http://clomag.co.kr/article/2616)
  - ERP급
      - [노빌리아](https://blog.naver.com/yuhyojong/221012478167) - 고객 맞춤형 대량생산
      - 아마존 무인편의점(유통 자동화)
<br />

## 공장 자동화와 스마트 팩토리 비교
** 가장 중요한 차이는 데이터의 흐름에 iCT기술이 포함되는지 여부**
  1. 수집
    - 센서를 통한 디지털 데이터
  2. 전송
    - iCT 프로토콜로 전송
  3. 저장
    - DB등에 디지털로 저장
  4. 분석
    - 빅데이터를 통한 분석
  5. 판매, 판촉
    - 판매 및 판촉에 분석자료 활용
  6. 생산계획
    - 판매/판촉 분석으로 통해 자동으로 생산계획 수립

----
##### 현재 카스의 현실적인 목표: SCADA급
##### 향후 지향 목표: MES급
----

## 국내 스마트 팩토리 현황

#### 1. 구현 현황
기초  | 중간1     | 중간2 | 고도화
------| ------- | ----| -----:
SCADA급 | SCADA급 | MES급   |  ERP급

![스마트 팩토리 구현 정도](https://cdn.steemitimages.com/0x0/https://steemitimages.com/DQmeCadUKFHHDNZYEmzjGGFSJK6tacecqoFSWCGyByxGN5a/%EC%8A%A4%EB%A7%88%ED%8A%B8%20%EA%B3%B5%EC%9E%A5%20%EA%B5%AC%ED%98%84%20%EC%A0%95%EB%8F%84%20%EC%8A%A4%EB%A7%88%ED%8A%B8%EA%B3%B5%EC%9E%A5%EC%B6%94%EC%A7%84%EB%8B%A8%20%EA%B8%B0%EC%A4%80%20%EC%82%B0%EC%97%85%ED%86%B5%EC%83%81%EC%9E%90%EC%9B%90%EB%B6%80.png)

#### 2. 분류 사례
산업통상 자원부 [링크](https://steemit.com/kr/@clutho/gj5bz-smart-factory)
![스마트 팩토리 수준 총괄도](https://steemitimages.com/DQmTVP51VrxxLSv2pfDSg4owPJYkvTYZAfr6KFT6in7GDwe/%EC%8A%A4%EB%A7%88%ED%8A%B8%20%ED%8C%A9%ED%86%A0%EB%A6%AC%20%EB%8B%A8%EA%B3%84%EB%B3%84%20%EC%88%98%EC%A4%80%20%EC%B4%9D%EA%B4%84%EB%8F%84.png)

#### 3. 삼성 맞춤형 지원 프로그램
[삼성전자 경북](https://news.samsung.com/kr/%EC%82%BC%EC%84%B1%EC%A0%84%EC%9E%90-%EB%8C%80%EA%B5%AC%EA%B2%BD%EB%B6%81-%EA%B2%BD%EC%A0%9C%EC%97%90-%EB%8F%9B-%EB%8B%AC%EB%8B%A4-%EC%A0%9C%EC%A1%B0-%ED%98%81%EC%8B%A0%EC%9C%BC%EB%A1%9C-%EC%B0%BD): 구미공단 대상
![삼성 맞춤형 지원 프로그램](https://news.samsung.com/kr/wp-content/uploads/2015/08/%EA%B2%BD%EB%B6%81%EC%8A%A4%EB%A7%88%ED%8A%B8%ED%8C%A9%ED%86%A0%EB%A6%AC_%ED%91%9C1.jpg)

## 도출 제안
#### 1. 스마트 팩토리 정의
  - 팩토리보다 상위의 개념 필요
    - 아마존 무인 편의점
    - 유통물품의 초이력
  - 외부 마케팅 용어로써의 "스마트 팩토리"
  - 사내 내부적으로 새로운 용어 필요

#### 2. 분류 쳬계 정의
  1. 카스 분류 체계 정의
  2. 누구나 납득할 수 있는
  3. 카스가 주도하는 한국형 스마트 팩토리 분류 체계로 홍보

#### 3. 체계적인 홍보 계획
  - 분류체계에 따른 영업사례의 수집
  - 홈페이지등 스마트팩토리 상담창구 마련
  - 뉴스, 홍보, 판촉 계획 산출

#### 4. 시행사, 시공사
  - 할 수 있는 분야는 시공사의 역할
  - 할 수 없는 분야는 시행사의 역할
    - 할 수 있게끔 도급업체의 노하우 수집 요망
  - 할 수 있는/없는 산업분야 혹은 프로젝트 구분


## 참고자료
[LG CNS 자료](http://blog.lgcns.com/723)
[어드벤텍](http://select.advantech.com/%EC%96%B4%EB%93%9C%EB%B0%B4%ED%85%8D-%EC%8A%A4%EB%A7%88%ED%8A%B8%ED%8C%A9%ED%86%A0%EB%A6%AC-%EC%86%94%EB%A3%A8%EC%85%98/)
