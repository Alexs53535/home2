# 1. Создать каталоги students и mentors в домашней директории, а в них — текстовые файлы students_list.txt и mentors_list.txt соответственно.
# создадим нужные папки
mkdir students
mkdir mentors

# 2. заполнить файлы данными
# заполним студентов
cat > students_list.txt << stop
Иван Диванов
Наталья Братан
Акиф Мамед Гадим Оглы
stop

# заполним наставников
cat > mentors_list.txt << stop
Cтивен Хокинг
Альберт Эйнштейн
stop


#	3. Переместите файл mentors_list.txt в папку students.
mv mentors/mentors_list.txt students/
 

# 4. Удалите папку mentors.
# способ из прошлого урока
rm -r mentors/

# безопасный способ удаления только пустого каталога
rmdir mentors/


# 5. Переименуйте папку students в students_and_mentors.
mv students students_and_mentors
 

# 6. Удалите папку students_mentors вместе с содержимым.
# правильное удаление (с ключом –r)
rm -r students_mentors
