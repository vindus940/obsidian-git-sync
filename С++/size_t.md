Открываем [cplusplus.com - size_t](http://www.cplusplus.com/reference/cstddef/size_t/) и читаем

> size_t Unsigned integral type

беззнаковое целое. То есть, это не int, он знаковый.

> Alias of one of the fundamental unsigned integer types.

Псевдоним для одного из фундаментальных без знаковых типов. (то есть, скорее всего 4 или 8 байтового).

> It is a type able to represent the size of any object in bytes: size_t is the type returned by the sizeof operator and is widely used in the standard library to represent sizes and counts.

Предназначен для отображения **размера** любого объекта в байтах: это возвращает size_of и много функций стандартной библиотеки - всякие length и count.

Пример использования в цикле: 
        for (size_t i = 0; i < nums.size(); ++i)
        {
            std::cout << (i + 1) << " - " << nums[i] << '\n';
        }