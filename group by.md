## 자동차 대여 기록에서 대여중 / 대여 가능 여부 구분하기
```sql
```
## 카테고리 별 도서 판매량 집계하기
```sql
```
## 자동차 종류 별 특정 옵션이 포함된 자동차 수 구하기
```sql
```
## 진료과별 총 예약 횟수 출력하기
```sql
```
## 조건에 맞는 사용자와 총 거래금액 조회하기
```sql
```
## 식품분류별 가장 비싼 식품의 정보 조회하기
```sql
```
## 대여 횟수가 많은 자동차들의 월별 대여 횟수 구하기
```sql
```
## 저자 별 카테고리 별 매출액 집계하기
```sql
```
## 성분으로 구분한 아이스크림 총 주문량
```sql
```
## 즐겨찾기가 가장 많은 식당 정보 출력하기
```sql
```
## 고양이와 개는 몇 마리 있을까
```sql
select animal_type, count(animal_type)
from animal_ins
group by animal_type
order by animal_type
```
## 동명 동물 수 찾기
```sql
select name, count(name)
from animal_ins
group by name having count(name) >= 2
order by name
```
## 년, 월, 성별 별 상품 구매 회원 수 구하기
```sql
```
## 입양 시각 구하기(1)
```sql
select hour(datetime) as hour , count(1) as count
from animal_outs
group by 1 having hour between 9 and 20
order by 1
```
## 입양 시각 구하기(2)
```sql
```
## 가격대 별 상품 개수 구하기
```sql
```
