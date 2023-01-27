# 키친포스

## 요구 사항

### 상품

- 상품을 등록할 수 있다.
- 상품의 가격이 올바르지 않으면 등록할 수 없다.
    - 상품의 가격은 0원 이상이어야 한다.
- 상품의 이름이 올바르지 않으면 등록할 수 없다.
    - 상품의 이름에는 비속어가 포함될 수 없다.
- 상품의 가격을 변경할 수 있다.
- 상품의 가격이 올바르지 않으면 변경할 수 없다.
    - 상품의 가격은 0원 이상이어야 한다.
- 상품의 가격이 변경될 때 메뉴의 가격이 메뉴에 속한 상품 금액의 합보다 크면 메뉴가 숨겨진다.
- 상품의 목록을 조회할 수 있다.

### 메뉴 그룹

- 메뉴 그룹을 등록할 수 있다.
- 메뉴 그룹의 이름이 올바르지 않으면 등록할 수 없다.
    - 메뉴 그룹의 이름은 비워 둘 수 없다.
- 메뉴 그룹의 목록을 조회할 수 있다.

### 메뉴

- 1 개 이상의 등록된 상품으로 메뉴를 등록할 수 있다.
- 상품이 없으면 등록할 수 없다.
- 메뉴에 속한 상품의 수량은 0 이상이어야 한다.
- 메뉴의 가격이 올바르지 않으면 등록할 수 없다.
    - 메뉴의 가격은 0원 이상이어야 한다.
- 메뉴에 속한 상품 금액의 합은 메뉴의 가격보다 크거나 같아야 한다.
- 메뉴는 특정 메뉴 그룹에 속해야 한다.
- 메뉴의 이름이 올바르지 않으면 등록할 수 없다.
    - 메뉴의 이름에는 비속어가 포함될 수 없다.
- 메뉴의 가격을 변경할 수 있다.
- 메뉴의 가격이 올바르지 않으면 변경할 수 없다.
    - 메뉴의 가격은 0원 이상이어야 한다.
- 메뉴에 속한 상품 금액의 합은 메뉴의 가격보다 크거나 같아야 한다.
- 메뉴를 노출할 수 있다.
- 메뉴의 가격이 메뉴에 속한 상품 금액의 합보다 높을 경우 메뉴를 노출할 수 없다.
- 메뉴를 숨길 수 있다.
- 메뉴의 목록을 조회할 수 있다.

### 주문 테이블

- 주문 테이블을 등록할 수 있다.
- 주문 테이블의 이름이 올바르지 않으면 등록할 수 없다.
    - 주문 테이블의 이름은 비워 둘 수 없다.
- 빈 테이블을 해지할 수 있다.
- 빈 테이블로 설정할 수 있다.
- 완료되지 않은 주문이 있는 주문 테이블은 빈 테이블로 설정할 수 없다.
- 방문한 손님 수를 변경할 수 있다.
- 방문한 손님 수가 올바르지 않으면 변경할 수 없다.
    - 방문한 손님 수는 0 이상이어야 한다.
- 빈 테이블은 방문한 손님 수를 변경할 수 없다.
- 주문 테이블의 목록을 조회할 수 있다.

### 주문

- 1개 이상의 등록된 메뉴로 배달 주문을 등록할 수 있다.
- 1개 이상의 등록된 메뉴로 포장 주문을 등록할 수 있다.
- 1개 이상의 등록된 메뉴로 매장 주문을 등록할 수 있다.
- 주문 유형이 올바르지 않으면 등록할 수 없다.
- 메뉴가 없으면 등록할 수 없다.
- 매장 주문은 주문 항목의 수량이 0 미만일 수 있다.
- 매장 주문을 제외한 주문의 경우 주문 항목의 수량은 0 이상이어야 한다.
- 배달 주소가 올바르지 않으면 배달 주문을 등록할 수 없다.
    - 배달 주소는 비워 둘 수 없다.
