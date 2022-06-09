# Terminal
1) Посмотреть где я
>**pwd**
2) Создать папку
>**mkdir new_folder**
3) Зайти в папку
>**cd new_folder**
4) Создать 3 папки
>**mkdir new_folder1 new_folder2 new_folder3**
5) Зайти в любоую папку
>**cd new_folder1**
6) Создать 5 файлов (3 txt, 2 json)
>**touch file1.txt file2.txt file3.txt file4.json file5.json**
7) Создать 3 папки
>**mkdir new_folder4 new_folder5 new_folder6**
8. Вывести список содержимого папки
>**ls -la**
9) + Открыть любой txt файл
>**vim file1.txt**
10) + написать туда что-нибудь, любой текст.
>**i**
```txt
С точки зрения банальной эрудиции, не каждый индивидуум, критически метафизирующий абстракции, способен опровергнуть тенденции парадоксальных эмоций.
```
11) + сохранить и выйти.
>**Esc**

>**:wq**
12) Выйти из папки на уровень выше
>**cd ..**
13) переместить любые 2 файла, которые вы создали, в любую другую папку.
>**mv file1.txt new_folder4/file1.txt**

>**mv file2.txt new_folder5/file2.txt** 
14) скопировать любые 2 файла, которые вы создали, в любую другую папку.
>**cp new_folder4/file1.txt new_folder5/file1.txt**

>**cp new_folder5/file2.txt new_folder4/file2.txt**
15) Найти файл по имени
>**find . -name file3.txt**
16) просмотреть содержимое в реальном времени (команда grep) изучите как она работает.
>**grep "Привет" file3.txt**
17) вывести несколько первых строк из текстового файла
>**head -3 file3.txt**
18) вывести несколько последних строк из текстового файла
>**tail -3 file3.txt**
19) просмотреть содержимое длинного файла (команда less) изучите как она работает.
>**less file3.txt**

>**q**
20) вывести дату и время
>**date**

Задание *
1) Отправить http запрос на сервер.
http://162.55.220.72:5005/terminal-hw-request
>**curl http://162.55.220.72:5005/terminal-hw-request**
2) Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13
```css
cat > my_script.sh << EOF
#!/bin/bash
mkdir folder_script
cd folder_script
mkdir folder1 folder2 folder3
cd folder1
touch text1.txt text2.txt text3.txt json4.json json5.json
mkdir script_folder1 script_folder2 script_folder3
ls -la
mv text1.txt script_folder1/text1.txt
mv text2.txt script_folder1/text2.txt
EOF
```
`Enter`

`./my_script.sh`
