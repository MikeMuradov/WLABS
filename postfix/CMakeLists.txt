file(GLOB hdrs "*.h*") #Добавляем в переменную hdrs все файлы с расширением .h
file(GLOB srcs "*.cpp")#Добавляем в переменную srcs все файлы с расширением .h
add_executable(${postfix} ${srcs} ${hdrs}) #Создаем проект с именем из переменной ${postfix}, в него добавляются файлы из переменных ${srcs} и ${hdrs}
target_link_libraries(${postfix} ${postfixlib}) #Подключаем к проекту с именем ${vector} библиотеку с именем ${vectorlib}