- 빈 테이블에는 매장 주문을 등록할 수 없다.
- 숨겨진 메뉴는 주문할 수 없다.
- 주문한 메뉴의 가격은 실제 메뉴 가격과 일치해야 한다.
- 주문을 접수한다.
- 접수 대기 중인 주문만 접수할 수 있다.
- 배달 주문을 접수되면 배달 대행사를 호출한다.
- 주문을 서빙한다.
- 접수된 주문만 서빙할 수 있다.
- 주문을 배달한다.
- 배달 주문만 배달할 수 있다.
- 서빙된 주문만 배달할 수 있다.
- 주문을 배달 완료한다.
- 배달 중인 주문만 배달 완료할 수 있다.
- 주문을 완료한다.
- 배달 주문의 경우 배달 완료된 주문만 완료할 수 있다.
- 포장 및 매장 주문의 경우 서빙된 주문만 완료할 수 있다.
- 주문 테이블의 모든 매장 주문이 완료되면 빈 테이블로 설정한다.
- 완료되지 않은 매장 주문이 있는 주문 테이블은 빈 테이블로 설정하지 않는다.
- 주문 목록을 조회할 수 있다.

## 유비쿼터스 언어

### 상품
| 한글명 | 영문명 | 설명 |
| --- | --- | --- |
| **상품** | Product | 식당에서 판매하는 음식, 음료를 지칭 |
| **이름** | Name | 상품 이름을 지정한다. 비속어는 안된다.  |
| **가격** | Price | 상품의 판매가격. 0원 이상 입력받는다. |
| 등록 | Register | 새로운 상품을 등록한다. |
| 가격 변경 | Change Price | 상품의 가격을 변경한다. 0원 이상 입력받는다. |


### 메뉴그룹
| 한글명 | 영문명 | 설명 |
|-----| --- | --- |
| 메뉴 그룹 | Menu Group | 고객에게 보여지는 메뉴그룹 목록이다. ex)한식, 일식, 중식, 점심특가 |
| **이름**  | Name | 메뉴 그룹 이름을 지정한다. | 
| 등록  | Register | 새로운 메뉴그룹을 등록한다. | 

### 메뉴
| 한글명 | 영문명 | 설명 | 
| --- | --- | --- |
| 메뉴 | Menu | 고객이 보는 메뉴다 |
| **이름** | Name | 메뉴 이름이다. 비속어는 안된다. |
| **가격** | Price | 메뉴의 가격이다. 해당 메뉴에 포함된 상품들의 가격을 초과할 수 없다. |
| **메뉴 상품** | Menu Product | 메뉴에 포함되는 상품이다. |
| 등록 | Register | 새로운 메뉴를 등록한다. |
| 공개 | Display | 정상적으로 판매중인 메뉴다. |
| 비공개 | Hide | 모종의 이유(매진)로 메뉴를 숨긴다. |
| 가격 변경 | Change Price | 메뉴의 가격을 변경한다. 0원 이상 입력받는다. 상품들의 가격을 초과할 수 없다. |


### 주문 테이블
| 한글명 | 영문명 | 설명 |
| --- | --- | --- |
| **주문** 테이블 | Order Table | 매장 테이블이다. |
| **이름** | Name | 테이블 이름으로 주로 1번, 2번, 3번 형식으로 사용한다. |
| **고객** 인원 | Guests | 테이블에 앉는 고객 인원이다. |  
| 자리 안내 | Sit | 고객이 테이블을 배정받고 앉았다. |  
| 테이블 정리 | Clear | 고객이 떠난 테이블을 정리한다. | 
| 인원 변경 | Change Guests | 테이블의 고객 인원을 변경한다. 고객이 있는 테이블만 변경이 가능하다. |

