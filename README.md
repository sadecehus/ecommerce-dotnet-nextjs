# 🛒 E-Commerce (.NET 9 API + Next.js)

.NET 9 Web API backend ve Next.js frontend'den oluşan e-ticaret uygulaması.

## Yapı

```
├── API/        # ASP.NET Core 9 Web API (EF Core + SQLite)
└── client/     # Next.js + Tailwind + shadcn/ui
```

## Backend (`API/`)

- ASP.NET Core 9 Controller tabanlı Web API
- Entity Framework Core + SQLite (`DefaultConnection`)
- `ProductsController` — ürün listeleme/detay
- Global hata yönetimi için `ExceptionHandling` middleware
- OpenAPI / Swagger UI (Development ortamında)
- CORS: `http://localhost:3000`

```bash
cd API
dotnet restore
dotnet ef database update
dotnet run
```

## Frontend (`client/`)

- Next.js (App Router) + TypeScript
- Tailwind CSS + Radix UI / shadcn/ui bileşenleri
- `next-themes` ile karanlık mod

```bash
cd client
cp .env.local.example .env.local   # NEXT_PUBLIC_API_URL değerini ayarla
npm install
npm run dev
```

## Teknolojiler

.NET 9 · EF Core · SQLite · Next.js · TypeScript · Tailwind CSS · Radix UI
