<img src="./icon.png" align="right" />

# `<!DOCTYPE html>` - nima?

- `!doctype` - sahifani browser tomonidan qanday formatda o'qib berishini belgilab beradi. Hozirda biz ishlatadigan format `html`, ammo boshqa formatlar ham mavjum. Masalan: `XHTML`, `Framesets`.

# HTML da `<head>` va `<body>` teglarinig farqi qanday?

- `<head>` tegi - sahifa haqidagi ma'lumotlarni, masalan meta teglar, stillar, faviconlar, title.
- `<body>` tegi - sahifaning asosiy kontentlarini o'z ichiga oladi. <br>
  
  **P.S. Texik tarafdan qaralganda, `html` tepadan pastga qarab o'qib keladi. `<head>` esa birinchi bo'lib o'qiladi.** 


# Teg turlari: Inline va Block teglarning farqi? 

- Har bir `html` elementlarining default display xossasi mavjud. Bu teg turlariga qarab inline va block bo'lishi mumkin. Block elementni inline element ichida yozish mumkin emas va unday qilish xato!
    * Block elementlar o'zining sahifadagi to'liq qatorini egallaydi.
    * Inline elementlar o'zining kontentiga mos joyni egallaydi.

# Meta tegalar orqali nimalar qila olamiz?

- Meta teglar sahifa haqidagi ma'lumotlarni ulash uchun ishlatiladi. Shuningdek ularni ishlatishdan yana bir asosiy maqsad SEOni rivojlantirish bo'ladi. Ya'ni, masalan Googledan qidirganda sahifangizni qidiruvda topish uchun Google aynan shu teglardagi ma'lumotlardan foydalanadi(yana boshqa ma'lumotlardan ham).

# Css fayllarni ulash tartibi qanday?

- Dastur talabidan kelib chiqib har-xil yo'llari bor, masalan:
  1. inline 
  2. internal(Critical css)
  3. external

# JavaScript fayllarni ulsh tartibi qanday? 

  1. JS fayllar `<body>` tegi oxirida yoki `<head>` tegi ichida.
  2. JS fayllar kerakli qismini  `<body>` tegi oxirida. Qolganini asinxron yuklash. Yoki hammasini asinxron yuklash.

   ``` js
   // Async yuklanishi bilan ishlaydi. HTML o'qib bo'linishini(parsing) kutib turmaydi.    
   // Ishlashni boshlaganida **parser** bloklanadi.
   <script async src="script.js">

   // Defer yuklanganidan so'ng HTML to'liq o'qib bo'linishini kutib turadi. 
   // Ishlashni boshlaganida **parser** bloklanmaydi.   
   <script defer src="script.js">