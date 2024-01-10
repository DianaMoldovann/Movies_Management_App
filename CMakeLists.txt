cmake_minimum_required(VERSION 3.23)
project(LAB_13-14_OOP)

set(CMAKE_CXX_STANDARD 14)
set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTORCC ON)
set(CMAKE_AUTOUIC ON)
set(CMAKE_PREFIX_PATH "/Users/dianamoldovan/Qt/6.5.0/macos/lib/cmake")

find_package(Qt6 COMPONENTS
        Core
        Gui
        Widgets
        REQUIRED)

add_executable(LAB_13-14_OOP main.cpp
        Domain/Movie.h
        Domain/Movie.cpp
        Validator/Validator.h
        Validator/Validator.cpp
        Repository/AbstractRepository.h
        Repository/Repository.h
        Repository/Repository.cpp
        Repository/LabRepository.h
        Repository/LabRepository.cpp
        Movies_Wishlist/Wishlist.h
        Movies_Wishlist/Wishlist.cpp
        Service/Service.h
        Service/Service.cpp
        Exceptii/Exceptii.h
        Exceptii/Exceptii.cpp
        Teste/Teste.h
        Teste/Teste.cpp
        Interfata/GUI/GUI.h
        Interfata/GUI/GUI.cpp
        Interfata/UI/UI.h
        Interfata/UI/UI.cpp
        Interfata/Observer/Observer-Observable.h
        Interfata/Observer/WishlistGUI.cpp
        Interfata/Observer/WishlistGUI.h
        Interfata/Model/MyTableModel.h
        Interfata/Model/GUIModel.h
        Interfata/Model/GUIModel.cpp
        Undo/Undo.h
        Undo/Undo.cpp)
target_link_libraries(LAB_13-14_OOP
        Qt::Core
        Qt::Gui
        Qt::Widgets
        )

