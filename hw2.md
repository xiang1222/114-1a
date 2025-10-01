```
gantt
    title 專案時程
    dateFormat YYYY-MM-DD
    axisFormat %m-%d

    section 規劃階段
    研擬計畫       :done, crit, 2025-10-01, 1d
    任務分配       :done, crit, 2025-10-02, 4d

    section 資源準備
    取得硬體       : 2025-10-02, 17d
    安裝硬體       : 2025-10-19, 10d

    section 程式開發
    程式開發       :crit, 2025-10-06, 70d
    程式測試       :crit, 2025-12-15, 30d

    section 系統驗證
    系統測試       :crit, 2025-01-14, 25d
    使用者訓練     : 2025-11-18, 25d
    撰寫手冊       : 2025-10-29, 25d
    轉換檔案       : 2025-10-29, 20d

    section 結案驗收
    使用者測試     :crit, 2025-02-08, 25d
```
```

- `:crit` 會用紅色顯示關鍵路徑，[4]
- 可用 `:done`（已完成）、` :active`（進行中）修飾各任務狀態[3][4]
- `dateFormat YYYY-MM-DD` 建議用起始日期配合天數計算，例如 2025-10-01 為第一天，依據上表逐項依序排出。

***

### 二、Mermaid 任務依賴（PERT/CPM風格流程圖）

GitHub 支援 Mermaid flowchart，能畫出節點與依賴流程：

````markdown
```
flowchart TD
    A[研擬計畫] --> B[任務分配]
    A --> C[取得硬體]
    B --> D[程式開發]
    D --> E[程式測試]
    E --> F[系統測試]
    C --> G[安裝硬體]
    G --> H[撰寫手冊]
    G --> I[轉換檔案]
    H --> J[使用者訓練]
    I --> J
    F --> K[使用者測試]
    J --> K
```
```

