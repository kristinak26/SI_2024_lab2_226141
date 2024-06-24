# SI_2024_lab2_226141
Кристина Каранфиловска 
226141

1.
![Control Flow Graph](https://github.com/kristinak26/SI_2024_lab2_226141/blob/master/Screenshot%202024-06-24%20182146.png?raw=true)

2.Цикломатската комплексност на овој код е 10,ја добив преку формулата P+1, каде што P е бројот на предикатни јазли. Во случајoв P=9 {има 9 if и for јазли}, па комплексност изнесува 10.

3,Тест случаи според критериумот Every Branch
![Every Branch](https://github.com/kristinak26/SI_2024_lab2_226141/blob/master/Screenshot%202024-06-24%20181756.png?raw=true)
4.![Multiple Condition](https://github.com/kristinak26/SI_2024_lab2_226141/blob/master/Screenshot%202024-06-24%20185559.png?raw=true)

Објаснување на напишаните unit tests every branch

allItems = null фрлa RuntimeException("allItems list can't be null!")

"allItems=[Item(null, ""1111"", 300, 0.50), Item(""Item2"", ""2222"", 350, -1)]  payment=10000;" 2 објекти, програмата заврсшува со true

"allItems=[Item(null, ""2222"", 350, 0.500), Item(""Item2"", ""666"", 350, -1)] payment=10;" 2 објекти и голема вредност за payment, програмата завршува со false

"allItems=[Item("""", ""hhhh"", 100, -1),
payment=100;" not valid Barcode -> фрла RuntimeException ("Invalid character in item barcode!")

"allItems=[Item(null, null , 100, -1),
payment=100;" null Barcode и Name -> фрлa RuntimeException ("No barcode!")
-multiple condition

allItems = [Item(Name = a, Barcode = 0001, Price = 355, Discount = 0.5)], payment = 145 TTT - сите се труе и програмата продолжува во if

allItems = [Item(Name = a, Barcode = 125, Price = 355, Discount = -1)], payment = 146 TFF - програмата нема да продолжи во if

allItems = [Item(Name = a, Barcode = 125, Price = 355, Discount = 0.5)], payment = 147 TTF - програмата нема да продолжи во if

allItems = [Item(Name = a, Barcode = 125, Price = 200, Discount = -1)], payment = 148 FXX - програмата нема да продолжи во if
