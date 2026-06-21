# Python Mashqlari — 60 ta amaliy masala

Quyida siz bergan mavzular bo'yicha jami **60 ta masala** tayyorlandi. Har bir masaladan keyin tushunish uchun qisqacha **misol** (kirish/chiqish) berildi — lekin yechimni o'zingiz yozasiz.

---

## 1. Numbers
1. Ikki sonni kiritib, ularning yig'indisi, ayirmasi, ko'paytmasi va bo'linmasini hisoblang.
   *Misol:* kiritildi `8` va `3` → yig'indi `11`, ayirma `5`, ko'paytma `24`, bo'linma `2.67`
2. Berilgan sonning tub son (prime) ekanligini tekshiruvchi dastur yozing.
   *Misol:* kiritildi `17` → `"17 — tub son"`; kiritildi `15` → `"15 — tub son emas"`

## 2. List
3. Berilgan ro'yxatdagi eng katta va eng kichik elementni toping (`max()`/`min()` funksiyasidan foydalanmasdan).
   *Misol:* `[4, 9, 2, 7, 1]` → eng katta `9`, eng kichik `1`
4. Ro'yxatdagi takrorlanuvchi elementlarni olib tashlang.
   *Misol:* `[1, 2, 2, 3, 4, 4, 5]` → `[1, 2, 3, 4, 5]`
5. Ro'yxatni teskari tartibda chiqaring (`reverse()` yoki slicing'dan foydalanmasdan, faqat `for` loop bilan).
   *Misol:* `[10, 20, 30]` → `30, 20, 10`

## 3. Nested List
6. 3x3 matritsani nested list ko'rinishida yarating va uning diagonal elementlari yig'indisini toping.
   *Misol:* `[[1,2,3],[4,5,6],[7,8,9]]` → diagonal yig'indi = `1+5+9 = 15`
7. Ikki nested listni (matritsalarni) element bo'yicha qo'shing.
   *Misol:* `[[1,2],[3,4]]` + `[[5,6],[7,8]]` → `[[6,8],[10,12]]`

## 4. List Slicing
8. Berilgan ro'yxatdan faqat juft index'dagi elementlarni slicing yordamida ajratib oling.
   *Misol:* `[10,20,30,40,50,60]` → `[10,30,50]`
9. Ro'yxatni teng ikkiga bo'lib, ikkinchi yarmini birinchisidan oldin chiqaring (slicing yordamida).
   *Misol:* `[1,2,3,4,5,6]` → `[4,5,6,1,2,3]`

## 5. List Comprehension
10. 1 dan 50 gachagi sonlardan faqat 3 ga bo'linadiganlarini list comprehension yordamida yig'ing.
    *Misol:* natija boshlanishi `[3, 6, 9, 12, ..., 48]`
11. Berilgan so'zlar ro'yxatidan faqat unli harf bilan boshlanadiganlarini ajratib oling.
*Misol:* `["olma","banan","anor","uzum"]` → `["olma","anor"]`
12. Ikki o'lchamli (nested) list comprehension yordamida 5x5 ko'paytirish jadvalini hosil qiling.
    *Misol:* 1-qator `[1,2,3,4,5]`, 2-qator `[2,4,6,8,10]`, ...

## 6. Tuple
13. Tuple ichidagi elementlarning chastotasini (necha marta takrorlangani) hisoblang.
    *Misol:* `(1,2,2,3,3,3)` → `{1:1, 2:2, 3:3}`
14. Ikkita tuple'ni birlashtirib, natijani saralangan (sorted) tuple sifatida qaytaring.
    *Misol:* `(3,1,2)` + `(6,4,5)` → `(1,2,3,4,5,6)`

## 7. Set
15. Ikki ro'yxatdagi umumiy (kesishgan) elementlarni set yordamida toping.
    *Misol:* `[1,2,3,4]` va `[3,4,5,6]` → `{3,4}`
16. Berilgan matndagi unique (takrorlanmaydigan) so'zlar sonini set yordamida hisoblang.
    *Misol:* `"olma anor olma uzum"` → unique so'zlar soni: `3`

## 8. Dictionary
17. Talabalar ismi va bahosi saqlangan dictionary yarating, eng yuqori bahoga ega talabani toping.
    *Misol:* `{"Ali":90, "Vali":85, "Soli":95}` → eng yuqori: `"Soli"`
18. Berilgan matndagi har bir harfning necha marta takrorlanganini dictionary'da saqlang.
    *Misol:* `"salom"` → `{'s':1,'a':1,'l':1,'o':1,'m':1}`
19. Ikki dictionary'ni birlashtiring, agar kalit takrorlansa qiymatlarini qo'shib chiqaring.
    *Misol:* `{"olma":5}` + `{"olma":3,"anor":2}` → `{"olma":8,"anor":2}`

