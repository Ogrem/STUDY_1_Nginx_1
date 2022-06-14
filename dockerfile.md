# ***Указываем образ источника из которого мы создаем свой образ.***
FROM nginx:1.22.0
# ***Копируем все файлы из корневой папки контейнера в папку где локализуем проэкт первого урока. _Пока там пусто_.***
COPY . /nginx
# ***Указываем папку внутри контейнера, для того чтобы локализовать проэкт.***
WORKDIR /nginx