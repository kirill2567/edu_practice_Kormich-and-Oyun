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



















