## 가격이 제일 비싼 식품의 정보 출력하기
```sql
```
## 가장 비싼 상품 구하기
```sql
select max(price) as max_price
from product
```
## 최댓값 구하기
```sql
select max(datetime) as '시간'
from animal_ins
```
## 최솟값 구하기
```sql
select min(datetime) as '시간'
from animal_ins
```
## 동물 수 구하기
```sql
select count(*) as count
from animal_ins
```
## 중복 제거하기
```sql
select count(distinct name) as count
from animal_ins
```
