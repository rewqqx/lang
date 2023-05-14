# Lang
 
Идея - язык с помощью Python без использования библиотек

## Функционал
### Декларирование
1. Переменные
2. Функции
### Утверждения
1. if конструкция (+else if, +else)
2. while конструкция
3. for конструкция
4. вывод
5. назначение
### Выражения
1. отрицательный унарный оператор
2. унарный оператор "not"
3. умножение
4. деление
5. возведение в степень
6. сложение
7. вычитание
8. меньше или равно
9. больше или равно
10. меньше
11. больше
12. равенство
13. неравенство
14. and
15. or
### Поддреживает
1. целые числа
2. числа с плавающей точкой
3. строки
4. списки (append, pop, extend, len)
5. проверка на тип (is_num, is_list, is_fun, is_str)

### Запуск
1. Запустить shell.py
2. Ввести ```RUN("example.lang")``` 
```
# Пример кода

FUN oopify(prefix) -> prefix + "est"

FUN join(elements, separator)
	VAR result = ""
	VAR len = LEN(elements)

	FOR i = 0 TO len THEN
		VAR result = result + elements/i
		IF i != len - 1 THEN VAR result = result + separator
	END

	RETURN result
END

FUN map(elements, func)
	VAR new_elements = []

	FOR i = 0 TO LEN(elements) THEN
	    IF i == 0 THEN
	       CONTINUE
	    END
		APPEND(new_elements, func(elements/i))
	END


	RETURN new_elements
END

PRINT("Hello, world!")


FOR i = 0 TO 5 THEN
	PRINT(join(map(["T", "V"], oopify), ", "))
END

VAR i = 2
IF NOT i THEN
    PRINT(i)
ELIF i == 1 THEN
    PRINT(i)
ELSE
    PRINT(i)
END
```
Вывод:
```
Hello, world!
Vest
Vest
Vest
Vest
Vest
2
0
```

### Ресурсы
Делал по гайду: https://ruslanspivak.com/lsbasi-part1/
