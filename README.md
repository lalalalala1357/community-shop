# Community Shop

社區團購平台的客人前台網站，使用 HTML、CSS、Vanilla JavaScript 與 Firebase Firestore。

這個 repository 放客人會使用的頁面：瀏覽商品、查看商品詳情、送出預購、查詢訂單、查看訂單詳細與許願池。

管理後台請放在 `community-shop-admin` repository。

## Included Pages

- `index.html`：首頁、熱門商品、最新商品、即將截止商品、公告
- `products.html`：商品列表、搜尋、分類、排序
- `product.html`：商品詳細與下單
- `order-success.html`：下單成功頁
- `order-search.html`：訂單查詢
- `order-detail.html`：客人訂單詳細
- `wish.html`：許願池
- `wishlist.html`：簡易願望清單頁

## Shared Assets

- `css/styles.css`
- `js/app.js`
- `js/firebase.js`
- `js/firebase-config.js`
- `firestore.rules`

## Firebase Setup

1. 建立 Firebase 專案。
2. 啟用 Firestore Database。
3. 將 Firebase Web App config 放在 `js/firebase-config.js`。
4. 若需要管理商品、訂單與公告，請使用獨立的 `community-shop-admin` 後台 repo。
5. 部署此 repo 到 GitHub Pages 或其他靜態網站服務。

## Firestore Collections

前台沿用既有資料結構，不修改 collection 名稱：

- `products`
- `orders`
- `publicOrders`
- `productImages`
- `productCategories`
- `announcements`
- `wishes`
- `wishlists`

## Notes

- 這個 repo 是 customer-facing 發布版本。
- 不包含 `admin-*.html` 後台入口。
- `js/app.js` 仍保留部分共用 helper，方便和後台 repo 使用同一套資料格式與流程。
