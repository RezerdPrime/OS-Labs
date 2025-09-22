cmake_minimum_required(VERSION 3.10) # Минимальная требуемая версия CMake
project(Main CXX) # Замените YourProjectName названием вашего проекта
set(CMAKE_CXX_STANDARD 17) # Стандарт C++, который вы хотите использовать (например, 11, 14, 17, 20)
# Укажите исходные файлы
file(GLOB SOURCES "*.cpp") # Автоматически добавляет все .cpp файлы в проект, если они все находятся в корне
# Если ваши исходные файлы находятся в подпапке, укажите путь к ней, например:
# file(GLOB SOURCES "src/*.cpp")
add_executable(${PROJECT_NAME} ${SOURCES}) # Создает исполняемый файл