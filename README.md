Marija Joveva 223018

Control Flow Graph

![Untitled Diagram drawio (1)](https://github.com/marijajoveva/SI_2024_lab2_223018/assets/165589124/4021e30a-9458-4191-9118-ace085c2fa77)


Цикломатска комплексност
- Цикломатската комплексност на овој код е 10, истата ја добив преку формулата P+1, каде што P е бројот на предикатни јазли. Во случајoв P=9, па цикломатската комплексност изнесува 10.

Тест случаи според Every Branch критериумот
1. []
2. Item("Klupa", "V4",350, 10.0), payment = 200
3. Item("Ogledalo" , "74", 450,5.0), payment = 2000
4. Item("Tetratka" ,"", 100,4.0), payment = 50
5. Item("Maica" , "07", 320, 0.0), payment = 300
6. Item("" ,"05", 420, 7.5), payment = 80

![image](https://github.com/marijajoveva/SI_2024_lab2_223018/assets/165589124/ce57db57-3a4e-41c6-b4f2-dd5f99d7bc6d)



Тест случаи според Multiple Condition критериумот

if (item.getPrice) > 300 && item.getDiscount() > 0 && item.getBarcode.charAt(0) == '0')

Можни услови:

F && X && X -> item.getPrice() <= 300, item.getDiscount() = anything, item.getBarcode.charAt0)=anything

T && F && X -> item.getPrice() >= 300, item.getDiscount() <=0, item.getBarcode().chatAt(0)= anything

T && T && T → item.getPrice() >= 300, item.getDiscount() > 0, item.getBarcode0.charAt(0) == '0'



