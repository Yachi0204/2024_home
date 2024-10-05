graph TD;
    A[1. 研擬任務 (1天)] --> B[2. 任務分配 (4天)];
    A --> C[3. 取得硬體 (17天)];
    B --> D[4. 程式開發 (70天)];
    C --> E[5. 安裝硬體 (10天)];
    D --> F[6. 程式測試 (30天)];
    E --> G[7. 撰寫使用手冊 (25天)];
    E --> H[8. 轉換檔案 (20天)];
    E --> I[9. 系統測試 (25天)];
    G --> J[10. 使用者訓練 (20天)];
    H --> J;
    I --> K[11. 使用者測試 (25天)];
    J --> K;
    F --> K;
gantt
    title 專案甘特圖
    dateFormat  YYYY-MM-DD
    section 任務
    研擬任務      :done,    des1, 2024-10-05, 1d
    任務分配      :active,  des2, after des1, 4d
    取得硬體      :         des3, after des1, 17d
    程式開發      :         des4, after des2, 70d
    安裝硬體      :         des5, after des3, 10d
    程式測試      :         des6, after des4, 30d
    撰寫使用手冊  :         des7, after des5, 25d
    轉換檔案      :         des8, after des5, 20d
    系統測試      :         des9, after des5, 25d
    使用者訓練    :         des10, after des7 des8, 20d
    使用者測試    :         des11, after des6 des9 des10, 25d
graph TD;
    A[1. 研擬任務 (1天)] --> B[2. 任務分配 (4天)];
    A --> C[3. 取得硬體 (17天)];
    B --> D[4. 程式開發 (70天)];
    C --> E[5. 安裝硬體 (10天)];
    D --> F[6. 程式測試 (30天)];
    E --> G[7. 撰寫使用手冊 (25天)];
    E --> H[8. 轉換檔案 (20天)];
    E --> I[9. 系統測試 (25天)];
    G --> J[10. 使用者訓練 (20天)];
    H --> J;
    I --> K[11. 使用者測試 (25天)];
    J --> K;
    F --> K;
    
    class D,F,K red;
    
    classDef red fill:#f96,stroke:#333,stroke-width:2px;