## 9. Nested Dictionary
20. Har bir talabaning fanlar bo'yicha bahosini saqlaydigan nested dictionary yarating va o'rtacha bahoni hisoblang.
    *Misol:* `{"Ali": {"mat":90,"fizika":80}}` → o'rtacha: `85`
21. Nested dictionary ichida ma'lum bir kalitni qidirib, uning qiymatini yangilang.
    *Misol:* `{"Ali": {"mat":90}}` → `"mat"` qiymatini `95`ga o'zgartirish

## 10. Dict Comprehension
22. Berilgan ro'yxatdagi sonlarning kvadratini kalit-qiymat juftligida saqlovchi dict comprehension yozing.
    *Misol:* `[1,2,3,4]` → `{1:1, 2:4, 3:9, 4:16}`
23. Berilgan dictionary'dan faqat qiymati 50 dan katta bo'lgan juftliklarni ajratib oling.
    *Misol:* `{"a":40,"b":60,"c":80}` → `{"b":60,"c":80}`

## 11. String
24. Berilgan satrning palindrom (orqa-oldin bir xil o'qiladigan) ekanligini tekshiring.
    *Misol:* `"radar"` → palindrom; `"salom"` → palindrom emas
25. Matndagi har bir so'zning birinchi harfini katta qilib chiqaring (title case'ni qo'lda yozing).
    *Misol:* `"salom dunyo"` → `"Salom Dunyo"`
26. Berilgan satrdagi unlilar sonini hisoblang.
    *Misol:* `"Python dasturlash"` → unlilar soni: `5`

## 12. String Slicing
27. Berilgan satrni teskari tartibda chiqaring (slicing yordamida, `[::-1]`).
    *Misol:* `"Python"` → `"nohtyP"`
28. Satrning faqat har 2-harfini slicing yordamida ajratib oling.
    *Misol:* `"abcdefgh"` → `"aceg"`

## 13. If...Elif...Else
29. Foydalanuvchi kiritgan yoshga qarab "bola", "o'smir", "kattalar" yoki "keksa" toifasini aniqlang.
    *Misol:* yosh `15` → `"o'smir"`
30. Uchta sonni solishtirib, eng kattasini if-elif-else yordamida toping.
    *Misol:* `4, 9, 7` → eng katta: `9`

## 14. While Loop
31. `while` loop yordamida 1 dan 100 gachagi sonlar yig'indisini hisoblang.
    *Misol:* natija: `5050`
32. Foydalanuvchidan son kiritishni "stop" so'zi kiritilguncha davom ettiring va kiritilgan sonlar o'rtachasini chiqaring.
    *Misol:* kiritildi `10, 20, 30, stop` → o'rtacha: `20`

## 15. For Loop
33. 1 dan 10 gacha sonlarning faktorialini chiqaring.
    *Misol:* `5! = 120`
34. Fibonachchi ketma-ketligining birinchi 15 ta sonini chiqaring.
    *Misol:* `0,1,1,2,3,5,8,13,21,34,55,89,144,233,377`
35. Berilgan ro'yxatdagi har bir elementni o'z indexi bilan birga chiqaring (`enumerate` yordamida).
    *Misol:* `["olma","anor","uzum"]` → `0 olma`, `1 anor`, `2 uzum`

## 16. Break Statement
36. 1 dan 100 gacha sonlarni tekshirib, birinchi 7 ga bo'linadigan sonni topib `break` bilan to'xtatib chiqaring.
    *Misol:* natija: `7`
37. Ro'yxat ichida berilgan elementni qidiring, topilgach loop'ni `break` bilan to'xtating.
    *Misol:* `[3,7,9,12]` da `9` ni qidirish → `"9 topildi, index=2"`

## 17. Continue Statement
38. 1 dan 20 gacha sonlardan faqat toqlarini `continue` yordamida o'tkazib yuborib, juftlarini chiqaring.
    *Misol:* `2,4,6,8,...,20`
39. Ro'yxatdagi manfiy sonlarni `continue` bilan o'tkazib, faqat musbat sonlarning yig'indisini hisoblang.
    *Misol:* `[5,-3,8,-1,2]` → musbat yig'indi: `15`

## 18. Functions
40. Berilgan sonning faktorialini hisoblovchi funksiya yozing.
    *Misol:* `factorial(6)` → `720`
41. Ikki son orasidagi barcha tub sonlarni qaytaruvchi funksiya yozing.
    *Misol:* `10` dan `30` gacha → `[11,13,17,19,23,29]`
42. Default va keyword argumentlardan foydalanib, talaba ma'lumotlarini chiqaruvchi funksiya yarating.
    *Misol:* `student_info("Ali", age=20, course="Python")` → `"Ali, 20 yosh, Python kursi"`

## 19. Lambda Function
43. Lambda funksiya yordamida ikkita sonning ko'paytmasini hisoblang.
    *Misol:* `multiply = lambda x,y: x*y` → `multiply(4,5)` → `20`
44. Ro'yxatdagi sonlarni lambda funksiya yordamida kamayish tartibida saralang (`sorted()` + `key`).
    *Misol:* `[5,2,8,1]` → `[8,5,2,1]`

## 20. Variables Scope
45. Global va local o'zgaruvchilar orasidagi farqni ko'rsatuvchi dastur yozing (`global` kalit so'zidan foydalaning).
    *Misol:* global `x=10`, funksiya ichida `x`ni `20`ga o'zgartirish va natijani chiqarish
46. Funksiya ichida `nonlocal` kalit so'zidan foydalanib, ichki funksiyada tashqi funksiya o'zgaruvchisini o'zgartiring.
    *Misol:* tashqi funksiyada `count=0`, ichki funksiya orqali `count`ni `1`ga oshirish

## 21. Classes and Objects
47. `Car` klassini yarating: marka, model, narx atributlari va ma'lumotni chiqaruvchi metod bilan.
    *Misol:* `Car("Chevrolet","Cobalt",12000)` → `"Chevrolet Cobalt - $12000"`
48. `BankAccount` klassi yarating: pul qo'yish (`deposit`), yechish (`withdraw`) va balansni ko'rsatish metodlari bilan.
    *Misol:* `deposit(500)`, `withdraw(200)` → balans: `300`
49. `Book` klassidan bir necha obyekt yaratib, ularni ro'yxatda saqlang va narxi bo'yicha saralang.
    *Misol:* `[Book("A",20), Book("B",10)]` → narx bo'yicha: `B, A`

## 22. Inheritance
50. `Animal` klassidan `Dog` va `Cat` klasslarini meros qilib oling, har biri uchun `sound()` metodini qayta yozing (override).
    *Misol:* `Dog().sound()` → `"Vov-vov"`, `Cat().sound()` → `"Miyov"`
51. `Person` klassidan `Student` klassini meros qilib oling, qo'shimcha "fakultet" atributi bilan.
    *Misol:* `Student("Ali", 20, "IT fakulteti")`
52. `Shape` klassidan `Circle` va `Rectangle` klasslarini hosil qiling, har biri o'z yuzasini hisoblaydigan metodga ega bo'lsin.
    *Misol:* `Circle(5).area()` → `78.5`, `Rectangle(4,6).area()` → `24`

## 23. Read/Write Txt Files
53. Foydalanuvchidan kiritilgan matnni `notes.txt` fayliga yozib saqlang.
    *Misol:* kiritildi `"Bugun Python o'rgandim"` → fayl yaratiladi va matn saqlanadi
54. `notes.txt` faylini o'qib, undagi qatorlar sonini va so'zlar sonini hisoblang.
    *Misol:* fayl 3 qatordan, 10 so'zdan iborat → `"3 qator, 10 so'z"`

## 24. Read/Write CSV Files
55. Talabalar ismi va bahosini o'z ichiga olgan ma'lumotlarni `students.csv` fayliga yozing.
    *Misol:* faylga `Ali,90` va `Vali,85` qatorlari yoziladi
56. `students.csv` faylini o'qib, eng yuqori bahoga ega talabani aniqlang.
    *Misol:* fayldan `"Ali,90"` eng yuqori ekanligi topiladi
57. CSV fayldagi ma'lumotlarni dictionary ko'rinishida (`DictReader`) o'qib, ekranga chiqaring.
    *Misol:* `{'ism': 'Ali', 'baho': '90'}`

## 25. Exception Handling
58. Foydalanuvchidan son kiritishni so'rang va agar son emas narsa kiritilsa, `try-except` yordamida xatolikni ushlang.
    *Misol:* kiritildi `"abc"` → `"Xato: bu son emas!"`
59. Nolga bo'lish (`ZeroDivisionError`) xatoligini `try-except-finally` bilan boshqaring.
    *Misol:* `10/0` → `"Xatolik: nolga bo'lib bo'lmaydi"`, so'ng `"Dastur tugadi"`
60. Maxsus (custom) exception klass yaratib, berilgan yosh manfiy bo'lsa shu xatolikni chaqiring (`raise`).
    *Misol:* `yosh=-5` → `raise NegativeAgeError("Yosh manfiy bo'lishi mumkin emas")`

---

**Maslahat:** Har bir masalani yechishdan oldin, avval qog'ozda yoki izoh sifatida algoritmni qisqacha yozib oling, keyin kodga o'tkazing. Agar biror masalada qiynalsangiz, ayting — birga ko'rib chiqamiz.
