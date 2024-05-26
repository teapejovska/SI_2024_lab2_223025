Теа Пејовска 223025

![graf](https://github.com/teapejovska/SI_2024_lab2_223025/assets/147940760/87f7162e-733d-4c51-aac1-aac5db6cef5c)

Цикломатска комплексност
3. Цикломатската комплексност е 10
        Предикатни јазли 9 9+1=10
        Региони = 9  9+1=10
        Јазли = 28
        Ребра = 36
        Цикломатска комплексност = (36-28)+2 = 8+2=10

Тест случаи според критериумот Every statement
4. За тестирање на кодот ми беа потребни 5 тест случаи
   Test Case 1: allitems[null], 100 //allItems == null
   Test Case 2: allitems[], 0  //празна листа
   Test Case 3: allitems["Item1", "1234567890", 150, 0
                         "Item2", "0234567895", 400, 15
                         "     ", 1q25qs563s  , 400, 0] , 100
   Test Case 4: allitems["Item3", "1234567890", 400, 0
                         "Item4", "0234567895", 700, 15
                         "Item5",             , 180, 20], 100
   Test Case 5: allitems["Item6", "8974154655", 300 0
                         "Item7", "0698481645", 800, 15
                         "Item8", "8546168413", 600, 20], 100

5. Според Multiple Condition критериумот потребни се 8 тест случаи:
   1. Т Т Т (item.getPrice() = 350, item.getDiscount() = 10, item.getBarcode() = "012345")
   2. T T F (item.getPrice() = 350, item.getDiscount() = 10, item.getBarcode() = "112345")
   3. T F T (item.getPrice() = 350, item.getDiscount() = 0, item.getBarcode() = "012345")
   4. T F F (item.getPrice() = 350, item.getDiscount() = 0, item.getBarcode() = "112345")
   5. F T T (item.getPrice() = 250, item.getDiscount() = 10, item.getBarcode() = "012345")
   6. F T F (item.getPrice() = 250, item.getDiscount() = 10, item.getBarcode() = "112345")
   7. F F T (item.getPrice() = 250, item.getDiscount() = 0, item.getBarcode() = "012345")
   8. F F F (item.getPrice() = 250, item.getDiscount() = 0, item.getBarcode() = "112345")

Објаснување на unit tests
6.
Според барањето треба да се напишат две функциии за unit тестирањето. При правење на овие две функции како критериум ги користев
1.Тестирање на гранични случаи и влезови - testNullAndEmptyList
        Test Case 1: Проверка дали програмата правилно фрла исклучок кога листата allItems е null.
        Тest Case 2: Проверка дали програмата правилно враќа true кога листата allItems е празна.

2.Тестирање на преостанатите услови во кодот -testVariousItems
        Test Case 3: Проверка дали програмата фрла исклучок кога баркодот содржи невалидни карактери.
        Test Case 4: Проверка дали програмата фрла исклучок кога предметот нема баркод.
        Test Case 5: Проверка на комбинација од предмети со и без попусти и дали програмата правилно ја пресметува сумата и враќа точен резултат според сумата што треба да се плати.

Со комбинирањето на тестовите на овој начин, се осигуруваме дека сите важни гранични случаи и услови се покриени со минимален број на тест функции, што го прави тестирањето поефикасно.
