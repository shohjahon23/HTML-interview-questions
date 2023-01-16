<img src="./icon.png" align="right" />

## `<!DOCTYPE html>` - nima?

- `!doctype` - sahifani browser tomonidan qanday formatda o'qib berishini belgilab beradi. Hozirda biz ishlatadigan format `html`, ammo boshqa formatlar ham mavjum. Masalan: `XHTML`, `Framesets`.

## HTML da `<head>` va `<body>` teglarinig farqi qanday?

- `<head>` tegi - sahifa haqidagi ma'lumotlarni, masalan meta teglar, stillar, faviconlar, title.
- `<body>` tegi - sahifaning asosiy kontentlarini o'z ichiga oladi. <br>
  
  **P.S. Texik tarafdan qaralganda, `html` tepadan pastga qarab o'qib keladi. `<head>` esa birinchi bo'lib o'qiladi.** 


## Teg turlari: Inline va Block teglarning farqi? 

- Har bir `html` elementlarining default display xossasi mavjud. Bu teg turlariga qarab inline va block bo'lishi mumkin. Block elementni inline element ichida yozish mumkin emas va unday qilish xato!
    * Block elementlar o'zining sahifadagi to'liq qatorini egallaydi.
    * Inline elementlar o'zining kontentiga mos joyni egallaydi.

## Meta tegalar orqali nimalar qila olamiz?

- Meta teglar sahifa haqidagi ma'lumotlarni ulash uchun ishlatiladi. Shuningdek ularni ishlatishdan yana bir asosiy maqsad SEOni rivojlantirish bo'ladi. Ya'ni, masalan Googledan qidirganda sahifangizni qidiruvda topish uchun Google aynan shu teglardagi ma'lumotlardan foydalanadi(yana boshqa ma'lumotlardan ham).

## Css fayllarni ulash tartibi qanday?

- Dastur talabidan kelib chiqib har-xil yo'llari bor, masalan:
  1. inline 
  2. internal(Critical css)
  3. external

## JavaScript fayllarni ulash tartibi qanday? 

  1. JS fayllar `<body>` tegi oxirida yoki `<head>` tegi ichida.
  2. JS fayllar kerakli qismini  `<body>` tegi oxirida. Qolganini asinxron yuklash. Yoki hammasini asinxron yuklash.

``` js
    // Async yuklanishi bilan ishlaydi. HTML o'qib bo'linishini (parsing) kutib turmaydi.    
    // Ishlashni boshlaganida parser bloklanadi.
    <script async src="script.js"></script>

    // Defer yuklanganidan so'ng HTML to'liq o'qib bo'linishini kutib turadi. 
    // Ishlashni boshlaganida parser bloklanmaydi.   
    <script defer src="script.js"></script>
```
## HTMLda Accessibility tushunchasi nima? 

- Dasturni boshqa texnalogiyalar to'g'ri o'qishini oson qilish bu accessibility deyiladi. Masalan Screenreaders, search engine va hkz. Asosiy maqsadlardan biri, nogiron insonlarga qulayliklar yaratish. 
  1. Perceivable (Hamma saytdagi ma'lumotlarga ega bo'la olishi. Ko'r inson eshita olishi, kar inson ko're olishi, texnik muammolari bor inson boshqa yo'llar orqali o'qiy olishi...)
  2. Operable (Sayt boshqaruvi hamma uchun mos bo'lishi.)
  3. Understandable (Sayt barcha uchun tushunarli bo'lishi)
  4. Robust (Sayt hozirgi va keyin kelishi mumkin bo'lgan qurilmalarda deyarli bir xil ishlashi.)
- Qanday qilib saytning accessibility qismini oshirish mumkin! 
  1. Alt teglar `<img src="url" alt="Rasm haqida ma'lumot">`
  2. Semantik elemantlar orqali. (keyingi savolda)
  3. Aria attributlar orqali. (keyingi savolda)
  4. Video/audio captions, autocomplete inputs, using keyboardsva hkz.

**Screen reader extension: Chrome Vox**

## Semantik elementlar nima?

- Semantik elementlar - nomidan odam va kompyuter tushunadigan qilib yozilgan elementlardir. Masalan: `<header>, <footer>, <main>, <section>, <nav>` va hkz. Ularning asl ustunliklari quyidagilar:

  1. O'qish va tushunishga oson.
  2. Accessibility oshiradi.

## HTMLda aria atributlarning o'rni qanday?

- Aria(Accessible Rich Internet Applications) atributlar saytni ko'zi ojiz insonlar ishlatishi oson bo'lishi uchun ishlatiladigan atributlar to'plami. Screen readerlar aria atributlarni dasturni ko'zi ojiz insonlarga to'gri va tushunarli o'qib berish uchun foydalanishadi.