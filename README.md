# 공공 와이파이 검색 시스템

### 프로그램 소개
* 현재 위치를 조회해 근처의 공공 와이파이 정보를 얻을수 있는 시스템 입니다.
* Dynamic Web Project 로 구현한 서블릿 기반 웹 프로젝트입니다.
* 공공데이터포털의 `서울시 공공 와이파이 API` 를 사용합니다.

### 사용법
1. `와이파이 정보 가져오기` 를 눌러 API 로부터 데이터를 DB로 받아옵니다.
2. `내 위치 가져오기` 를 눌러 JS Geolocation 을 사용해 LAT,LNT 를 업데이트 합니다.
3. `근처 와이파이 보기` 를 눌러 현재 위치에서 가까운 순으로 와이파이 정보를 보여줍니다.
4. `위치 히스토리` 에서 조회한 정보 히스토리를 확인할 수 있습니다.
5. `북마크 그룹`(집,직장 등) 별로 자주 찾는 와이파이를 북마킹 할 수 있습니다.

### 문제 및 해결
* 처음 진행해본 웹 프로젝트라 이런저런 문제들을 많이 마주쳤는데  
  특히 폼 내용을 전달하거나 새로운 페이지로 이동할 때마다  
  서블릿을 이용해 처리하는 과정이 꽤나 복잡하다 느꼈고  
  또한 DB 요청시에도 직접 쿼리를 다 작성하는 방법밖에 없어서 힘들었습니다.  
  하지만 이후 프로젝트부터 스프링부트를 사용하며 JPA, JDBC 등의 개념을 배워  
  이런 부분들에 대해 많은 도움을 받았습니다.  
