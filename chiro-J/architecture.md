my-service/
├── .github/                # GitHub Actions 워크플로우(CI/CD) 폴더
│   └── workflows/
│       └── ci.yml
│       └── cd.yml
│
├── docker/                 # 도커 관련 파일/설정 (DB, nginx 등)
│   └── nginx.conf
│   └── init.sql
│
├── backend/
│   ├── src/
│   │   ├── controllers/
│   │   ├── routes/
│   │   ├── services/
│   │   ├── models/
│   │   ├── middlewares/
│   │   ├── utils/
│   │   ├── app.ts
│   │   ├── server.ts
│   │   └── swagger/         # Swagger(오픈API) 설정
│   │        └── swagger.yaml
│   ├── tests/
│   ├── Dockerfile
│   ├── docker-compose.yml   # 백엔드 단독 개발/테스트용
│   ├── package.json
│   ├── .env
│   └── README.md
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── store/
│   │   ├── api/
│   │   ├── utils/
│   │   ├── App.tsx
│   │   ├── index.tsx
│   │   └── setupTests.ts
│   ├── public/
│   ├── Dockerfile
│   ├── package.json
│   ├── .env
│   └── README.md
│
├── docker-compose.yml       # 전체 서비스(프론트+백+DB) 통합용
│
├── scripts/                 # CI/CD, 배포, 마이그레이션 등 스크립트
│   └── deploy.sh
│   └── db-migrate.js
│
├── docs/                    # 아키텍처/시스템 설계, API 문서
│   └── api-spec.md
│   └── system-arch.drawio
│
├── .env.example
├── .gitignore
└── README.md