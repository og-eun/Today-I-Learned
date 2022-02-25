# NoSQL

[Using MongoDB with Morphia](https://web.obsidianscheduler.com/using-mongodb-with-morphia/)

[RDBMS의 한계와 NoSQL을 사용하는 이유 (2) RDBMS의 한계, 트랜잭션](https://sujl95.tistory.com/82)

### Scheduler 에 어떤 DB 가 좋을까에 대해 생각해 봤습니다.

### RDB는 다들 알고 계시니까 NoSQL 에 대해 알아봤습니당.

### NoSQL 이 사용 사례

- 전자 상거래 플랫폼
- 메세지 저장
- 추천 서비스 등...

### NoSQL 장점

- 유연성 : 스키마 선언 없이 필드의 추가 및 삭제가 **자유로운 Schema-less 구조를 가지고 있다.**
- 확장성 : 스케일 아웃에 의한 **서버 확장 용이하다.**
- 고성능 : 대용량 데이터를 처리하는 **성능**이 뛰어나다.
- 가용성 : 여러 대의 백업 서버 구성이 가능하여 장애 발생 시에도 **무중단 서비스 가능하다.**
- 테이블 간 join 기능이 없다. (aggregate 로 대체 .. )

### NoSQL 단점

- 데이터베이스 일관성 약하다.
- key값에 대한 입출력만 지원한다.
- 스키마가 정해져 있지 않아, 데이터에 대한 규격화가 없다.
- 데이터가 여러 컬렉션에 중복되어 있어서 데이터를 **UPDATE 하는 경우 모든 컬렉션에서 수행**해야하기 때문에 느리다.
- 데이터 중복으로 인한 수정 작업의 번거롭다.
- 데이터 처리 완결성 (Transaction ACID) 을 보장하지 않다.

### NoSQL 목적

- 초고용량 데이터 처리 시 성능을 향상시키기 위해 !
- 비 관계형 데이터, 비 구조적 데이터를 활용하기 위해 !

### NoSQL 종류

- Key - Value DB
ex) Redis
- Document DB : Json, xml 형식과 같은 Collection 데이터 모텔 구조.
ex) MongoDB
- ~~Graph DB~~
- ~~Wide Columnar Store~~

### **스케줄러 DB........... NoSQL 이라면..?**

- 테이블의 형태가 간단합니다.
- 조인 연산이 없음 → 빠른 읽기 연산이 가능합니다.
- Rule 을 구성하는 요소 (모임 유형, 타겟 유형 등 .. ) 가 추가되거나 변경될 때 NoSQL 이면 커버가 됩니다.
- RDBMS 를 사용하다가 데이터가 많이 쌓이고, 어드민을 사용하는 크루가 원하는 검색 조건이 변경되거나 스케줄러에서 생성되는 구성 요소가 변경될 때 NoSQL 로 변환하려면 시도할 엄두도 안 날 수도..
- ObjectId 라는 Unique 한 값으로 Transaction ID를 대체할 수 있습니다.

***NoSQL 어ㄸㅐ요??....!??!?!?!***