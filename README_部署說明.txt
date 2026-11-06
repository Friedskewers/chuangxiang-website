串香蔬食炸烤萬隆店｜正式網站部署包
======================================

網站內容
- index.html：品牌首頁、店家資訊、Google 地圖、Restaurant 結構化資料
- menu.html：菜單介紹頁、Menu 結構化資料
- assets/style.css：手機優先的響應式版型
- assets/favicon.svg：網站圖示
- robots.txt、sitemap.xml：搜尋引擎爬取與網站地圖
- .github/workflows/pages.yml：GitHub Pages 自動部署

已採用可核對的公開店家資訊
- 地址：台北市文山區興隆路一段263號2樓
- 電話：0987-718-118
- Uber Eats：萬德福串香蔬食炸烤 萬隆店
- 公開平台列示營業時間：週一至週六 17:00–22:30（上線前請店家再次確認）
- Google Maps 座標：24.9991699, 121.5443952

重要：目前還沒有正式網域，因此程式內 __SITE_URL__ 是待設定值。請完成以下步驟：

A. 建立 GitHub Pages 網站（免費）
1. 登入 https://github.com/ 並建立新 Repository，名稱建議 chuangxiang-website。
2. 將本資料夾內所有檔案與 .github 資料夾完整上傳到 Repository 根目錄。
3. Repository → Settings → Pages → Build and deployment，選 GitHub Actions。
4. 將 main 分支設為主要分支，等待 Actions 執行完成。
5. 網址通常會是 https://你的GitHub帳號.github.io/chuangxiang-website/ 。

B. 設定正式網址
1. 確定 GitHub Pages 網址後，將所有檔案中的 __SITE_URL__ 替換為完整網址（結尾不要加斜線）。
2. 提交變更到 main，GitHub Actions 會重新部署。
3. 若日後購買自有網域，需在 GitHub Pages 設定 Custom domain、DNS 設定及 HTTPS，再將 __SITE_URL__ 換成自有網域重新部署。

C. Google 搜尋收錄
1. 開啟 https://search.google.com/search-console/ ，新增「網址前置字元」資源，輸入實際網站網址。
2. 使用 HTML 檔案驗證或 DNS 驗證。若使用 HTML 檔案驗證，請將 Google 提供的驗證 HTML 檔放在網站根目錄再提交。
3. 在 Search Console → Sitemap 提交 sitemap.xml。
4. 用網址審查檢查首頁及 menu.html，符合條件後按「要求建立索引」。索引與排名需要時間，無法保證特定日期或名次。

D. Google Analytics 4（可選）
1. 到 https://analytics.google.com/ 建立 GA4 資源及 Web 資料串流。
2. 取得自己的 G-XXXXXXXXXX Measurement ID。
3. 依 GA4 官方安裝說明，將 Google tag 放進 index.html 與 menu.html 的 <head>。
4. 不要貼上他人的 Measurement ID。沒有 GA4 ID 前，不會放入虛構追蹤碼。

E. 上線前請店家確認
- 店名是否要顯示「串香蔬食炸烤」或「萬德福串香蔬食炸烤 萬隆店」。
- 地址、電話、營業時間目前依公開 Uber Eats 頁面整理，請確認是否仍正確。
- 菜單頁列的是品項介紹，沒有固定價格；最新價格連到 Uber Eats，以免價格過期。
- 各品項的全素／蛋素／蛋奶素及過敏原標示請逐項確認，不可把整間店宣稱為全素。

網站不會自動製造評論、假訪客或假搜尋點擊。Google 排名取決於內容品質、網站體驗、商家資料一致性、競爭程度與時間，沒有程式能保證流量暴增或首頁排名。
