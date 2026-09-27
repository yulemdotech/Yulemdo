# Yulemdo bilan ishlashni boshlash

Bu hujjat Yulemdo ekotizimini sinovdan o‘tkazish, lokal muhitda ishlatish va loyihaga hissa qo‘shish uchun umumiy yo‘l-yo‘riq beradi.

## 1. Loyihani o‘rganish

Avval loyiha maqsadini va asosiy yo‘nalishlarini tushunib oling:

- [README.md](../README.md)
- [CONTRIBUTING.md](../CONTRIBUTING.md)
- [docs/architecture.md](architecture.md)

## 2. Mahalliy muhit

Loyiha boshlanishdan oldin quyidagi asosiy narsalar mavjud bo‘lishi kerak:

- Git
- Node.js yoki boshqa loyihada talab qilinadigan runtime
- Paket manager
- IDE / code editor

Agar loyiha keyingi bosqichlarda frontend, backend, auth yoki API xizmatlarini qo‘shsa, ularni alohida konteyner yoki monorepo tuzilishida boshqarish mumkin.

## 3. Lokal ishlab chiqarish

Proyektning texnik ishlash uslubi tayyorlash bosqichlarida quyidagilar bilan ishlanadi:

```bash
git clone https://github.com/yulemdotech/Yulemdo.git
cd Yulemdo
npm install
npm run dev
```

Agar loyiha keyinchalik boshqa stack bo‘lsa, bu qadamlar yangilanishi mumkin. Muhim narsa, ishlab qilishdan oldin loyiha uchun aniq start script va environment variables dokumentatsiyasi mavjud bo‘lishidir.

## 4. Mahalliy konfiguratsiya

Har bir xizmat yoki modul uchun quyidagi ma’lumotlar mavjud bo‘lishi kerak:

- PORT
- DATABASE_URL
- JWT_SECRET
- API_BASE_URL
- ENV mode (`development`, `staging`, `production`)

Barcha maxfiy ma’lumotlar `.env.example` yoki xuddi shunday namunaviy fayl orqali yoziladi.

## 5. Test va tekshirish

Loyihada quyidagi bosqichlar bo‘lishi kerak:

- unit test
- integration test
- lint / formatting
- build check

Masalan:

```bash
npm run lint
npm run test
npm run build
```

## 6. Hissa qo‘shish

O‘zgarishni boshlashdan oldin yangi branch oling:

```bash
git checkout -b feature/feature-name
```

Keyin kichik, tamoyili va aniq commitlar yozing. Pull request ochishda:

- muammoni aniq ayting;
- yechim nimadan iborat ekanini izohlang;
- tekshirish bosqichlarini ko‘rsating;
- kerak bo‘lsa screenshot yoki demo havolani qo‘shing.

## 7. Kelajakda kerak bo‘ladigan texnik birliklar

Yulemdo ekotizimi rivojlanar ekan, quyidagi qoliplarga ehtiyoj paydo bo‘ladi:

- auth service
- user profile service
- search API
- notifications
- CMS / admin panel
- analytics
- developer portal
- webhook system

Bu xizmatlar bir-biriga to‘g‘ri va xavfsiz integratsiyalanishi kerak.

## 8. Xulosa

Yulemdo ekotizimi uchun muhim jihat — tizimning barcha qismi bir-biriga bog‘langan, xavfsiz, o‘zbek tiliga mos va kelajakga yo‘l ochadigan arxitekturani yaratishdir. Hujjatlarni muntazam yangilab borish loyiha boshqaruvini osonlashtiradi.
