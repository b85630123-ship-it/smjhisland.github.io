# 石門國中・山海之間的學習群島

以石門國中校務架構與龍潭佳安的山海意象為基礎，製作可部署到 GitHub Pages 的原創低多邊形 3D 網站原型。3D 場景使用 Three.js，包含群島環視、點選島嶼進入近景、居民行走、天氣情境切換、官方網站導覽與手機版版面。

## 互動方式

- 在群島總覽拖曳畫面旋轉，滾輪或右下角按鈕縮放；點選一座島進入近距離觀察，再按「返回群島」離開。
- 進入島嶼後可繼續拖曳環視，也可用滾輪或按鈕調整距離。
- 預設讀取石門國中位置的 Open-Meteo 即時天氣，約每 15 分鐘更新。雨天會顯示雨滴、居民雨衣與雨傘、地面積水；入夜會點亮路燈與窗戶，居民也會打開手電筒。
- 也可選擇晴天、下雨或夜晚模擬情境，預覽其他狀況。
- Open-Meteo 天氣資料依 CC BY 4.0 授權，網站天氣區提供資料來源連結。免費 API 適用非商業用途。

## 本機預覽

這是純靜態網站，不需建置步驟。可用任何靜態 HTTP 伺服器預覽專案根目錄，或直接部署到 GitHub Pages。Three.js、字型透過 CDN 載入，因此瀏覽器需要網路連線。

## GitHub Pages 部署

1. 在 GitHub 建立一個新的 repository，並將本資料夾中的 `index.html`、`style.css`、`main.js`、`README.md` 推送至 repository 根目錄。
2. 開啟 repository 的 **Settings → Pages**。
3. 在 **Build and deployment** 選擇 **Deploy from a branch**，branch 選 `main`、資料夾選 `/(root)`，再按 **Save**。
4. 等待 GitHub Pages 完成部署；網址會顯示在 Pages 設定頁。repository 名稱為 `<帳號>.github.io` 時使用帳號根網址，其他名稱則使用 `https://<帳號>.github.io/<repository>/`。

此原型只提供原始碼與部署步驟，不需要 GitHub 授權，也不會替使用者建立 repository 或發布網站。

## 校務入口與資料來源

入口依官方網站公開架構整理，將教務處、學務處、輔導室、總務處、特殊教育、資優教育、課程、午餐、公告與校史等概念轉為四座導覽島。部分官方網站內頁會因校方改版而異動；未確認穩定內頁的入口先連至官方首頁。

- [石門國中官方網站](https://www.smjh.tyc.edu.tw/index.php)
- [Open-Meteo 即時天氣 API 文件](https://open-meteo.com/en/docs)
- [桃園市公車石門國中站址資料（座標來源）](https://ebus.tycg.gov.tw/cms/api/route/5044/stop-address.pdf)
- [教務處業務職掌](https://www.smjh.tyc.edu.tw/modules/school/index.php?department_id=2&page_id=14)
- [學務處業務職掌](https://www.smjh.tyc.edu.tw/modules/school/index.php?department_id=3&page_id=25)
- [輔導室業務職掌](https://www.smjh.tyc.edu.tw/modules/school/index.php?department_id=5&page_id=71)
- [石門國中校史](https://sites.google.com/smjh.tyc.edu.tw/smjh/%E6%A0%A1%E5%8F%B2)

校史內容提到石門國中民國七十年設校、位於龍潭佳安里，以及學校結合社區資源、發展校園文化的方向。群島為品牌概念原型，不是官方校徽、校園測繪或正式校務系統。連結目標與視覺素材可於正式採用前由校方確認。
