# Path Passport｜HTB Academy 非官方學習助手 / Unofficial Study Helper

**[繁體中文](#繁體中文) ｜ [English](#english)**

---

## 繁體中文

自動追蹤 HTB Academy 的 Path、模組與學習章節，並依章節儲存筆記，支援 Markdown 與 HTML 匯出。這是 Chrome／Firefox 擴充套件，介面與操作手冊都可以切換繁體中文與 English。

作者：Vivian Lu · [Vivian@SecMomBag](https://vvnblog.com/en/)

> 非官方工具。自動化讀取可能受 HTB 使用政策限制；版本編號與「非官方」標示，並不代表已取得 HTB 授權或已上架。

### 下載

請一律從 **Releases** 下載最新版，版本號以該頁為準。

👉 **<https://github.com/viviol-lu/htb-passport/releases/latest>**

每個版本都會附上以下檔案。

| 附件 | 說明 |
|---|---|
| `academy-passport-chrome-*.zip` | Chrome 擴充套件安裝包 |
| `academy-passport-firefox-*.zip` | Firefox 擴充套件安裝包 |
| `installation-guide-*.html` | 離線安裝手冊，可在安裝前先閱讀 |
| `user-guide-*.html` | 操作手冊 |
| `SHA256SUMS.txt` | 檔案雜湊值，用來驗證完整性 |

#### 驗證下載（建議）

下載後可以比對 SHA-256 雜湊值，確認檔案沒有被竄改。

```bash
shasum -a 256 academy-passport-*.zip
```

比對出來的結果，應該與同一個 Release 裡 `SHA256SUMS.txt` 所列的值一致。

### 安裝

**Chrome**

1. 將下載的 Chrome 安裝包 ZIP 解壓縮。
2. 開啟 `chrome://extensions`，並開啟「開發人員模式」。
3. 點選「載入未封裝項目」，選擇剛才解壓縮出來的資料夾。
4. 重新整理已經登入的 HTB Academy 分頁。

**Firefox**

1. 將下載的 Firefox 安裝包 ZIP 解壓縮。
2. 開啟 `about:debugging#/runtime/this-firefox`。
3. 點選「暫時載入附加元件」，選擇解壓縮資料夾裡的 `manifest.json`，需要 Firefox 142 或更新的版本。
4. 重新整理 Academy 分頁。

> Firefox 的這種方式屬於開發測試安裝，關閉瀏覽器後需要重新載入；若要長期安裝，必須經過 Mozilla 簽署，而本專案尚未上架或簽署。更新之後，請先重新載入擴充套件，再重新整理 Academy。

詳細的圖文步驟，請參考同一個 Release 附件裡的安裝手冊 HTML（`installation-guide-*.html`）。

### 隱私與權限

這個擴充套件只會在 HTB Academy 網站上運作，不會讀取你在其他網站的瀏覽內容。所有筆記與設定，都只儲存在你自己的瀏覽器本機，不會上傳，也不會傳送到任何外部伺服器。它只要求運作所需的最小權限。

---

## English

Automatically tracks your HTB Academy paths, modules and lesson sections, keeps notes per section, and exports to Markdown and HTML. It is a Chrome／Firefox extension, and both the interface and the guides switch between Traditional Chinese and English.

Author: Vivian Lu · [Vivian@SecMomBag](https://vvnblog.com/en/)

> Unofficial tool. Automated reading may be subject to HTB's usage policy; the version number and the "unofficial" label do not imply HTB authorization or any listing.

### Download

Always get the newest build from **Releases**; the version number is shown there.

👉 **<https://github.com/viviol-lu/htb-passport/releases/latest>**

Each release ships these files:

| Asset | Description |
|---|---|
| `academy-passport-chrome-*.zip` | Chrome extension package |
| `academy-passport-firefox-*.zip` | Firefox extension package |
| `installation-guide-*.html` | Offline installation guide (readable before installing) |
| `user-guide-*.html` | User guide |
| `SHA256SUMS.txt` | Checksums for verifying integrity |

#### Verify your download (recommended)

After downloading, compare the SHA-256 hashes to confirm the files were not tampered with.

```bash
shasum -a 256 academy-passport-*.zip
```

The results should match the values listed in the `SHA256SUMS.txt` from the same release.

### Install

**Chrome**

1. Unzip the downloaded Chrome package.
2. Open `chrome://extensions` and turn on **Developer mode**.
3. Choose **Load unpacked** and select the extracted folder.
4. Refresh any signed-in HTB Academy tab.

**Firefox**

1. Unzip the downloaded Firefox package.
2. Open `about:debugging#/runtime/this-firefox`.
3. Choose **Load Temporary Add-on** and select `manifest.json` inside the extracted folder (Firefox 142 or later).
4. Refresh the Academy tab.

> On Firefox this is a temporary developer install and must be reloaded after the browser restarts. A permanent install requires Mozilla signing, which this project has not done. After updating, reload the extension and then refresh Academy.

For step-by-step instructions with screenshots, see the installation guide HTML (`installation-guide-*.html`) attached to the same release.

### Privacy & permissions

The extension runs only on the HTB Academy website and does not read your activity on other sites. All notes and settings stay locally in your own browser — they are never uploaded or sent to any external server. It requests only the minimum permissions needed to work.
