# pyinstaller_extractor

Данная инстукция предназначена для реверса скомпилированных в exe файлов python.

1. Установите библеотеку uncompyle6:
pip install uncompyle6

2. Скачайте с этого репозитория pyinstxtractor18.py или другую версию с https://sourceforge.net/projects/pyinstallerextractor/

3. Поместите этот файл в директорию с exe файлом

4. Наберите команду python pyinstxtractor18.py your_filename.py

5. В появившейся директории your_filename.exe_extracted находим файл your_filename и добавляем ему формат .pyc

6. Находим и открываем архив base_library.zip. В нем открываем в hex-редакторе (HxD) файл abc.pyc. Копируем 
![image](https://user-images.githubusercontent.com/65065736/126106085-f5405e97-65a0-40f3-8f32-95a2bc884a47.png)
