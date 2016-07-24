# 테이블 변경관리 (한국어)

이 도구는 DB 변경을 위한 DDL 구문을 만들어주는 VBA macro가 포함된 엑셀 파일이다.

업무에서 이 도구를 사용하려면 아래 설명을 먼저 읽고 사용할 것을 권장한다.

## 목표

윈도우즈에서 엑셀에 정의한 테이블 설계 내용과 실제 DB를 비교하여 변경에 필요한 DDL문과 DML문을 만들어낸다.

DDL문 실행은 작업자가 DB에 접속해서 직접(수작업으로) 실행한다.

## 구성 이해

3개 파일이 있습니다.

* DDL을 만들어내는 VBA가 포함된 엑셀 파일
* 테이블 설계가 포함된 엑셀 파일
* 테이블 변경 요청이 포함된 엑셀 파일

## 선행요건

ODBC 드라이버를 이용하므로 목표 DBMS에 적합한 ODBC 드라이버가 미리 설치 돼 있어야 한다.

## 사용법

### 테이블 설계서 작성

* 작업 주체: 설계자
* 엑셀 내에 있는 "시트이름", "필드 이름", "필드 위치"를 변경하면 안 된다.
* 엑셀 내에 있는 포멧을 유지하고, 원해는 내용에 맞춰서 각 시트 안에 내용을 작성한다. 
* 테이블목록
* 테이블정의
* 인덱스정의
* reference정의

### 변경 요청서 작성

* 작업 주체: 설계자
* 반영할 내용은 "테이블 설계서"에 먼저 작성 돼 있어야 한다.
* 반영하고 싶은 항목[테이블/컬럼/인덱스/reference]에 따라 해당 시트에 내용을 작성한다. 회색으로 표시된 점검결과,점검자,점검일,개발반영일,운영반영일에는 아무 내용도 적지 않는다.
* 테이블변경요청
* 컬럼변경요청
* 인덱스변경요청
* reference변경요청

### 변경 작업 실행

* 작업 주체: DBA 혹은 변경담당자 
* 비교 대상이 될 DB 정보를 입력한다.
* "테이블 설계서" 및 "변경요청서"의 경로를 입력한다.
* DDL이 출력되서 나올 파일의 경로를 입력한다. DDL 구문이 길기 때문에 별도의 텍스트 파일에 소스가 출력되서 나오게 하는 것이다.
* 변경 내용을 반영하고 싶은 항목[테이블/컬럼/인덱스/reference]에 따라 해당 작업 버튼을 클릭해서 DDL 소스가 나오도록 한다.
* 출력된 결과를 이용해서 DB에 변경내용을 반영한다.

# table change management (english: I will write later.)

Excel file that contains the VBA macro to create DDL statements for chaning DB.

If you want to use this tool in your work, If you want to use this tool in your work, read the instructions below first.

## Goal

It compare table design in excel file and DB, and creates DML and DML.

The generated DDL is the worker must be run manually.

## Understanding configuration

There are three files.

* Excel file that contains the VBA for creating DDL
* Excel file that contains tables design
* Excel file that contains table change requests

## Precedence

ODBC driver should have been installed in Windows.
