
:warning: _Most of these examples were created 10+ years ago and are being kept here for reference purposes (tons of legacy code out there, right?). If you want to tackle any of these problems, you should first try looking for modern APIs on newer ABAP versions ([this](https://help.sap.com/http.svc/rc/abapdocu_752_index_htm/7.52/en-US/index.htm) is a good start)._

ABAPZombie-Code-Library
=======================

This repository contains all examples from on our website. 

If you need further information about any code, search for the appropriate post at www.abapzombie.com

Contact us for suggestions: contato@abapzombie.com

다음은 ABAPZombie-Code-Library-master/src 폴더 아래, 각 서브폴더별로 제공되는 ABAP 예제의 주요 로직을 요약한 내용입니다.


---

1. ABAP - Finding BADIs and User-Exits

표준 레포지토리 테이블(TSTC, TADIR, ENLFDIR 등)을 조회하여 시스템에 존재하는 BADI 구현체와 User-Exit 이름·위치를 자동으로 검색·목록화하는 로직입니다.


2. ABAP - Macros

반복되는 코드 패턴(예: 문자열 포맷팅, 변수 초기화 등)을 MACRO로 정의하고, 이를 호출해 가독성과 재사용성을 높이는 예제입니다.


3. ABAP - Parallel Processing

STARTING NEW TASK 또는 RFC in Background Task 기법을 이용해, 대량 데이터 처리·외부 시스템 호출 등 무거운 로직을 병렬로 실행하는 방법을 시연합니다.


4. ABAP - Performance Comparison

동일 작업(예: 내부 테이블 검색, 문자열 처리)을 여러 방법으로 구현한 뒤, STATS나 TIME 유틸리티를 이용해 실행 시간을 비교·측정하는 벤치마크 예제입니다.


5. ABAP - Project Pattern

대규모 ABAP 개발 프로젝트에서 권장되는 레이어드 아키텍처(Domain → Service → Repository 패턴 등) 구조를 간단히 구현해 보여 줍니다.


6. ABAP - RTTS

Runtime Type Services(CL_ABAP_TYPEDESCR, CL_ABAP_OBJECTDESCR 등)를 이용해

변수·구조체·테이블 타입을 동적으로 생성

런타임에 타입 정보를 조회·캐스팅

DDIC 기반·비DDIC 기반 예제를 모두 다룹니다.



7. ABAP - Removing Invalid Characters with Example

주어진 문자열에서 제어문자·특수문자 등 유효하지 않은 문자를 정규식(CL_ABAP_REGEX) 또는 TRANSLATE로 필터링해 제거하는 로직입니다.


8. ABAP - SORT tables using BINARY SEARCH (no SORT command)

내부 테이블을 SORT 문 없이 이진 검색 알고리즘으로 정렬·삽입하는 방법을 직접 구현한 예제입니다.


9. ABAP - Standard Exception Classes

CX_ROOT를 비롯한 표준 CX_… 예외 클래스를 사용해 Open SQL 에러, 런타임 에러 등을 TRY…CATCH 블록으로 처리하는 패턴을 보여 줍니다.


10. ABAP - TVARV Class and Example

TVARV 테이블(프로그램 파라미터 저장)에서 값을 조회·변환하는 전용 클래스 활용법을 예제로 제공합니다.


11. ABAP - Using OLE for Microsoft Word

OLE Automation을 통해 SAP GUI에서 Word 문서를 생성·편집하고, 텍스트를 쓰거나 서식을 지정하는 방법을 시연합니다.



---

12. ALV - ALV’s consistency check

CL_GUI_ALV_GRID 사용 시, 데이터 일관성(Consistency Check) 이벤트를 캡처하고 재검증 루틴을 실행하는 예제입니다.


13. ALV - Reusing Standard ALVs

SAP 표준 ALV(예: REUSE_ALV_GRID_DISPLAY)를 Z-Report 안에서 호출·확장하여, 개발자가 공통 레이아웃을 그대로 재사용하는 패턴입니다.



---

14. CRM BOL - Alert Modeler

CRM BOL API를 이용해 CRM Alert(경고) 객체를 생성·관리하는 로직. Alert Context 설정부터 Alert 생성까지 흐름을 보여 줍니다.


15. CRM BOL - Dynamic Query

BOL Query Builder(CL_CRM_BOL_QUERY_BUILDER)를 사용해, 사용자 입력에 따라 동적으로 쿼리 조건을 생성·실행하는 방법입니다.


16. CRM BOL - Get Entities

BOL Business Object Layer를 통해 CRM 엔티티(예: 비즈니스 파트너, 영업문서)를 프로그래밍 방식으로 조회·조작하는 예제입니다.


17. CRM BOL - Messages

CRM 메시지 프레임워크를 활용해 메시지 관리(읽기·쓰기·삭제) 기능을 BOL API로 구현하는 패턴입니다.


18. CRM BOL - Relationship

BOL 엔티티 간 관계(Relationship) 를 설정·탐색하는 로직으로, 예를 들어 판매문서와 파트너 사이를 연결·분리하는 방법을 보여 줍니다.



---

19. Security - Dynamic Code Generation

런타임에 소스코드를 문자열로 생성해 EVAL(동적 실행)하거나 메모리에 저장하는 방식으로, 보안성·검증 절차를 함께 설명합니다.


20. Security - Kernel Calls

CALL FUNCTION 'SAPGUI_CREATE' 등 커널 레벨 함수를 직접 호출해 저수준 시스템 자원을 사용하는 예제를 담고 있습니다.


21. Security - OS Commands

SYSTEM 호출을 통해 운영체제 명령(파일 복사·디렉토리 조회 등)을 실행하고, 결과를 ABAP 변수로 받아오는 방법을 시연합니다.


22. Security - Virus Scan Interface

바이러스 스캔 API(예: SCAN_ATTACH)를 호출해 파일 첨부 전후에 악성코드 여부를 검사하는 보안 연동 예제입니다.



---

23. Selection Screen - Buttons

SELECTION-SCREEN에 사용자 정의 버튼을 추가하고, 클릭 이벤트를 AT SELECTION-SCREEN에서 처리하는 방법을 예시로 보여 줍니다.


24. Selection Screen - Hide Elements

특정 조건(예: 사용자 권한)에 따라 파라미터·옵션을 동적으로 ON/OFF 하거나 숨김 처리하는 로직입니다.


25. Selection Screen - New Screen

SUBSCREEN 또는 SELECTION-SCREEN BEGIN OF SCREEN을 이용해 기존 Selection Screen 위에 추가 영역을 생성하는 방법입니다.


26. Selection Screen - Tabstrip

Tabstrip 컨트롤을 Selection Screen에 구현해, 탭별로 서로 다른 입력 필드를 그룹화하는 예제입니다.


27. Selection Screen - Useful Stuff

다양한 유용 기능(텍스트 포맷, 위치 지정, 그룹 헤더/푸터, INPUT 검증 등)을 한 곳에 모아 놓은 실용 예제 모음입니다.



---

28. Selects - Dynamic Selection

동적 WHERE절(SELECT … WHERE (lv_cond)) 작성법과, SELECT-OPTIONS로 받은 값을 기반으로 쿼리 조건을 프로그램 실행 중에 조립하는 방법을 다룹니다.


29. Selects - Testing WHERE clauses

다양한 WHERE 절 조합(AND/OR, 괄호, LIKE 등)을 테스트 루틴으로 자동 생성·검증해 보는 예제입니다.



---

30. Webdynpro - Dynamic MIME content from AS Cache

Webdynpro 컴포넌트에서 MIME 객체를 로드해, 애플리케이션 서버 캐시 내의 파일을 동적으로 사용자에게 전송하는 예제입니다.


31. Webdynpro - Get URL

Webdynpro 컨텍스트에서 외부 URL(서비스 엔드포인트 등) 정보를 읽어 와, HTTP 호출 또는 링크 생성에 활용하는 방법입니다。



---

각 폴더의 예제 코드를 참고하시면, ABAP의 다양한 테크닉(성능 최적화·보안·UI·CRM 연동·Webdynpro 등)을 실제 업무에 그대로 적용해 볼 수 있습니다. 필요하신 주제의 코드를 더 깊이 분석하거나, 활용 방안을 구체적으로 알고 싶으시면 언제든 말씀해 주세요!

