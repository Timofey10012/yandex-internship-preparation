# Задача: Планирование разгрузки грузовиков

На складе стоит N грузовиков. Каждый грузовик хочет заехать на платформу, но у каждого есть своё окно во времени, когда он может это сделать. Платформа вмещает только один грузовик одновременно и работает в течение T минут с момента открытия.  
У каждого грузовика:
- l_i — момент, когда он готов заехать
- r_i — момент, до которого он может ждать
(оба включительно)
 
Считается, что грузовик успеет заехать, если он может заехать в свободную минуту, не раньше l_i и не позже r_i, и платформа ещё не закрыта. 

## Ввод:

- N — количество грузовиков
- T — количество минут с момента открытия
- l_i — момент, когда он готов заехать
- r_i — момент, до которого он может ждать
(оба включительно)

┍---------┒  
&nbsp;&nbsp;&nbsp;&nbsp;N T  
&nbsp;&nbsp;&nbsp;&nbsp;l_1 r_1  
&nbsp;&nbsp;&nbsp;&nbsp;l_2 r_2  
&nbsp;&nbsp;&nbsp;&nbsp;...  
&nbsp;&nbsp;&nbsp;&nbsp;l_N r_N  
┗---------┛  

- 1 ≤ N ≤ 10^5
- 1 ≤ T ≤ 10^9
- 0 ≤ l_i ≤ r_i ≤ 10^9

## Вывод:
Вывести N строк:
В i-й строке — Yes, если i-й грузовик может заехать, иначе — No.

# Пример:
Ввод: &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Вывод:  
4 5  
0 10 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Yes  
2 3 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Yes  
6 7 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; No  
4 9 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Yes   
