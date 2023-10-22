# job4j_di
Внедрение зависимостей

Идея DI.
1. Есть хранилище объектов. В нем мы будем регистрировать классы, объекты которых хотим иметь в проекте.
   В нашем примере мы зарегистрируем там Tracker, StartUI, ConsoleInput.
2. Хранилище в рамках DI называется Context, то есть объекты относящиеся к предметной области нашего проекта.
3. После регистрации классов Context начинает инициализацию объектов. Он строит дерево зависимостей. Сначала он создает объекты без зависимостей.
   А потом создаем объекты с зависимостями.
4. После инициализации программист может получить нужный объект из Context.