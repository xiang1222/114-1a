```markdown
```
gantt
    title 專案時程
    dateFormat YYYY-MM-DD
    axisFormat %m-%d

    section 規劃階段
    研擬計畫       :crit, 2025-10-01, 1d
    任務分配       :crit, 2025-10-02, 4d

    section 資源準備
    取得硬體       : 2025-10-02, 17d
    安裝硬體       : 2025-10-19, 10d

    section 開發測試
    程式開發       :crit, 2025-10-06, 70d
    程式測試       :crit, 2025-12-15, 30d
    系統測試       :crit, 2025-01-14, 25d

    section 文件/訓練/驗收
    撰寫手冊       : 2025-10-29, 25d
    轉換檔案       : 2025-10-29, 20d
    使用者訓練     : 2025-11-18, 25d
    使用者測試     :crit, 2025-02-08, 25d
```
```
