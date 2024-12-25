# Планировщик задач cron

## Разминка(ее в отчет включать не нужно)

### 1) Открытие файла crontab:

```bash
crontab -e
```
Эта комманда откроет файл crontab в текстовом редакторе

### 2) Добавление задачи в файл crontab

```bash
* * * * * echo "Текущая дата и время: $(date)" >> ~/cron_test.txt
```
Данная программа будет записывать текущую дату и время в файл cron_test.txt раз в минуту

### 3) Сохраните изменения
   
Для этого используйте комбинацию клавиш Ctrl + x

### 4) Проверка задачи:

```bash
crontab -l
```
Через некоторое время откройте файл cron_test.txt

```bash
cat ~/cron_test.txt
```
Должны вывестись записи с датой и время

## Задание лабораторной работы (вот только его и нужно включить в отчет!)

Настройте задачу с помощью cron, которая будет выполнять скрипт для резервного копирования каталога /home/user/documents в /home/user/backup каждый вечер в 20:00.

## Результат: Каждый день в 20:00 ваш каталог /home/user/documents будет копироваться в /home/user/backup.

## Дополнительные источники

1. [Документация по cron.](https://man7.org/linux/man-pages/man5/crontab.5.html)
2. [Как использовать cron.](https://www.digitalocean.com/community/tutorials/how-to-use-cron-to-automate-tasks-on-a-vps)
3. [Документация по cron, Ubuntu.](https://help.ubuntu.com/community/CronHowto)
