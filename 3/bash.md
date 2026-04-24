# Bash lab 1

## 1.zero.sh 
## Скрипт с использованием переменных

~~~
#!/bin/bash
group="9CA-321"
first_name="Кирилл"
last_name="Кормич"
salary=770
usd_rate=90
usd_salary=$(echo "scale=2; $salary / $usd_rate" | bc)

echo "Я учусь в $group, зовут меня $first_name $last_name. В этом месяце мне пришла стипендия размером в $salary рублей, это $usd_salary в $."
~~~

<img width="840" height="62" alt="image" src="https://github.com/user-attachments/assets/d573873e-7f9e-4971-9f29-49f38c385771" />

## 2.start.sh 
## Приветствие через аргумент без if

~~~
#!/bin/bash
echo "Привет, Кирилл!"
~~~

<img width="326" height="44" alt="image" src="https://github.com/user-attachments/assets/11d162b6-c877-4923-9555-67b0cec84e3b" />

## 3.start_2.sh
## То же самое, но с if

~~~
#!/bin/bash
if [ -n "$1" ]; then
    echo "Привет, $1!"
else
    echo "Привет, Кирилл! Вы забыли указать имя в аргументах."
fi
~~~

<img width="408" height="56" alt="image" src="https://github.com/user-attachments/assets/bd04da56-a13b-4f9c-9c3f-831a0f117100" />
<img width="386" height="38" alt="image" src="https://github.com/user-attachments/assets/a4e99501-db48-46c3-8bcd-ec833bb0e623" />


## 4. file.sh
## Проверка существования файла

~~~
#!/bin/bash
if [ -e "$1" ]; then
    echo "Файл $1 существует."
else
    echo "Файл $1 отсутствует."
fi
~~~

<img width="410" height="54" alt="Выделение_025" src="https://github.com/user-attachments/assets/52938468-ff74-43b8-8039-14e1f0ebf5d1" />
<img width="350" height="40" alt="Выделение_024" src="https://github.com/user-attachments/assets/05aedf1d-2091-4b67-8bae-ba3f4d6d7c87" />


## 5. my_dir.sh
## Список файлов в директории.

~~~
#!/bin/bash
if [ -z "$1" ]; then
    echo "Ошибка: укажите путь к директории. Пример: ./my_dir.sh /etc"
else
    echo "Содержимое директории $1:"
    ls "$1"
fi
~~~

<img width="562" height="60" alt="Выделение_027" src="https://github.com/user-attachments/assets/a8542db2-c470-4fa7-98b1-d3d436991054" />
<img width="386" height="60" alt="image" src="https://github.com/user-attachments/assets/60366e76-9990-4dee-bcf3-a0c506ababe2" />


## 6. dir_m.sh
## Создание директории с проверкой.

~~~
#!/bin/bash
if [ -z "$1" ]; then
    echo "Ошибка: введите название новой папки. Пример: ./dir_m.sh МояПапка"
else
    if [ -d "$1" ]; then
        echo "Директория '$1' уже существует." 
    else
        mkdir "$1" 
        echo "Директория '$1' успешно создана."
    fi
fi
~~~


<img width="408" height="34" alt="Выделение_028" src="https://github.com/user-attachments/assets/a46ddb48-9a46-40bf-a6cf-f1e61b018179" />
<img width="364" height="38" alt="image" src="https://github.com/user-attachments/assets/4af506e1-948f-4b35-a02b-635b0c2a1a04" />



## 7. user_light.sh
## Скрипт который ищет вашего пользователя 

~~~
#!/bin/bash
# Ищем текущего пользователя в файле passwd
if grep -q "$USER" /etc/passwd; then
    echo "Поздравляю! Пользователь $USER найден в системе."
fi
~~~

<img width="428" height="67" alt="image" src="https://github.com/user-attachments/assets/71be6135-2bd5-49a5-9d7d-95f3557c758c" />


## 8. user_f.sh
## Скрипт который принимает имя пользоваетеля

~~~
#!/bin/bash
username=$1
if grep -q "$username" /etc/passwd; then
    echo "Пользователь $username найден."
else
    echo "Пользователь $username не найден."
fi
~~~

<img width="371" height="74" alt="image" src="https://github.com/user-attachments/assets/2bdd5740-76bd-4982-be03-364f26e72928" />


## 9. user_f2.sh
## Скрипт который создает файл в случае отсутсвия пользователя 

