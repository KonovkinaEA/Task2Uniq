# Uniq
Объединение последовательностей одинаковых идущих подряд строк в файле в одну:
- Флаг `file`задает имя входного файла. Если параметр отсутствует, следует считывать текст с консоли
- Флаг `-o ofile` задает имя выходного файла. Если параметр отсутствует, следует выводить результаты на консоль
- Флаг `-i` означает, что при сравнении строк следует не учитывать регистр символов
- Флаг `-s N` означает, что при сравнении строк следует игнорировать первые N символов каждой строки. Выводить нужно первую строку
- Флаг `-u` означает, что следует выводить в качестве результата только **уникальные** строки
- Флаг `-c` означает, что перед каждой строкой вывода следует вывести количество строк, которые были заменены данной (т.е. если во входных данных было 2 одинаковые строки, в выходных данных должна быть одна с префиксом "2")

Command line: uniq [-i] [-u] [-c] [-s num] [-o ofile] [file]

В случае, когда какое-нибудь из имен файлов указано неверно, следует выдать ошибку
