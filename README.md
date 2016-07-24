# table change management (english)

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


# 테이블 변경관리 (한국어)

DB 변경을 위한 DDL 구문을 만들어주는 VBA macro가 포함된 엑셀 파일

업무에서 이 도구를 사용하려면 아래 설명을 먼저 일고 사용하시기 바랍니다.

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
