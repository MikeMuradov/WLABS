file(GLOB hdrs "*.h*") #Добавляем в переменную hdrs все файлы с расширением .h
file(GLOB srcs "*.cpp")#Добавляем в переменную srcs все файлы с расширением .h
add_executable(${polinom} ${srcs} ${hdrs}) #Создаем проект с именем из переменной ${polinom}, в него добавляются файлы из переменных ${srcs} и ${hdrs}
target_link_libraries(${polinom} ${polinomlib}) #Подключаем к проекту с именем ${vector} библиотеку с именем ${vectorlib}