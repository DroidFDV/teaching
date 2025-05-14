### Для комфортного написания кода потребуется установить пару расширений 
- C/C++ от Micrisoft
- C/C++ Extension Pack от Micrisoft
- Better C++ Syntax от Jeff Hykin
- Code Runner (опционально, удобно запускать программы напрямую)

### Так же нужно для сборки поставить компилятор

#### 🪟Windows:
- Вариает 1: Установи MinGW-w64  
    **Шаги**:
    1. Скачай toolkit c MinGW-w64:
    🔗 [https://github.com/skeeto/w64devkit/releases] 
        Нужно будет найти w64devkit-x64-X.X.X.7z.exe, где X.X.X это просто версия
    1. Запусти w64devkit-x64-X.X.X.7z.exe.
    1. Путь установки: ```C:\w64devkit```  
    1. Добавьте путь к bin (```C:\w64devkit\bin``` в нашем случае) в системную переменную среды PATH:
        - Открой панель управления
        - В поиске найди ```Изменение системных переменных среды```
        - Перейди в ```Переменные среды...```
        - В списке ```Системные переменные``` найди переменную ```Path``` кликни по ней дважды
        - В появившемся окне кликни ```Создать``` и вставь путь к bin
    1. Перезагрузи пк  
    Путь установки можешь выбрать, какой тебе удобно, но тогда в ```Path``` нужно будет добавить полный путь к папке bin (```path\to\w64devkit\bin```)

- Вариант 2: Используй MSVC (компилятор из состава Visual Studio)
    Шаги:
    1. Скачай Build Tools:
    🔗 [https://visualstudio.microsoft.com/downloads/]
    1. При установке выберите:
    "Desktop development with C++"
    Компоненты: MSVC Toolset, Windows SDK
    1. Используйте Developer Command Prompt для работы с cl.exe.
    1. Проверьте:
```bash
cl
```

#### 🍎macOS: 
Для macOS рекомендуется использовать Clang, который поставляется с Xcode.  

**Шаги**:
1. Установите Xcode Command Line Tools:
```bash
xcode-select --install
```
1. Проверьте установку:
```bash
clang++ --version
```
Пример компиляции:
```bash
clang++ -std=c++XX main.cpp -o myprogram
./myprogram
```

#### 🐧Linux (на примере Ubuntu):
На большинстве дистрибутивов Linux компилятор GCC уже установлен, но если его нет — можно легко установить.

**Шаги**:
```bash
sudo apt update
sudo apt install build-essential
```
Проверка:
```bash 
g++ --version
```
Пример компиляции:
```bash
g++ -std=c++17 main.cpp -o myprogram
./myprogram
```
