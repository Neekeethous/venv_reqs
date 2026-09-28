## Виртуальное окружение
### Создание venv и установка библиотек
1. Создадим виртуальное окружение:
    ```cmd
    python -m venv my_venv
    ```

2. Активируем виртуальное окружение:
    ```cmd
    my_venv\Scripts\activate.bat
    ```
    При успешной активации слева должно появиться название вашей venv:
    
    <img width="761" height="281" alt="image" src="https://github.com/user-attachments/assets/5d4e9a20-21fa-4f45-b2aa-262f966b52d0" />

3. Проверим, какой интерпретатор сейчас используется:
    ```cmd
    where python
    ```
    Первая строка указывает на текущий интерпретатор:
    
    <img width="654" height="100" alt="image" src="https://github.com/user-attachments/assets/20990344-230d-4647-85c6-00ee7a0b9796" />
    
4. Установим менеджер пакетов uv:
     ```cmd
   pip install uv
    ```
5. В дальнейшем все зависимости будем устанавливать при помощи uv:
    ```cmd
   uv pip install numpy pandas 
    ```

    Если есть файл с необходимыми зависимостями, то устанавливаем следующим образом:
    ```cmd
     uv pip install -r requirements.txt
    ```
