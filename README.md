 Проверьте конфигурацию, используемую для определения правил для типов элементов (BUNDLE, PACKAGE, CLASS, SOURCEFILE или METHOD) со списком ограничений. Каждый лимит применяется к определенному счетчику (INSTRUCTION, LINE, BRANCH, COMPLEXITY, METHOD, CLASS) и определяет минимум или максимум для соответствующего значения (TOTALCOUNT, COVEREDCOUNT, MISSEDCOUNT, COVEREDRATIO, MISSEDRATIO). Если предел относится к соотношению, он должен находиться в диапазоне от 0,0 до 1,0, где количество десятичных знаков также будет определять точность сообщений об ошибках. При желании предельное отношение может быть объявлено в виде процента, где 0,80 и 80% представляют одно и то же значение.
 
 Если не указано иное, предполагаются следующие значения по умолчанию:
 
 элемент правила: BUNDLE
 счетчик лимита: INSTRUCTION
 предельное значение: COVEREDRATIO
 
 
JaCoCo также вычисляет охват филиальную для всех ifи switchотчетности. Эта метрика подсчитывает общее количество таких ветвей в методе и определяет количество выполненных или пропущенных ветвей. Покрытие веток всегда доступно, даже при отсутствии отладочной информации в файлах классов. Обратите внимание, что обработка исключений не рассматривается как ветки в контексте этого определения счетчика.

Если файлы классов были скомпилированы с отладочной информацией, точки принятия решения могут быть сопоставлены с исходными строками и выделены соответствующим образом:

* Нет покрытия: нет ответвлений в линии (красный ромб)
* Частичное покрытие: выполнена только часть ветвей в линии (желтый ромб)
* Полное покрытие: все ответвления в линии выполнены (зеленый ромб)
 
 Я использовала счетчик лимита: INSTRUCTION со 100%, как требовалось в дз