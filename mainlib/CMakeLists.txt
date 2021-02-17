file(GLOB hdrs "*.h*") #Добавляем в переменную hdrs все файлы с расширением .h
file(GLOB srcs "*.cpp")#Добавляем в переменную srcs все файлы с расширением .h
add_executable(${lib} ${srcs} ${hdrs}) #Создаем проект с именем из переменной ${temp}, в него добавляются файлы из переменных ${srcs} и ${hdrs}
target_link_libraries(${lib} ${mainlib}) #Подключаем к проекту с именем ${mainlib} библиотеку с именем ${lib}