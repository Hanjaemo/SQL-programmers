## 자동차 대여 기록 별 대여 금액 구하기
```sql
```
## 자동차 평균 대여 기간 구하기
```sql
```
## 자동차 대여 기록에서 장기/단기 대여 구분하기
```sql
```
## 특정 옵션이 포함된 자동차 리스트 구하기
```sql
```
## 조건에 맞는 사용자 정보 조회하기
```sql
```
## 조회수가 가장 많은 중고거래 게시판의 첨부파일 조회하기
```sql
```
## 취소되지 않은 진료 예약 조회하기
```sql
```
## 조건별로 분류하여 주문상태 출력하기
```sql
```
## 조건에 부합하는 중고거래 상태 조회하기
```sql
```
## 대여 기록이 존재하는 자동차 리스트 구하기
```sql
```
## 루시와 엘라 찾기
```sql
select animal_id, name, sex_upon_intake
from animal_ins
where name in ('Lucy', 'Ella', 'Pickle', 'Rogan', 'Sabrina', 'Mitty')
```
## 이름에 el이 들어가는 동물 찾기
```sql
select animal_id, name
from animal_ins
where name like '%el%' and animal_type = 'Dog'
order by name
```
## 중성화 여부 파악하기
```sql
select animal_id, name, if (sex_upon_intake like '%Neutered%' or sex_upon_intake like '%Spayed%', 'O', 'X')
from animal_ins
order by animal_id
```
## 오랜 기간 보호한 동물(2)
```sql
select o.animal_id, o.name
from animal_outs o join animal_ins i on o.animal_id = i.animal_id
order by datediff(o.datetime, i.datetime) desc
limit 2
```
## DATETIME에서 DATE로 형 변환
```sql
```
## 카테고리 별 상품 개수 구하기
```sql
```
