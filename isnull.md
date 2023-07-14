## 경기도에 위치한 식품창고 목록 출력하기
```sql
SELECT warehouse_id, warehouse_name, address, IFNULL(freezer_yn, 'N')
FROM food_warehouse
WHERE warehouse_name LIKE '경기도%'
ORDER BY warehouse_id
```
## 이름이 없는 동물의 아이디
```sql
select animal_id
from animal_ins 
where name is null
order by 1;
```
## 이름이 있는 동물의 아이디
```sql
select animal_id
from animal_ins 
where name is not null
order by 1;
```
## NULL 처리하기
```sql
select animal_type, ifnull(name, "No name"), sex_upon_intake
from animal_ins 
order by animal_id;
```
## 나이 정보가 없는 회원 수 구하기
```sql
```
