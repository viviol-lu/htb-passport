# Path Passport｜HTB Academy 非官方學習助手

自動追蹤 HTB Academy 的 Path、模組與學習章節，依章節保存筆記，支援 Markdown 與 HTML 匯出。Chrome／Firefox 擴充功能，介面與手冊可切換繁體中文／English。

作者：Vivian Lu · [Vivian@SecMomBag](https://vvnblog.com/en/)

> 非官方工具。自動化讀取可能受 HTB 使用政策限制；版本編號與「非官方」標示不代表取得 HTB 授權或已上架。

目前發行版：**v1.1.4**

## 下載

到本頁右側（或上方）的 **Releases** 下載最新版，或直接前往：

👉 **<https://github.com/viviol-lu/htb-passport/releases/latest>**

| 檔案 | 說明 |
|---|---|
| `academy-passport-chrome-v1.1.4.zip` | Chrome 擴充包 |
| `academy-passport-firefox-v1.1.4.zip` | Firefox 擴充包 |
| `installation-guide-v1.1.4.html` | 離線安裝手冊（可在安裝前閱讀） |
| `user-guide-v1.1.4.html` | 操作手冊 |
| `SHA256SUMS.txt` | 檔案校驗碼 |

### 校驗下載（建議）

下載後可比對 SHA-256，確認檔案未被竄改：

```bash
shasum -a 256 academy-passport-chrome-v1.1.4.zip academy-passport-firefox-v1.1.4.zip
```

比對結果應與 `SHA256SUMS.txt` 內的值一致。

## 安裝

### Chrome
1. 解壓縮 `academy-passport-chrome-v1.1.4.zip`。
2. 開啟 `chrome://extensions`，開啟「開發人員模式」。
3. 選「載入未封裝項目」，選擇解壓出來的資料夾。
4. 重新整理已登入的 HTB Academy 頁面。

### Firefox
1. 解壓縮 `academy-passport-firefox-v1.1.4.zip`。
2. 開啟 `about:debugging#/runtime/this-firefox`。
3. 選「暫時載入附加元件」，選擇解壓資料夾內的 `manifest.json`（Firefox 142 或更新版本）。
4. 重新整理 Academy 頁面。

> Firefox 此方式為開發測試安裝，關閉瀏覽器後需要重新載入；正式持續安裝需 Mozilla 簽署，本專案尚未上架或簽署。更新後請重新載入擴充功能再重新整理 Academy。

詳細圖文步驟請見 `installation-guide-v1.1.4.html`。

## 權限說明

擴充套件僅要求 `storage`（本機保存筆記與設定）與 `activeTab`，只在 `https://academy.hackthebox.com/*` 運作。筆記與資料皆保存在本機瀏覽器，不上傳。
