1. Создание репозитория
Создал новый репозиторий на GitHub/GitLab.

Клонировал репозиторий на локальный компьютер:


git clone <ссылка_на_репозиторий>
2. Настройка CMake
Создал структуру проекта:

Папка src с файлами main.cpp, utils.cpp и utils.h.

Написал код:

В utils.cpp добавил функции (сложение, вычитание, умножение).

В main.cpp использовал эти функции.

Создал CMakeLists.txt для сборки проекта
Собрал проект:

Создал папку build.

Запустил CMake и сборку:


cd build
cmake ..
cmake --build .
3. Работа с Git
Инициализировал Git-репозиторий (если не был инициализирован автоматически):
git init
Добавил файлы и сделал первый коммит:

git add .
git commit -m "Initial commit: CMake project setup"
Создал новую ветку featureutils:


git checkout -b featureutils
Добавил функцию умножения в utils.cpp и обновил main.cpp.

Закоммитил изменения:

git add .
git commit -m "feat: Add multiplication function to utils"
Вернулся в основную ветку (main/master) и внес изменения в main.cpp.

Слил ветку featureutils в основную:

git merge featureutils
Разрешил конфликты (если они возникли).

4. Отправка изменений
Отправил все ветки и коммиты в удаленный репозиторий:

git push --all origin
Добавил описание проекта в README.md:

Указал структуру проекта, инструкцию по сборке и историю коммитов.

5. Результат
Создан репозиторий с C++ проектом, который собирается с помощью CMake.
Продемонстрирована работа с Git: создание веток, слияние, разрешение конфликтов.
Проект успешно собран и запущен.
