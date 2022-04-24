##  задание 1
1. _Скачайте библиотеку boost с помощью утилиты wget.[Адрес для скачивания](https://sourceforge.net/projects/boost/files/boost/1.69.0/boost_1_69_0.tar.gz)
```
$ wget https://sourceforge.net/projects/boost/files/boost/1.69.0/boost_1_69_0.tar.gz
```
2. _Разархивируйте скаченный файл в директорию ~/boost_1_69_0_
```
$ tar -xvf boost_1_69_0.tar.gz
```
3. _Подсчитайте количество файлов в директории ~/boost_1_69_0 не включая вложенные директории._
```
18
```
4. _Подсчитайте количество файлов в директории ~/boost_1_69_0 включая вложенные директории._
```
62134
```
5. _Подсчитайте количество заголовочных файлов, файлов с расширением .cpp, сколько остальных файлов (не заголовочных и не .cpp)._

Заголовочные
```
$ find boost_1_69_0 -type f -name '*.hpp' -o -name '*.h' | wc -l
15208
```
cpp файлы
```
$ find boost_1_69_0 -type f -name '*.cpp' | wc -l
13789
```
остальные файлы 
```
$ find boost_1_69_0 -type f -name '*.cpp' -o -name '*.h' -o -name '*.hpp' | wc -l
28997
```
6. _Найдите полный пусть до файла any.hpp внутри библиотеки boost._
```
$  find `pwd`/boost_1_69_0/boost -name 'any.hpp'
>>/home/alexandra/boost_1_69_0/boost/hana/any.hpp
>>/home/alexandra/boost_1_69_0/boost/hana/fwd/any.hpp
>>/home/alexandra/boost_1_69_0/boost/proto/detail/any.hpp
>>/home/alexandra/boost_1_69_0/boost/any.hpp
>>/home/alexandra/boost_1_69_0/boost/type_erasure/any.hpp
>>/home/alexandra/boost_1_69_0/boost/fusion/include/any.hpp
>>/home/alexandra/boost_1_69_0/boost/fusion/algorithm/query/any.hpp
>>/home/alexandra/boost_1_69_0/boost/fusion/algorithm/query/detail/any.hpp
>>/home/alexandra/boost_1_69_0/boost/spirit/home/support/algorithm/any.hpp
>>/home/alexandra/boost_1_69_0/boost/xpressive/detail/utility/any.hpp
```
7. _Выведите в консоль все файлы, где упоминается последовательность boost::asio._
```