### 주문
| 한글명 | 영문명 | 설명 |
| --- | --- | --- |
| 주문 | Order | 고객이 메뉴를 주문한다. |
| **주문 유형** | Order Type | 주문의 유형은 배달, 포장, 매장내 식사로 나눠진다. |
| 매장내 식사 | Eat In | 매장내 식사 주문건이다. | 
| 포장 | Take Out | 포장 주문건이다. |
| 배달 | Delivery | 배달 주문건이다. |
| **주문 상태** | Order Status | 주문 상황을 표시한다.  <br/>매장내 식사와 포장은 대기 -> 접수 -> 제공 -> 완료로 진행된다.<br/>배달 주문은 대기 -> 접수 -> 제공 -> 배달중 -> 배달됨 -> 완료로 진행한다.|
| 대기 | Waiting | 주문 접수를 기다리고 있다. |
| 접수 | Accepted | 주문이 접수되었다. |
| 제공 | Served | 주문 메뉴를 제공한다. |
| 배달중 | Delivering | 주문을 배달중이다. |
| 배달됨 | Delivered | 주문이 고객에게 배달되었다. |  
| 완료 | Completed | 주문이 완료되었다. |
| **주문 메뉴** | Order Line Item | 주문받은 메뉴 내역이다. |
| **주문 시각** | Order Date | 주문이 들어온 시각이다. |
| **배송 주소** | Delivery Address | 메뉴를 받을 주소다 |
| **배달 기사** | Delivery Rider | 배달 주문을 전달하는 배달 기사를 요청한다. 기사에게 배달 주문 정보(가격, 주소)를 전달한다. |
| **주문 테이블** | Order Table | 주문이 들어온 테이블 번호다. | 


