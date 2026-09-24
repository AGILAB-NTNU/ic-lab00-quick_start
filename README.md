# PYNQ-ZU SD 卡映像檔燒錄與啟動步驟

本文件整理 PYNQ-ZU 開發板從確認硬體、燒錄 MicroSD 卡，到連接電腦並進入 JupyterLab 的完整操作流程。

## 一、硬體確認與準備

### 1. 確認開發板型號

確認包裝與開發板型號為 **PYNQ-ZU**。

![PYNQ-ZU 包裝與型號](images/step-01-board-model.png)

### 2. 打開包裝盒

打開 PYNQ-ZU 的包裝盒。

![打開包裝盒](images/step-02-open-box.png)

### 3. 取出 FPGA 開發板

從包裝中取出 FPGA 開發板。

![PYNQ-ZU FPGA 開發板](images/step-03-fpga-board.png)

### 4. 取出 MicroSD 記憶卡

準備隨附或要使用的 MicroSD 記憶卡。

![MicroSD 記憶卡](images/step-04-microsd-card.png)

### 5. 將 MicroSD 卡連接至電腦

將 MicroSD 卡插入讀卡機，再將讀卡機連接至電腦，準備進行映像檔燒錄。

![MicroSD 讀卡機](images/step-05-card-reader.png)

## 二、下載映像檔並燒錄 MicroSD 卡

### 6. 下載 PYNQ-ZU 映像檔

前往 [PYNQ Boards](https://www.pynq.io/boards.html)，下載對應 **PYNQ-ZU** 的 image 映像檔。

![PYNQ 映像檔下載頁面](images/step-06-pynq-image-download.png)

### 7. 下載並安裝 balenaEtcher

前往 [balenaEtcher 官方網站](https://etcher.balena.io/)，下載並安裝 **balenaEtcher** 燒錄工具。

![balenaEtcher 下載頁面](images/step-07-balena-etcher-download.png)

### 8. 開啟 balenaEtcher

安裝完成後，在桌面或應用程式清單中找到 **balenaEtcher** 並開啟。

![balenaEtcher 應用程式](images/step-08-balena-etcher-app.png)

### 9. 選擇映像檔與目標 MicroSD 卡

在 balenaEtcher 中依序選擇：

1. 已下載的 **PYNQ-ZU 映像檔**。
2. 要燒錄的 **MicroSD 卡**。
3. 確認選擇無誤後，按下開始燒錄。

![選擇映像檔](images/step-09-select-image.png)

![選擇目標 MicroSD 卡並開始燒錄](images/step-09-select-target.png)

### 10. 等待燒錄完成

balenaEtcher 開始寫入映像檔後，等待燒錄程序完成。

![balenaEtcher 燒錄進行中](images/step-10-flashing.png)

### 11. 確認燒錄後的檔案

燒錄完成後，開啟 MicroSD 卡，確認可以看到圖中所示的 **5 個檔案**。

![MicroSD 卡燒錄完成後的檔案](images/step-11-sd-files.png)

## 三、安裝 MicroSD 卡並連接開發板

### 12. 將 MicroSD 卡插入 PYNQ-ZU

從讀卡機中取出 MicroSD 卡，並插入 **PYNQ-ZU 的 MicroSD 卡插槽**。

![將 MicroSD 卡插入 PYNQ-ZU](images/step-12-insert-microsd.png)

### 13. 準備電源線

準備開發板所需的電源線。

![電源線](images/step-13-power-cable.png)

### 14. 準備電源轉接器

準備與電源線搭配使用的電源轉接器。

![電源轉接器](images/step-14-power-adapter.png)

### 15. 將 PYNQ-ZU 接上電源

將電源線與轉接器連接完成後，接至 PYNQ-ZU 的電源輸入端。

![PYNQ-ZU 接上電源](images/step-15-connect-power.png)

### 16. 開啟開發板電源

確認接線完成後，開啟 PYNQ-ZU 電源。

![開啟 PYNQ-ZU 電源](images/step-16-power-on.png)

### 17. 準備資料傳輸線

準備用於連接 PYNQ-ZU 與電腦的傳輸線。

![資料傳輸線](images/step-17-usb-cable.png)

### 18. 將 Micro-USB 端接至 PYNQ-ZU

將傳輸線的 **Micro-USB 端**接到 PYNQ-ZU 的 Micro-USB 接孔。

![Micro-USB 連接 PYNQ-ZU](images/step-18-connect-microusb.png)

### 19. 將 USB-C 端接至電腦

將傳輸線另一端的 **USB-C** 接至電腦。

![USB-C 連接電腦](images/step-19-connect-usbc-pc.png)

## 四、登入 JupyterLab 並驗證功能

### 20. 查詢開發板連線資訊

前往下列頁面查詢 PYNQ-ZU 開發板的相關資訊：

[開發板資訊頁面](https://share.google/1CTaT1acnmX7GL08b)

![PYNQ-ZU 開發板資訊頁面](images/step-20-board-information.png)

### 21. 登入 JupyterLab

依開發板資訊頁面提供的連結開啟 JupyterLab，輸入密碼後登入。

![JupyterLab 登入畫面](images/step-21-jupyter-login.png)

### 22. 執行範例確認功能

成功進入 JupyterLab 主畫面後，執行範例程式，確認開發板功能是否正常。

![JupyterLab 主畫面](images/step-22-jupyterlab.png)
