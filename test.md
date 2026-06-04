graph LR
    A[Веб-браузер / Мобильное приложение] -->|HTTPS/REST API| B[Nginx]
    B --> C["Backend API"]
    C --> D[(PostgreSQL)]
    C --> E[(Redis Cache)]
    
    classDef client fill:#f9f,stroke:#333,stroke-width:2px;
    classDef server fill:#bbf,stroke:#333,stroke-width:2px;
    classDef db fill:#bfb,stroke:#333,stroke-width:2px;
    
    class A client;
    class B,C server;
    class D,E db;
