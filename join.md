## 조건에 맞는 도서와 저자 리스트 출력하기
```sql
select b.book_id, a.author_name, date_format(b.published_date, '%Y-%m-%d') as published_date
from book b join author a on b.author_id = a.author_id
where b.category = '경제'
order by b.published_date
```
## 특정 기간동안 대여 가능한 자동차들의 대여비용 구하기
```sql
```
## 5월 식품들의 총매출 조회하기
```sql
```
## 주문량이 많은 아이스크림들 조회하기
```sql
```
## 그룹별 조건에 맞는 식당 목록 출력하기
```sql
```
## 없어진 기록 찾기
```sql
select o.animal_id, o.name
from animal_outs o left join animal_ins i on o.animal_id = i.animal_id
where i.animal_id is null
order by o.animal_id
```
## 있었는데요 없었습니다
```sql
select o.animal_id, o.name
from animal_outs o join animal_ins i on o.animal_id = i.animal_id
where o.datetime < i.datetime
order by i.datetime
```
## 오랜 기간 보호한 동물(1)
```sql
select i.name, i.datetime
from animal_ins i left join animal_outs o on i.animal_id = o.animal_id
where o.animal_id is null
order by i.datetime
limit 3
```
## 보호소에서 중성화한 동물
```sql
```
## 상품 별 오프라인 매출 구하기
```sql
```
## 상품을 구매한 회원 비율 구하기
```sql
```
