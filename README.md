# Mellow

온라인 의류 쇼핑몰 개발 의뢰가 들어왔습니다.  
우리가 만들 서비스의 이름은 **[Mellow]** 다양한 카테고리로 구분된 의류를 판매하려 합니다.  
사용자는 원하는 의류를 검색하고, 장바구니에 추가하고, 결제 과정을 통해 구매를 완료할 수 있습니다.  


## 🎭 시나리오

**Case-1**
```
사용자 A는 겨울용 코트를 구매하고 싶습니다.  
쇼핑몰에서 "겨울 코트"를 검색하여 원하는 상품을 찾습니다.  
A는 상품 정보를 확인한 뒤, M 사이즈의 "브라운 롱 코트"를 장바구니에 추가합니다.  
장바구니를 확인한 후 결제 페이지로 이동하여 주문을 완료합니다.  
결제가 성공적으로 완료되면, A는 주문 내역에서 주문한 상품의 상태를 확인합니다.  
```

## 📚 전제 조건

- 🍀 사용자 계정이 존재해야 합니다.
  - 회원가입과 로그인 기능은 구현된 상태로 가정합니다.
- 🍀 상품 데이터는 서비스 초기 상태로 제공됩니다.
  - 상품 등록 및 수정 기능은 없으며, 데이터는 고정되어 있습니다.
- 🍀 결제 API는 가상으로 동작한다고 가정하며, 결제 성공 또는 실패 응답만 제공합니다.


## ⛳ Goals

- ✅ 사용자는 의류를 검색하고, 장바구니에 추가하며, 결제까지 완료할 수 있어야 합니다.
- ✅ 사용자는 결제 완료 후 주문 내역을 확인할 수 있어야 합니다.
- ✅ 상품은 카테고리별로 분류되어 탐색이 가능해야 합니다.


## 📑 정책

### ♟️ Stage 1: 기본 기능

**상품탐색**
- 사용자는 상품을 검색할 수 있어야 합니다.
- 사용자는 상품을 카테고리별로 탐색할 수 있어야 합니다.
**장바구니**
- 사용자는 상품을 장바구니에 추가하고, 장바구니를 조회할 수 있어야 합니다.
**주문**
- 사용자는 상품을 주문하고 결제를 완료할 수 있어야 합니다.
- 사용자는 주문 내역을 조회할 수 있어야 합니다.

### ♟️ Stage 2: 추가 기능

**상품리뷰**
- 사용자는 구매한 상품에 대해 리뷰를 작성할 수 있어야 합니다.

**상품추천**
- 사용자가 탐색한 상품과 연관있는 상품을 최대 15개 추천할 수 있어야합니다.
- 탐색에 포함되는 행동은 "상품 검색", "상품 조회", "장바구니에 상품 추가"입니다.

**상품탐색 필터**
- 검색 시 가격대나 색상, 사이즈 등을 기준으로 필터링할 수 있어야 합니다.

### ♟️ Stage 3: 고급 기능

**할인/쿠폰**
- 결제 시 할인율 적용이나 쿠폰 사용이 가능해야 합니다.
