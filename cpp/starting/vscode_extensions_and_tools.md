### Для работы комфортного написания кода потребуется установить пару расширений.  
- C/C++ от Micrisoft
- C/C++ Extension Pack от Micrisoft
- Better C++ Syntax от Jeff Hykin
- Code Runner (опционально, удобно запускать программы напрямую)

### Так же нужно для сборки поставить компилятор

#### 🪟Windows:
- Вариает 1: Установи MinGW-w64

Шаги:
1. Скачайте онлайн-установщик MinGW-w64:
🔗 https://sourceforge.net/projects/mingw-w64/files/
2. Запустите mingw-w64-install.exe.
3. Настройки при установке:
Version : любая (например, 8.1.0)
Architecture : x86_64
Threads : win32
Exception : seh
Путь установки:


1
C:\mingw64
Добавьте путь к bin в системную переменную среды PATH:


1
C:\mingw64\bin
Перезагрузите терминал и проверьте:
cmd

- Вариант 2: Используй MSVC (компилятор из состава Visual Studio)

#### 🍎macOS: 
- Установите Xcode Command Line Tools
```bash
xcode-select --install
```

#### Linux: