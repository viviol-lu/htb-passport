# Path Passport｜HTB Academy 非官方學習助手 / Unofficial Study Helper

**[繁體中文](#繁體中文) ｜ [English](#english)**

---

## 繁體中文

自動追蹤 HTB Academy 的 Path、模組與學習章節，依章節保存筆記，支援 Markdown 與 HTML 匯出。Chrome／Firefox 擴充功能，介面與手冊可切換繁體中文／English。

作者：Vivian Lu · [Vivian@SecMomBag](https://vvnblog.com/en/)

> 非官方工具。自動化讀取可能受 HTB 使用政策限制；版本編號與「非官方」標示不代表取得 HTB 授權或已上架。

### 下載

一律從 **Releases** 下載最新版（版本號以該頁為準）：

👉 **<https://github.com/viviol-lu/htb-passport/releases/latest>**

每個版本的附件：

| 附件 | 說明 |
|---|---|
| `academy-passport-chrome-*.zip` | Chrome 擴充包 |
| `academy-passport-firefox-*.zip` | Firefox 擴充包 |
| `installation-guide-*.html` | 離線安裝手冊（可在安裝前閱讀） |
| `user-guide-*.html` | 操作手冊 |
| `SHA256SUMS.txt` | 檔案校驗碼 |

#### 校驗下載（建議）

下載後可比對 SHA-256，確認檔案未被竄改：

```bash
shasum -a 256 academy-passport-*.zip
```

比對結果應與同一個 Release 內 `SHA256SUMS.txt` 的值一致。

### 安裝

**Chrome**
1. 解壓縮下載的 Chrome 擴充包 ZIP。
2. 開啟 `chrome://extensions`，開啟「開發人員模式」。
3. 選「載入未封裝項目」，選擇解壓出來的資料夾。
4. 重新整理已登入的 HTB Academy 頁面。

**Firefox**
1. 解壓縮下載的 Firefox 擴充包 ZIP。
2. 開啟 `about:debugging#/runtime/this-firefox`。
3. 選「暫時載入附加元件」，選擇解壓資料夾內的 `manifest.json`（Firefox 142 或更新版本）。
4. 重新整理 Academy 頁面。

> Firefox 此方式為開發測試安裝，關閉瀏覽器後需要重新載入；正式持續安裝需 Mozilla 簽署，本專案尚未上架或簽署。更新後請重新載入擴充功能再重新整理 Academy。

詳細圖文步驟請見同一個 Release 附件中的安裝手冊 HTML（`installation-guide-*.html`）。

### 權限說明

擴充套件僅要求 `storage`（本機保存筆記與設定）與 `activeTab`，只在 `https://academy.hackthebox.com/*` 運作。筆記與資料皆保存在本機瀏覽器，不上傳。

---

## English

Automatically tracks your HTB Academy paths, modules and lesson sections, keeps notes per section, and exports to Markdown and HTML. A Chrome／Firefox extension; interface and guides switch between Traditional Chinese and English.

Author: Vivian Lu · [Vivian@SecMomBag](https://vvnblog.com/en/)

> Unofficial tool. Automated reading may be subject to HTB's usage policy; the version number and the "unofficial" label do not imply HTB authorization or any listing.

### Download

Always get the newest build from **Releases** (the version number is shown there):

👉 **<https://github.com/viviol-lu/htb-passport/releases/latest>**

Assets in each release:

| Asset | Description |
|---|---|
| `academy-passport-chrome-*.zip` | Chrome extension package |
| `academy-passport-firefox-*.zip` | Firefox extension package |
| `installation-guide-*.html` | Offline installation guide (readable before installing) |
| `user-guide-*.html` | User guide |
| `SHA256SUMS.txt` | File checksums |

#### Verify your download (recommended)

After downloading, compare the SHA-256 hashes to confirm the files were not tampered with:

```bash
shasum -a 256 academy-passport-*.zip
```

The results should match the values in the `SHA256SUMS.txt` from the same release.

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
4. Refresh the Academy page.

> On Firefox this is a temporary developer install and must be reloaded after the browser restarts; a permanent install requires Mozilla signing, which this project has not done. After updating, reload the extension and refresh Academy.

For step-by-step instructions with screenshots, see the installation guide HTML (`installation-guide-*.html`) attached to the same release.

### Permissions

The extension requests only `storage` (to keep notes and settings locally) and `activeTab`, and runs only on `https://academy.hackthebox.com/*`. Notes and data stay in your local browser and are never uploaded.
