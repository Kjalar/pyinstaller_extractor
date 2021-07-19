# pyinstaller_extractor

Данная инстукция предназначена для реверса скомпилированных в exe файлов python.

1. Установите библеотеку uncompyle6:
pip install uncompyle6

2. Скачайте с этого репозитория pyinstxtractor18.py или другую версию с https://sourceforge.net/projects/pyinstallerextractor/. Также вы можете скачайть с этого репозитория HxD редактор

3. Поместите pyinstxtractor18.py в директорию с exe файлом

4. Наберите команду python pyinstxtractor18.py your_filename.py

5. В появившейся директории your_filename.exe_extracted находим файл your_filename и добавляем ему формат .pyc

6. Находим и открываем архив base_library.zip. В нем открываем в hex-редакторе (HxD) файл abc.pyc. Копируем первую строку (до "г").
![image](https://user-images.githubusercontent.com/65065736/126106085-f5405e97-65a0-40f3-8f32-95a2bc884a47.png)

7. Вставляем скопированную строку в файл your_filename.pyc из шага 5
![image](https://user-images.githubusercontent.com/65065736/126106591-8364afbf-ada8-462a-87c4-79ea67da22a0.png)

8. Набираем в консоли uncompyle6 your_filename.exe_extracted/your_filename.pyc > your_filename_reverse.py
