## Шаги по выполнению лабораторой работы

### 1) Создание файлф скрипта backup.sh

```bash
echo -e "#!/bin/bash\ncp -r /home/andrey/documents /home/andrey/backup" > ~/backup.sh
```

### 2) Изменить права доступа и сделать скрипт исполняемым

![image](https://github.com/user-attachments/assets/4eaef6ca-4816-4ee7-900d-61c6f54f7dbb)

### 3) Открыть файл crontab:

```bash
crontab -e
```

### 4)Добавим в последнюю строчку файла crontab ''' 2 0 * * * ~/backup.sh '''

![image](https://github.com/user-attachments/assets/bd2b3a37-efe9-4365-be9e-33e230ef44cf)

### 5)Сохраним все

### 6)Убедимся, что изменения сохранились, выполнив 
```bash
crontab -l
```

![image](https://github.com/user-attachments/assets/31f9ed30-a716-42e2-81da-13a7094bf196)