~~~
#!/bin/bash
username=$1
if grep -q "$username" /etc/passwd; then
    echo "Пользователь $username нашелся."
else
    echo "Пользователь не найден."
    touch "don_t_be_sad_user_${username}_will_be_there_soon.txt"
fi
~~~

<img width="476" height="92" alt="image" src="https://github.com/user-attachments/assets/204235e9-b4f8-4cda-afab-a8a319843056" />


## 10. finder_liight.sh
## Скрипт который принимает имя файла в качестве аргумента 

~~~
#!/bin/bash
file=$1
if [ -L "$file" ]; then
    echo "$file — это символическая ссылка."
elif [ -d "$file" ]; then
    echo "$file — это директория."
elif [ -f "$file" ]; then
    echo "$file — это обычный файл."
else
    echo "Объект не найден."
fi
~~~

<img width="331" height="175" alt="image" src="https://github.com/user-attachments/assets/81a88887-0ad9-4685-b4e6-421efde7e2e5" />


## 11. math.sh
## Скрипт который принимает два числа в качестве аргумента 

~~~
#!/bin/bash
if [ "$#" -ne 2 ]; then
  echo "Ошибка: нужно ввести два числа."
  exit 1
fi

NUM1=$1
NUM2=$2

SUM=$((NUM1 + NUM2))
DIFF=$((NUM1 - NUM2))
PROD=$((NUM1 * NUM2))

echo "Сумма: $SUM"
echo "Разность: $DIFF"
echo "Произведение: $PROD"
~~~

<img width="219" height="79" alt="image" src="https://github.com/user-attachments/assets/11d732a0-a43a-4bc8-bf85-cdd54e271543" />


## 12. sort.sh 
## Скрипт который выводит все аргументы 

~~~
#!/bin/bash

# Цикл проходит по всем аргументам, переданным скрипту
for arg in "$@"
do
  echo "$arg"
done
~~~

<img width="334" height="92" alt="image" src="https://github.com/user-attachments/assets/830ec377-6695-45c2-8b72-df47cf1df723" />

## 13. io.sh 
## Скрипт который принимает один аргумент 

~~~
#!/bin/bash
if [ "$1" == "start" ]; then
  echo "Starting..."
elif [ "$1" == "stop" ]; then
  echo "Stopping..."
else
  echo "Используйте start или stop"
fi
~~~

<img width="219" height="172" alt="image" src="https://github.com/user-attachments/assets/a41d72a4-8e4c-4b7b-a6bb-55ecd2f2ed3e" />


## 14. user_use.sh 
## Скрипт который принимает один аргумент 

~~~
#!/bin/bash

echo "Использование диска в /home (от большего к меньшему):"

# du -sh считает размер, 2>/dev/null скрывает ошибки доступа
# sort -rh сортирует по размеру в обратном порядке
du -sh /home/* 2>/dev/null | sort -rh
~~~

<img width="1055" height="117" alt="image" src="https://github.com/user-attachments/assets/4a78dd1f-3103-4c09-b933-784ae5b459ce" />


## 15. sort_du.sh 
## Скрипт который сортирует

~~~
#!/bin/bash
dir=${1:-.}
find "$dir" -maxdepth 1 -type f -exec stat -c "%y %n" {} + | sort | head -n 3
~~~

<img width="435" height="77" alt="image" src="https://github.com/user-attachments/assets/b6dc1385-d515-4b42-ae50-8790b8d0ebd5" />


## 16. dir_info.sh 
## Скрипт который принимает путь к директории в качестве аргумента 

~~~
#!/bin/bash
# [span_6](start_span)Определяем директорию[span_6](end_span)
target_dir=${1:-.}

# du -s (итог), -k (в килобайтах)
# [span_7](start_span)awk формирует нужный формат вывода[span_7](end_span)
du -sk "$target_dir" | awk '{print "Общий размер: " $1 " КВ"}'
~~~

<img width="175" height="198" alt="image" src="https://github.com/user-attachments/assets/0f79264c-ca7a-412f-a1df-e62717d88f73" />
*GitBash не выводит числа*


## 17. bash_history.sh 
## Скрипт который анализирует историю команд

~~~
echo '#!/bin/bash
history -a

cat ~/.bash_history | awk "{print \$1}" | sort | uniq -c | sort -nr | head -n 5' > bash_history.sh
~~~
<img width="210" height="153" alt="image" src="https://github.com/user-attachments/assets/8832f09a-989d-4851-acc5-50d7231d2403" />
