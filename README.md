# RESTful Photo Gallery
Task from lozenko mentoring.

Технологии которые обязательны к использованию
1.	Maven
2.	Maven Jacoco Plugin с 80% покрытием тестов
3.	Maven Checkstyle Plugin с выключенным package-info компонентом
4.	Spring Boot + Embedded Tomcat
5.	Spring Thymeleaf
6.	Twitter Bootstrap
Не использование данного стека автоматически исключает вас с ревью.
Ваша задача написать простенький сервис который будет предлагать пользователю создать фото галлерею на основании папки где эти фотографии лежат (внутренние папки тоже сканируются).
Вот прототип который нужно повторить.

 

Ваш сервис будет находится на localhost:8080/photo , где /photo - это маппинг стартовой страницы как и дальнейшая работа с ним после.
После того как вы нажмете на кнопку Create Galleryвыполниться обработка папки на предмет фотографий которые имееют расширение png (ТОЛЬКО PNG!!).
После этого страница будет иметь такой вид:

 

Как видите готовый вид имеет ряд закономерностей:
1.	Все фотографии имеет одинаковый размер (по дефолту 200x200)
2.	Фотографию имеет не больше 4 фотографий в ряд
3.	В конце, как на картинке, выводиться результат сколько фотографий получилось загрузить.
Дополнительные RESTlike опции:
1.	/photo/original - показывает реальные размеры фотографий
2.	/photo/row/5 - показывает все фотографии с рядом где можно уже не 4 а 5 фотографий (может быть любое число)
3.	/photo/wh/200x250 - фотографии выводятся с размером 200 на 250. Можно подставить любые по маске ZZZxYYY.
4.	/photo/blackbackground - фотографии отображаются на черном фоне
Вышестоящие опции вместе соединять не нужно, они работают по отдельности.
Дается неделя (а это много) даже для тех кто вообще не понимает о чем речь.
Дедлайн: пятница 22-00.
Мой совет всем - прочитайте по каждой технологии немножко отдельно с маленьким хелловордом. Запустите сначала просто Spring boot c маппингом /hello который будет просто “hello world” возвращать, потом вместо “hello world” верни простой thymeleaf теймплейт. И по шажочку понемножку наращиваете мясом программу.
