``` mermaid
gantt
    title 專案進度甘特圖
    dateFormat YYYY-MM-DD
    axisFormat %m-%d

    section 規劃
    研擬計畫      :crit, 2025-10-01, 1d
    任務分配      :crit, after 研擬計畫, 4d

    section 硬體準備
    取得硬體      :after 研擬計畫, 17d
    安裝硬體      :after 取得硬體, 10d

    section 系統開發
    程式開發      :crit, after 任務分配, 70d
    程式測試      :crit, after 程式開發, 30d
    系統測試      :crit, after 程式測試, 25d

    section 文件/轉檔
    撰寫手冊      :after 安裝硬體, 25d
    轉換檔案      :after 安裝硬體, 20d

    section 訓練與驗收
    使用者訓練    :after 撰寫手冊, 25d
    使用者訓練    :after 轉換檔案, 25d
    使用者測試    :crit, after 系統測試, 25d
    使用者測試    :crit, after 使用者訓練, 25d
```
```


