1. 	Перевірити в якій директорії зараз знаходжуся
```bash
Команда pwd  - print working directory
```
 

2. Створити нову папку (назва на свій вибір) командою mkdir  - make directory і перевірити чи створилась  папка командою ls -  list
 ```bash
 mkdir g_4
 ```

3. Зайти в папку 
 ```bash
 cd g_4
 ```


4. Створити папки 
Командою mkdir (назва_1, назва_2, назва_3) створити папки та командою ls та перевірити їх наявність
 ```bash
 mkdir gg_1 gg_2 gg_3
 ```
5. Зайти в папку gg_1
```bash
cd gg_1
```
 
6. 	Створити три текстових файли та двох файлів json
```bash
touch t_item1.txt t_item2.txt t_item3.txt j_item1.json j_item2.json
```

7. Cтворити 3 папки
```bash
mkdir ggg_1 ggg_2 ggg_3
```
8. Вивести список змісту
```bash
ls -la
```


9/10/11. Зайти в  файл t_item1.txt и зробити запис в файлі в редакторі vim, зберегти файл (натиснути escape + команда :qw)
 ```bash
 vim t_item1.txt
 ```

12.Вийти на рівень вище за допомогою cd ..
 ```bash
 cd ..
 ```

13.Переміщення файлів в другий каталог:
```bash
mv gg_1/j_item1.json gg_2/j_item1.json
mv gg_1/j_item2.json gg_2/j_item2.json
```
 
 14. Копіювання любих 2-х файлів які ви створили,в любу іншу папку
 ```bash
 cp gg_2/j_item1.json gg_3/j_item1.json
 cp  gg_2/j_item2.json gg_3/j_item2.json
 ```
 
 

15) Пошук файлу по імені 
 ```bash
Знайти всі файли  с розширенням txt
Команда find /имя директории/ “*.txt” -  найти все файлы  с расширением txt
```
```bash
find . -name "j_item1.json"
```

16) Передивитися вміст в реальному часі (використання команд tail і grep для мониторинга нових строк с заданим умовою пошуку)
```bash
grep test t_item1.txt
```
```bash
tail -f t_item1.txt | grep test
```

 
17) Вивести декілька строк з текстового файлу:
```bash
head -3 t_item1.txt
```

 
18) Вивести декілька  останніх строк з файлу
```bash
tail –3 t_item1.txt
```
 
19) команда less для перегляду вмісту файла.Дозволяє здійснювати пошук по файлу згідно заданому шаблону.Використовується тільки для перегляду , але не зміна файлу!
```bash
less t_item1.txt
Ctrl+Z
```

20) вивести дату та час (команда date)
```bash
date
```

 



*
1) Відправити запит на сервер http://162.55.220.72:5005/terminal-hw-request
```bash
curl http://162.55.220.72:5005/terminal-hw-request
```
2) Написати скріпт який виконає автоматично пункти 3,4,5,6,7,8,13
Створити скріпт ./myscript1.bash і через vim редактор ввести ці команди:
```bash
#!/bin/bash
cd /c/Users/Admin/gitbash_31/g_4/gg_1/
echo "The current directory is:"
pwd
echo "Creating a new directory"
mkdir my_script
echo "Open new directory"
cd my_script
echo "Creating new directories"
mdir test_1 test_2 test_3
echo "Open new directory"
cd test_1
echo "Creating new files"
touch file_1.txt file_2.txt file_3.txt j_file1.json j_file2.json
echo "Show all files in this directory"
mv test/file_1.txt test_1/file_2.txt test_2
```
 

 




