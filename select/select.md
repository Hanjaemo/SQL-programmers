## 3월에 태어난 여성 회원 목록 출력하기
```sql
select member_id, member_name, gender, date_format(date_of_birth, '%Y-%m-%d')
from member_profile
where month(date_of_birth) = 3 and gender = 'W' and tlno is not null 
order by member_id
```
## 과일로 만든 아이스크림 고르기
```sql
select f.flavor
from first_half f, icecream_info i
where f.flavor = i.flavor and f.total_order > 3000 and i.ingredient_type = 'fruit_based'
order by f.total_order desc
```
## 12세 이하인 여자 환자 목록 출력하기
```sql
select pt_name, pt_no, gend_cd, age, if(tlno is null, 'NONE', tlno) as tlno
from patient
where age <= 12 and gend_cd = 'W'
order by age desc, pt_name asc
```
## 흉부외과 또는 일반외과 의사 목록 출력하기
```sql
select dr_name, dr_id, mcdp_cd, date_format(hire_ymd, '%Y-%m-%d')
from doctor
where mcdp_cd = 'CS' or mcdp_cd = 'gs'
order by hire_ymd desc, dr_name asc
```
## 평균 일일 대여 요금 구하기
```sql
select round(avg(daily_fee), 0) as average_fee
from car_rental_company_car
where car_type = 'SUV'
```
## 인기있는 아이스크림
```sql
select flavor
from first_half
order by total_order desc, shipment_id asc
```
## 서울에 위치한 식당 목록 출력하기
```sql

```
## 조건에 부합하는 중고거래 댓글 조회하기
```sql
select b.title, b.board_id, r.reply_id, r.writer_id, r.contents, date_format(r.created_date, '%Y-%m-%d') as created_date
from used_goods_board b, used_goods_reply r
where b.board_id = r.board_id and year(b.created_date) = 2022 and month(b.created_date) = 10
order by r.created_date asc, b.title
```
## 조건에 맞는 도서 리스트 출력하기
```sql

```
## 강원도에 위치한 생산공장 목록 출력하기
```sql

```
## 모든 레코드 조회하기
```sql

```
## 재구매가 일어난 상품과 회원 리스트 구하기
```sql

```
## 오프라인/온라인 판매 데이터 통합하기
```sql

```
## 역순 정렬하기
```sql

```
## 아픈 동물 찾기
```sql

```
## 어린 동물 찾기
```sql

```
## 동물의 아이디와 이름
```sql

```
## 여러 기준으로 정렬하기
```sql

```
## 상위 n개 레코드
```sql

```
## 조건에 맞는 회원수 구하기
```sql

```