## 모델링
[![](https://mermaid.ink/img/pako:eNqtldFq2zAUhl_F6Lp9gdyNmZVStoVml4ah2aeZILaDLA9CGtjWtWysF2PLYLAEVgqDjl5kpXQe9Ili5R0mybasxHa9wXRhx9J3LP3_OSceIzf0AHUQUJvgPsW-E1hidGnoxS6zDg-3t8Ox9RCCuJjqWG4YMEyCaB0dZ49ykIAZK7u21d2zHMRvpsvFy6f86NXq49td20FWGRExSoJ-EfEI-yAmRYhi0x_Hd8BdSlwoYbHF8urCQSXuYQbWPvSJiMOMhIEtJ_R50k8_07M5n9_y97MibJLdpOwdGsZD04eKASVVtUCvbZiQXkzTd9fLX0l6_ltaURGnA3Mv1HCQGadsaZOZ2dimVOlqz7XC6kXW6mtUphOccRtKDFAnNxf-n5JbJq65ev9S1b_Vut77MfWAPsHPBlD4rmYqxWVw1SMai2rX1fEpn1-nybTWeAVq5zUrr9_f1EhS_E4MEYvW-YR__WAqUkVWnnZNUGPHtFPZyxpUF0bnDzVyM3NGQ7hv511wfpteJnz2bfXlcxPfY5jFkYjQuMjg0Wzt70eVnKKzDtNoXmUG2steLYcNA_IC6Oie51GIpKPpYsFPzkQsPzk1z1MTtE-kFUXIMlnw15c1GduoiQd7-mw6e5UmMBKwYXWbz5LJm-TOLpmgLeQD9THxxIdGbeIg9hx8cFBH_PTgAMcDJnGJ4piFvVHgos4BHkSwheKhdDz_POWzkz-6SX1t?type=png)](https://mermaid.live/edit#pako:eNqtldFq2zAUhl_F6Lp9gdyNmZVStoVml4ah2aeZILaDLA9CGtjWtWysF2PLYLAEVgqDjl5kpXQe9Ili5R0mybasxHa9wXRhx9J3LP3_OSceIzf0AHUQUJvgPsW-E1hidGnoxS6zDg-3t8Ox9RCCuJjqWG4YMEyCaB0dZ49ykIAZK7u21d2zHMRvpsvFy6f86NXq49td20FWGRExSoJ-EfEI-yAmRYhi0x_Hd8BdSlwoYbHF8urCQSXuYQbWPvSJiMOMhIEtJ_R50k8_07M5n9_y97MibJLdpOwdGsZD04eKASVVtUCvbZiQXkzTd9fLX0l6_ltaURGnA3Mv1HCQGadsaZOZ2dimVOlqz7XC6kXW6mtUphOccRtKDFAnNxf-n5JbJq65ev9S1b_Vut77MfWAPsHPBlD4rmYqxWVw1SMai2rX1fEpn1-nybTWeAVq5zUrr9_f1EhS_E4MEYvW-YR__WAqUkVWnnZNUGPHtFPZyxpUF0bnDzVyM3NGQ7hv511wfpteJnz2bfXlcxPfY5jFkYjQuMjg0Wzt70eVnKKzDtNoXmUG2steLYcNA_IC6Oie51GIpKPpYsFPzkQsPzk1z1MTtE-kFUXIMlnw15c1GduoiQd7-mw6e5UmMBKwYXWbz5LJm-TOLpmgLeQD9THxxIdGbeIg9hx8cFBH_PTgAMcDJnGJ4piFvVHgos4BHkSwheKhdDz_POWzkz-6SX1t)

## 데이터 단어사전
| No  | 단어명      | 영문명          | 단어 설명 | 분류단어  | Type     |
|-----|----------|-----------------|-------|--------|----------|
| 1   | 상품       | Product         |       |       |          |
| 2   | 명        | Name            |       | Y     | String   |
| 3   | 가격       | Price           |       | Y     | int      |
| 4   | 등록       | Registration    |       |       ||
| 5   | 메뉴       | Menu            |       |       ||
| 6   | 그룹       | Group           |       |       ||
| 7   | ID       | ID              |       | Y     | String   |
| 8   | 주문       | Order          |       |       ||
| 9   | 테이블      | Table          |       |       ||
| 10  | 인원       | Guests          |       |       ||
| 11  | 유형       | Type            |       | Y     | String   |
| 12  | 상태       | Status          |       | Y     | String   |
| 13  | 배송       | Delivery        |       |       ||
| 14  | 주소       | Address         |       | Y     | String   |
| 15  | 기사       | Rider           |       |       |          |
| 16  | 일시       | Date            |       | Y     | Date     |

## 데이터 용어 사전
| No  | 용어     | 영문명             |  용어설명  |
|---|--------|-----------------|---|
| 1   | 상품ID   | ProductID       | |    
| 2   | 상품명    | ProductName     ||
| 3   | 상품가격   | ProductPrice    ||
| 4   | 등록일시   | RegistraionDate | |   
| 5   | 메뉴그룹ID | MenuGroupID     | |
| 6   | 메뉴그룹명  | MenuGroupName   | |
| 7   | 메뉴ID   | MenuID          | |
| 8   | 메뉴명    | MenuName        | |
| 9   | 메뉴가격   | MenuPrice       | |
| 10  | 테이블ID  | OrderTable      | |
| 11  | 테이블이름  | TableName       | |
| 12  | 테이블인원  | TableGuests     | |
| 13  | 주문ID   | OrderID         |  | 
| 14  | 주문유형   | OrderType       | |
| 15  | 주문상태   | OrderStatus     | |
| 16  | 주문일자   | OrderDate       | |
| 17  | 배송주소   | DeliveryAddress | |
| 18  | 배송기사   | DeliveryRider   | |
| 19  | 주문테이블  | OrderTable      |  |


### 메뉴그룹(`MenuGroup`)
- 메뉴그룹(`MenuGroup`)은 메뉴그룹 정보을 가진다.
  - 외부에 노출되는 메뉴 그룹명(Name)을 가진다.

- `MenuGroupService`는 메뉴그룹(`MenuGroup`) 관련된 작업을 한다.
  - 새로운 메뉴그룹(`MenuGroup`)을 등록한다.
    - 메뉴 그룹명(Name)은 올바르지 않으면 등록할 수 없다.
      - 메뉴 그룹명(Name)은 빈 값이 올 수 없다.
      - 메뉴 그룹명(Name)은 비속어검증기(`PurgomalumClient`)를 통해 비속어를 필터링한다.

  - 사용자에게 메뉴그룹(`MenuGroup`) 내역을 제공한다.

### 상품(`Product`)
- 상품(`Product`)는 상품 정보를 가진다.
  - 외부에 노출되는 상품 명(Name)을 가진다.
  - 상품의 판매 금액(Price)을 가진다.

- `ProductService`는 상품(`Product`) 관련된 작업을 한다.
  - 새로운 상품(`Product`)를 등록한다.
    - 상품 가격(Price)이 잘못 입력되면 등록할 수 없다.
      - 상품 가격(Price)은 0원 이상 입력한다.
    - 상품명(Name)이 잘못 입력되면 등록할 수 없다.
      - 상품명(Name)은 빈 값이 올 수 없다.
      - 상품명(Name)은 비속어검증기(`PurgomalumClient`)를 통해 비속어를 필터링한다.

  - 상품 가격(Price)을 변경할 수 있다.
    - 상품 가격(Price)이 잘못 입력되면 변경할 수 없다.
      - 상품 가격(Price)은 0원 이상 입력한다.
    - 해당 상품이 포함된 메뉴(`Menu`) 내역을 가져와서 메뉴의 가격이 상품들(`menuProducts`) 총합보다 비쌀 경우 메뉴를 비공개(Display)한다.

  - 사용자에게 상품(`Product`) 내역을 제공한다.

### 메뉴(`Menu`)
- 메뉴(`Menu`)는 메뉴 정보를 가진다.
  - 외부에 노출되는 메뉴명(Name)을 가진다.
  - 판매 금액(Price)을 가진다.
  - 고객에게 판매될지 안될지 공개여부(Display)를 가진다.
  - 메뉴가 속한 메뉴그룹(`MenuGroup`)을 가진다.
  - 새로운 메뉴 등록 시, 메뉴그룹(`MenuGroup`)을 찾기위한 메뉴그룹 아이디(menuGroupId)를 가진다.
  - 메뉴를 통해 제공되는 상품 내역(`MenuProduct`)을 가진다.

- 메뉴 상품(`MenuProduct`)은 메뉴 상품 정보를 가진다.
  - 메뉴에 속한 상품(`Product`)을 가진다.
  - 고객에게 얼마나 제공되는지 메뉴 상품 수량(Quantity)를 가진다.
  - 새로운 메뉴 상품 등록 시, 상품(`Product`)을 찾기위한 상품 아이디(productId)를 가진다.

- `MenuService`는 메뉴(`Menu`) 관련된 작업을 한다.
  - 새로운 메뉴(`Menu`)를 등록한다.
    - 메뉴 가격(Price)이 잘못 입력되면 등록할 수 없다.
      - 메뉴 가격(Price)은 0원 이상 입력해야한다.
      - 메뉴 가격(Price)은 메뉴 상품(`MenuProduct`) 가격의 총합을 넘을 수 없다.
    - 메뉴그룹 아이디(menuGroupId)이 잘못 입력되면 등록할 수 없다.
      - 메뉴그룹 아이디(menuGroupId)은 등록된 메뉴그룹(`MenuGroup`)의 아이디여야한다.
    - 메뉴 상품(`MenuProduct`)이 잘못 입력되면 등록할 수 없다.
      - 상품 수량(Quantity)은 0개 이상 입력해야 한다.
      - 상품 아이디(productId)은 등록된 상품(`Product`)의 아이디여야한다.
    - 메뉴명(Name)은 잘못 입력되면 등록할 수 없다.
      - 메뉴명(Name)은 빈 값이 올 수 없다.
      - 메뉴명(Name)은 비속어검증기(`PurgomalumClient`)를 통해 비속어를 필터링한다.

  - 메뉴 가격(Price)을 변경한다.
    - 메뉴 가격(Price)이 잘못 입력되면 등록할 수 없다.
      - 메뉴 가격(Price)은 0원 이상 입력해야한다.
      - 메뉴 가격(Price)은 메뉴 상품(`MenuProduct`) 가격의 총합을 넘을 수 없다.

  - 메뉴를 판매하기 위해 공개(Display)한다.
    - 메뉴 가격(Price)이 잘못 되어있으면 공개할 수 없다.
      - 메뉴 가격(Price)은 메뉴 상품(`MenuProduct`) 가격의 총합을 넘을 수 없다. 메뉴 가격(Price)부터 변경해야한다.

  - 메뉴를 판매 안하기 위해 비공개(Display)한다.

  - 사용자에게 메뉴(`Menu`) 내역을 제공한다.


### 주문 테이블(`OrderTable`)
- 주문 테이블(`OrderTable`)은 매장 테이블 정보를 가진다.
  - 주문 테이블 이름(Name)을 가진다.
  - 주문 테이블에 앉은 손님 수(numberOfGuests)를 가진다.
  - 주문 테이블이 사용중인지 확인하는 빈(empty) 상태를 가진다.

- `OrderTableService`는 주문 테이블(`OrderTable`) 관련 작업을 한다.
  - 새로운 주문 테이블(`OrderTable`)를 등록한다.
    - 테이블 이름(Name)은 잘못 입력되면 등록할 수 없다.
      - 테이블 이름(Name)은 빈 값이 올 수 없다.
    - 새로운 주문 테이블의 손님 수(numberOfGuests)는 기본 0명이다
    - 새로운 주문 테이블의 빈(empty) 상태는 기본이 비어있다.

  - 테이블을 사용중으로 변경한다.
    - 빈(empty) 상태를 사용중으로 변경한다.

  - 테이블을 정리한다.
    - 주문 테이블 정보가 잘못되면 변경할 수 없다.
      - 주문 테이블의 주문 완료(COMPLETED)가 아니면 변경할 수 없다.

  - 손님 수(numberOfGuests)를 변경한다.
    - 손님 수(numberOfGuests)가 잘못 입력되면 변경할 수 없다.
      - 손님 수(numberOfGuests)는 0명 이상 입력해야한다.
    - 테이블의 빈(empty) 상태가 이상하면 변경할 수 없다.
      - 테이블의 빈(empty) 상태는 비어있지 않아야한다.

  - 사용자에게 주문 테이블(`OrderTable`) 내역을 제공한다.


### 주문(`Order`)
- 주문(`Order`)은 주문 정보를 가진다.
  - 고객이 선택한 주문 유형(`OrderType`)을 가진다.
  - 고객이 확인할 수 있는 주문 상태(`OrderStatus`)를 가진다.
  - 고객이 주문한 주문 메뉴(`OrderLineItem`)를 가진다.
  - 주문이 들어온 주문 시각(orderDateTime)을 가진다.
  - 주문이 배송(`DELIVERY`)일 경우 경우 배송 받을 주소(deliveryAddress)를 가진다..
  - 주문이 매장내 식사(`EAT_IN`)일 경우 주문이 들어온 주문 테이블(`OrderTable`)을 가진다.
  - 주문이 매장내 식사(`EAT_IN`)일 경우 주문 테이블(`OrderTable`)을 찾기 위한 주문 테이블 아이디(orderTableId)을 가진다.

- 주문 유형(`OrderType`)은 주문 유형 정보를 가진다.
  - 배달 주문(`DELIVERY`)을 표현한다.
  - 포장 주문(`TAKEOUT`)을 표현한다.
  - 매장내 식사(`EAT_IN`)를 표현한다.

- 주문 상태(`OrderStatus`)는 주문 상태 정보를 가진다.
  - 주문 대기(`WAITING`)를 표현한다.
  - 주문 접수(`ACCEPTED`)를 표현한다.
  - 주문 전달(`SERVED`)를 표현한다.
  - 주문 배송 중(`DELIVERING`)를 표현한다.
  - 주문 배송 완료(`DELIVERED`)를 표현한다.
  - 주문 완료(`COMPLETED`)를 표현한다.

- 주문 메뉴(`OrderLineItem`)은 주문 메뉴 정보를 가진다.
  - 주문 받은 메뉴(`Menu`)를 가진다.
  - 주문 수량(Quantity)를 가진다.
  - 주문 금액(Price)를 가진다.

- `OrderService`은 주문(`Order`) 관련된 작업을 한다.
  - 새로운 주문(`Order`)을 등록한다.
    - 주문 유형(`OrderType`)이 잘못 입력되면 등록할 수 없다.
      - 주문 유형(`OrderType`)은 빈 값이 올 수 없다.
    - 매장내 식사(`EAT_IN`)일 경우 주문 테이블(`OrderTable`) 정보가 잘못되면 입력할 수 없다.
      - 주문 테이블 아이디(orderTableId)은 등록된 주문 테이블(`OrderTable`)의 아이디여야한다.
      - 주문 테이블(`OrderTable`)을 찾지 못하면 등록할 수 없다.
      - 주문 테이블(`OrderTable`)이 비어있으면 등록할 수 없다.
    - 배송 주문(`DELIVERY`)일 경우 배송지가 잘못 입력되면 등록할 수 없다.
      - 배송지(deliveryAddress)는 빈 값이 올 수 없다.
    - 주문 상태(`OrderStatus`)는 기본적으로 대기(WAITING)다.
    - 주문 메뉴(`OrderLineItem`)가 잘못 입력되면 등록할 수 없다.
      - 주문 메뉴(`OrderLineItem`)는 한개 이상 있어야 한다.
      - 매장내 식사(`EAT_IN`)가 아닐 경우 수량(Quantity)은 0개 이상이여야 한다.
      - 주문 메뉴(`OrderLineItem`)가 판매중인 상태(Display)인지 확인한다.
      - 주문 메뉴(`OrderLineItem`) 가격(Price)과 메뉴(`Menu`)의 가격(Price)은 동일해야한다.
    - 주문 시각(orderDateTime)은 현재 시각으로 등록한다.

  - 주문을 접수(`ACCEPTED`)한다.
    - 대기(`WAITING`) 상태만 변경할 수 있다.
    - 배달 유형(`DELIVERY`)은 라이더(`KitchenridersClient`)를 호출한다.
      - 주문의 총 금액(Price)을 구하여 전달한다.
      - 배송지(deliveryAddress)를 전달한다.

  - 주문을 전달(`SERVED`)한다.
    - 접수(`ACCEPTED`) 상태만 변경할 수 있다.

  - 배달 주문(`DELIVERY`)을 배송(`DELIVERING`)한다.
    - 배달 주문(`DELIVERY`)만 변경 할 수 있다.
    - 전달(`SERVED`) 상태만 변경 할 수 있다.

  - 배달 주문(`DELIVERY`)을 배송 완료(`DELIVERED`)한다.
    - 배달 주문(`DELIVERY`)만 변경 할 수 있다.
    - 배송 중(`DELIVERING`) 상태만 변경 할 수 있다.

  - 주문을 완료(`COMPLETED`)한다.
    - 주문 유형(`OrderType`)에 따라 다르게 진행한다.
      - 배송 주문(`DELIVERY`)은 배송 완료(`COMPLETED`)일 경우에 변경이 가능하다.
      - 포장 주문(`TAKEOUT`)은 전달(`SERVED`)일 경우에 변경이 가능하다.
      - 매장내 식사(`EAT_IN`)는 전달(`SERVED`)일 경우에 변경이 가능하다.
        - 주문 테이블(`OrderTable`)이 비어있지 않아야한다.

  - 사용자에게 주문(`Order`) 내역을 제공한다.

### 범용 보조
비속어검증기(`PurgomalumClient`)는 비속어를 필터링한다.

### 외부
라이더(`KitchenridersClient`)는 배달 기사를 호출한다. 
