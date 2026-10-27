# ZERO//TRUST: Korporativ xavfsizlik platformasi (simulyatsiya)

Zero Trust ("hech kimga ishonma, har doim tekshir") xavfsizlik modelini o'rgatish uchun interaktiv veb-sahifa. Sahifa o'quv maqsadida yaratilgan simulyatsiya: barcha foydalanuvchilar, qurilmalar va qarorlar sun'iy ma'lumotdir va haqiqiy tarmoqqa ulanmaydi.

## Bo'limlar

- **Boshqaruv paneli**: 240 ta sun'iy kirish so'rovi, qarorlar taqsimoti va xavfsizlik holati bahosi.
- **Siyosat simulyatori**: so'rov shartlarini o'zgartirib, qaror va xavf bahosini kuzatish. Qoidalar va tuzatish tavsiyalari ko'rsatiladi.
- **Senariylar**: sakkizta tayyor vaziyat, ularni simulyatorga yuklash mumkin.
- **Savol-javob**: Zero Trust bo'yicha savollar, qidiruv va bilim tekshiruvi testi.
- **Monitoring**: talabalar ismi bilan kiradi, test va simulyator harakatlari yoziladi. Natijalarni JSON fayl sifatida yuklab olish va boshqa fayllarni yuklab, umumiy jadval hosil qilish mumkin.

## Ishga tushirish

Hech qanday o'rnatish talab etilmaydi. `index.html` faylini brauzerda oching.

## GitHub Pages orqali nashr qilish

1. Repozitoriy yarating (masalan, `zero-trust-sim`) va `index.html` faylini ildiz papkasiga yuklang.
2. Repozitoriy sahifasida **Settings → Pages** bo'limiga o'ting.
3. **Source** qismida `Deploy from a branch` ni tanlang, branch sifatida `main` va papka sifatida `/ (root)` ni belgilang, so'ng **Save** bosing.
4. Bir necha daqiqadan so'ng sayt `https://<foydalanuvchi-nomi>.github.io/<repozitoriy-nomi>/` manzilida ochiladi.

Terminal orqali yuklash uchun:

```bash
git init
git add index.html README.md
git commit -m "ZERO//TRUST simulyatsiya sayti"
git branch -M main
git remote add origin https://github.com/<foydalanuvchi-nomi>/<repozitoriy-nomi>.git
git push -u origin main
```

## Muhim eslatmalar

- Monitoring ma'lumotlari har bir brauzerning `localStorage` xotirasida saqlanadi. Ma'lumotlar serverga yuborilmaydi, shuning uchun bir nechta qurilmadagi natijalar avtomatik birlashmaydi. Ularni fayl orqali yig'ish kerak.
- Sayt shriftlarni Google Fonts'dan yuklaydi. Internet ulanishi kerak.
- Bu sayt ta'lim maqsadida yaratilgan. Haqiqiy avtorizatsiya, identifikatsiya va jurnallash tizimi o'rnini bosmaydi.

## Manba

NIST SP 800-207, Zero Trust Architecture.
