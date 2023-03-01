# Linux_h_w.02
Используя команду cat, создать два файла с данными, а затем объединить их. 

	cat > testfile 
	cat > test2
	cat testfile test2 > test_all

Просмотреть содержимое созданного файла.
	
	ll

Переименовать файл, дав ему новое имя
	
	mv test_all test3

Создать несколько файлов. Создать директорию, переместить файл туда. 
Удалить все созданные в этом и предыдущем задании директории и файлы.

	touch test4
	touch test5
	mkdir test_file
	mv test5 test_file
	rm  -fr


Создать файл file1 и наполнить его произвольным содержимым. 
Скопировать его в file2. Создать символическую ссылку file3 на file1. 
Создать жесткую ссылку file4 на file1. Посмотреть, какие айноды у файлов. Удалить file1.

	cat > file1 
awdadawdawdawdawd
awdawdawdawdawdaw
	Ctrl+d
	cp -r file1 file2
	ln -s test2 file1
	ln file4 file1
	ls -ali
	rm file1


Что стало с остальными созданными файлами? 
Попробовать вывести их на экран.
	
	file2 остался без изменений

	file3 -> file1 остался, но выделен красным

	file4 остался без изменений


Дать созданным файлам другие, произвольные имена. 
Создать новую символическую ссылку. 
Переместить ссылки в другую директорию.
	
	mv file2 new_file2
	mv file3 new_file3
	mv file4 new_file4

	ln -s new_file2 new_file2_link

	mv new_file2_link /tmp/
	mv new_file3 /tmp/
	mv new_file4 /tmp/















