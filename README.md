Кристијан Блажевски 203166

Цикломатската комплексност

M=E−N+2P
E е бројот на ребра (edges) во графот.

N е бројот на јазли (nodes) во графот.

P е бројот на поврзани компоненти (за една функција, 𝑃=1).

Пресметка:
Јазли N = 14 

Ребра E = 25

Поврзани компоненти (P) = 1

РЕБРА(Е)

1. Start -> if (allItems == null)
2. if (allItems == null) -> throw new RuntimeException (true)
3. if (allItems == null) -> Initialize sum = 0 (false)
4. Initialize sum = 0 -> for each item in allItems
5. for each item in allItems -> if (item.getName() == null || item.getName().length() == 0)
6. if (item.getName() == null || item.getName().length() == 0) -> item.setName("unknown") (true)
7. if (item.getName() == null || item.getName().length() == 0) -> if (item.getBarcode() != null) (false)
8. item.setName("unknown") -> if (item.getBarcode() != null)
9. if (item.getBarcode() != null) -> throw new RuntimeException (false)
10. if (item.getBarcode() != null) -> Check if barcode contains only numbers (true)
11. Check if barcode contains only numbers -> throw new RuntimeException (true)
12. Check if barcode contains only numbers -> if (item.getDiscount() > 0) (false)
13. if (item.getDiscount() > 0) -> sum += item.getPrice() * item.getDiscount() (true)
14. if (item.getDiscount() > 0) -> sum += item.getPrice() (false)
15. sum += item.getPrice() * item.getDiscount() -> if (item.getPrice() > 300 && item.getDiscount() > 0 && item.getBarcode().charAt(0) == '0')
16. sum += item.getPrice() -> if (item.getPrice() > 300 && item.getDiscount() > 0 && item.getBarcode().charAt(0) == '0')
17. if (item.getPrice() > 300 && item.getDiscount() > 0 && item.getBarcode().charAt(0) == '0') -> sum -= 30 (true)
18. if (item.getPrice() > 300 && item.getDiscount() > 0 && item.getBarcode().charAt(0) == '0') -> Next item (false)
19. sum -= 30 -> Next item
20. Next item -> for each item in allItems
21. for each item in allItems -> if (sum <= payment) (loop exits)
22. if (sum <= payment) -> return true (true)
23. if (sum <= payment) -> return false (false)
24. return true -> End
25. return false -> End

M=25−13+2×1

M=13
