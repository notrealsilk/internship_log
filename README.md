# 💻 실습 준비 가이드

## 1️⃣ 자바 (Java) 설치

* 구글에서 `jdk-8u202-windows-x64.exe` 검색
* 또는 [Oracle Java SE 8 아카이브 다운로드 페이지](https://www.oracle.com/kr/java/technologies/javase/javase8-archive-downloads.html) 방문

---

## 2️⃣ KoNLPy 설치

> ⚠️ KoNLPy는 **Java 설치 후** 가능

### 방법 1) 공식 사이트 다운로드

[https://konlpy.org/ko/latest/install/#id2](https://konlpy.org/ko/latest/install/#id2)

### 방법 2) 명령어 설치

```bash
pip install konlpy
```

---

## 3️⃣ MySQL 설치

* [공식 다운로드 사이트](https://www.mysql.com/)
* [MySQL Tutorial 공식문서](https://www.mysqltutorial.org/)

---

## 4️⃣ 캔바 (Canva)

* **간트차트(Gantt Chart)** 제작 시 유용
  → 프로젝트 진행상황 보고자료용으로 활용 가능

---

## 5️⃣ UML Work

UML 다이어그램 작성 시 유용한 도구

---

# 🧭 Git 실습

> 명령어는 **cmd (콘솔창)** 에서 입력합니다.

### 1. 원격 레포지토리 생성

```bash
https://github.com/깃헙이름/레포지토리이름
```

### 2. 원격 ↔ 로컬 레포지토리 연결

```bash
git remote add origin https://github.com/깃헙이름/레포지토리이름
```

### 3. 현재 연결된 사용자 확인

```bash
git config --global user.email
git config --global user.name
```

### 4. 로컬 저장소 초기화

```bash
git init
```

### 5. 로컬 → 원격 업로드

```bash
git add .
git commit -m "커밋 메시지"
git push origin 브랜치이름
```

---

# 📊 간트차트 (Gantt Chart)

* **Canva**를 이용해 시각적으로 제작 가능
* 프로젝트 일정 및 진행상황 시각화에 적합

![간트차트 예시](src/gantt_chart.png)

---

# 🧩 UML

### 1.설치

```bash
brew install graphviz
```

### 2. 참고

[PlantUML 공식 사이트](https://plantuml.com/ko/)

> 간단한 텍스트를 이용해 멋진 UML 다이어그램을 만들 수 있는 오픈소스 도구입니다.

- puml 유용한 라이브러리
![UML 예시](src/puml.png)

- 정부 표준 프레임워크
[표준프레임워크 포털 eGovFrame](https://www.egovframe.go.kr/home/main.do)

[egovframework:dev4.3    [eGovFrame]](https://www.egovframe.go.kr/wiki/doku.php?id=egovframework:dev4.3)



---

# 🌐 HTML / CSS / JavaScript

* SPA(Single Page Application) 주요 프레임워크:

  * **Angular** (롯데)
  * **Vue.js** (삼성, KT)
  * **React**
  * **Svelte**
- Jquery

[jQuery](https://jquery.com/)

[ThemeRoller | jQuery Mobile](https://themeroller.jquerymobile.com/)

- Bootstrap

[Bootstrap 시작하기](https://getbootstrap.kr/docs/5.3/getting-started/introduction/)

- W3H

[W3Schools.com](https://www.w3schools.com/)

- html태그 : 웹브라우저에서 인식되는 언어
- TCP/IP : 인터넷 관련 통신 프로토콜
- http : 웹브라우저 통신 규약
- SMTP : 메일통신규약
- FTP : 파일 규약

### HTML이란?

HTML 태그는 웹브라우저에서 인식되는 언어입니다.

대소문자를 구분하지 않으며, 문장 끝에 세미콜론(;)을 사용하지 않습니다.

HTML은 태그 기반 언어로, <태그> 와 </태그> 형태로 구성됩니다.

🪶 개행(Line Break)

HTML은 자동으로 줄바꿈을 인식하지 않기 때문에 직접 개행 태그를 사용해야 합니다.

태그	설명	효과
<br>	한 줄 개행	Enter 한 번
<p>	문단 구분	2줄 개행

예시:

안녕하세요<br>
반갑습니다<p>HTML 공부 중입니다</p>

🔗 균형 태그 (Balanced Tags)

시작과 끝 태그가 한 쌍으로 존재해야 하는 태그입니다.

<a href="https://www.naver.com">네이버 사이트</a>

- 비균형 태그 (Unbalanced / Self-closing Tags)

닫는 태그가 없는 형태입니다.

<img src="images/sample.png">
<img src="images/sample.png" />
<image source="images/sample.png"></image>


<img> 태그는 닫는 태그 없이 사용 가능하며,
<image>는 <img>의 대체 표현으로도 쓰이지만 일반적이지 않습니다.

- 태그의 종류
구분	이름	설명
인라인 태그 (inline)	<a>, <span>, <img> 등	줄바꿈이 없는 태그 — 한 줄 안에서 이어짐
블록 태그 (block)	<div>, <p>, <h1> ~ <h6> 등	자동으로 줄바꿈이 포함된 태그

예시:

<p>이 문장은 블록 태그입니다.</p>
<span>이 문장은 인라인 태그입니다.</span>

---

# 🗃️ SQL

* 관계형 DB: **Oracle, MySQL, SQLite**
* NoSQL: **MongoDB, Firebase**

1. MySQL 서버 실행
```sql
brew services start mysql
```

2. MySQL 접속
```sql
# root 사용자로 접속 (-p : 비밀번호 입력)
mysql -u root -p
```

3. 기본 명령어
```sql
system cls;             -- 콘솔 화면 지우기
select sysdate();       -- 현재 시스템 날짜
select current_time();  -- 현재 시간
select now();           -- 현재 날짜와 시간
show databases;         -- 데이터베이스 목록 조회
```

4. 데이터베이스 생성 및 선택
```sql
create database google;
show databases;
use google;
```

5. 테이블 생성
```sql
create table test (
  code int(4) not null primary key,
  name varchar(10) not null
);
commit;
show tables;
desc test;
```

6. 데이터 삽입 (INSERT)
```sql
insert into test(code, name) values(2200, 'hong');
insert into test(code, name) values(7700, 'kim');
insert into test(code, name) values(8800, 'lee');
insert into test(code, name) values(9900, 'goo');
insert into test(code, name) values(1200, 'park');
insert into test(code, name) values(3300, 'choi');
commit;
```

7. 데이터 조회 (SELECT)
```sql
select * from test;


출력 예시:

+------+------+
| code | name |
+------+------+
| 1200 | park |
| 2200 | hong |
| 3300 | choi |
| 7700 | kim  |
| 8800 | lee  |
| 9900 | goo  |
+------+------+
6 rows in set (0.00 sec)
```

8. 데이터 추가 삽입 예시
```sql
insert into test(code, name) values(5600, 'abc');
```

9. 테이블 구조 추가 예시
```sql
alter table test add (wdate datetime default now());
```


설명:

ALTER TABLE : 기존 테이블 구조 변경

ADD : 새 컬럼 추가

wdate datetime default now() : 등록 시간(datetime)을 자동으로 현재 시간으로 설정

10. 데이터 개수 확인
```sql
select count(*) from test;
select count(*) as total from test;
```

```sql
count(*) : 전체 행(row) 개수를 조회
```

as total : 컬럼 이름을 별칭(alias)으로 표시

11. SQL 언어 구조 정리
| 구분  | 명칭                         | 주요 명령어                         | 설명                      |
| --- | -------------------------- | ------------------------------ | ----------------------- |
| DDL | Data Definition Language   | CREATE, DROP, ALTER            | 테이블 구조 정의 및 변경          |
| DML | Data Manipulation Language | INSERT, SELECT, DELETE, UPDATE | 데이터 조작 (등록, 수정, 삭제, 조회) |
| DCL | Data Control Language      | GRANT, REVOKE                  | 권한 부여 및 취소              |
| DTL | Data Transaction Language  | COMMIT, ROLLBACK               | 트랜잭션 적용 또는 취소           |

12. 테이블 컬럼 추가 실습

이미 test 테이블이 존재하므로 CREATE TABLE 재생성 금지

```sql
alter table test add (wdate datetime default now());
desc test;

insert into test(code, name) values(5600, 'abc');
select * from test;

alter table test add (hit int(4) default 0);
desc test;
```

13. DML 명령어 실습
(1) 데이터 등록
```sql
insert into test(code, name) values(7700, 'kim');
```

(2) 데이터 조회
```sql
select * from test;
select * from test where code > 5500;
select * from test where code = 7700;
select * from test where code < 3300;
```

주의:
SQL에서는 = 하나만 사용해야 함.
== 사용 시 오류 발생.

잘못된 예시
```sql
select * from test where code == 7700; -- 에러
```


올바른 예시
```sql
select * from test where code = 7700;
```

(3) 데이터 수정
```sql
update test set name='LG' where code=3300;
```


주의:
WHERE 절 없이 UPDATE를 실행하면 모든 행이 수정됨.
실수 시 ROLLBACK으로 복구 가능.

```sql
update test set name='LG';   -- 모든 행 변경
rollback;                    -- 변경 취소
```

(4) 데이터 삭제
```sql
delete from test where code=9900;
commit;
```

14. 트랜잭션 관리 (DTL)
명령어	설명
COMMIT	변경사항 적용
ROLLBACK	최근 변경사항 취소 (되돌리기)

예시:
```sql
update test set name='LG' where code=3300;
rollback;
```

15. DBA(관리자) 유의사항

DML 명령어(INSERT, UPDATE, DELETE)는 데이터에 직접 영향을 주므로
백업 및 트랜잭션 관리가 중요함

COMMIT 전에는 항상 SELECT로 결과 확인

WHERE 절이 없거나 잘못된 경우 전체 데이터 변경 위험 존재

---

# ⚙️ Backend

* **FastAPI**

---

# 🎨 Frontend

* **Flutter**

---
