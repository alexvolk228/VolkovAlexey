## Курсовой проект по дисциплине "Проектирование информационных систем"

## Волков Алексей, ИДБ-17-06

### 1. Определение требований к модели [✋](https://github.com/stankin/design-part-2/wiki/LR-1)

**Тема ВКР:** Разработка и создание CRM-системы для кастомизированного производства велосипедных компонентов. 

**Объект исследований:** бизнес-процессы управления взаимоотношениями с клиентами.

**Предмет исследований:** система для управления взаимоотношениями с клиентами.

**Процессы верхнего уровня:** [✋](https://github.com/stankin/design-part-2/wiki/sem1)
* **А1** Управление продажами. 
* **А2** Производсво. 
* **А3** Складирование. 
* **А4** Доставка компонентов потребителю.  

**Точка зрения:** Коммерческий директор. 

**Цель моделирования:** определение автоматизируемых функций. 

### 2. Функциональное моделирование процессов (IDEF0) [✋](https://github.com/stankin/design-part-2/wiki/LR-1)

* A-0 (контекстная диаграмма)

![A-0](https://github.com/alexvolk228/VolkovAlexey.github.io/blob/master/Course%20project/Screenshots/A0.png?raw=true)

* A0 (диаграмма верхнего уровня)

![A0](https://github.com/alexvolk228/VolkovAlexey.github.io/blob/master/Course%20project/Screenshots/A1-A4.png?raw=true)

* A1 (декомпозиция процесса/процессов внутренней среды)

![A1](https://github.com/alexvolk228/VolkovAlexey.github.io/blob/master/Course%20project/Screenshots/A11-A14.png?raw=true)


* A2 (декомпозиция процесса/процессов внутренней среды)

![A2](https://github.com/alexvolk228/VolkovAlexey.github.io/blob/master/Course%20project/Screenshots/A21-A23.png?raw=true)


* A3 (декомпозиция процесса/процессов внутренней среды)

![A3](https://github.com/alexvolk228/VolkovAlexey.github.io/blob/master/Course%20project/Screenshots/A31-A33.png?raw=true)


* A4 (декомпозиция процесса/процессов внутренней среды)

![A4](https://github.com/alexvolk228/VolkovAlexey.github.io/blob/master/Course%20project/Screenshots/A41-A43.png?raw=true)

### 3. Функциональное моделирование программных и информационных средств (DFD) [✋](https://github.com/stankin/design-part-2/wiki/LR-2)

**Конфигурация технических средств:** сервер (Apache/2.4.46), осуществляющий хранение и обработку данных. ПК для работы с веб-приложением. Операционная система Windows, Linux или Mac OS.  

**Конфигурация программных средств:** трехуровневая: клиент - веб-приложение, веб-сервер, сервер БД. 

**Допустимые виды хранилищ и их размещение:** БД phpMyAdmin. 

* Автоматизация процесса А12

![A12](https://github.com/alexvolk228/VolkovAlexey.github.io/blob/master/Course%20project/Screenshots/A12-dfd.png?raw=true)

* Автоматизация процесса А13

![A13](https://github.com/alexvolk228/VolkovAlexey.github.io/blob/master/Course%20project/Screenshots/A13-dfd.png?raw=true)

* Автоматизация процесса А14

![A14](https://github.com/alexvolk228/VolkovAlexey.github.io/blob/master/Course%20project/Screenshots/A14-dfd.png?raw=true)

* Автоматизация процесса А21

![A21](https://github.com/alexvolk228/VolkovAlexey.github.io/blob/master/Course%20project/Screenshots/A21-dfd.png?raw=true)

* Автоматизация процесса А32

![A32](https://github.com/alexvolk228/VolkovAlexey.github.io/blob/master/Course%20project/Screenshots/A32-dfd.png?raw=true)

* Автоматизация процесса А33

![A33](https://github.com/alexvolk228/VolkovAlexey.github.io/blob/master/Course%20project/Screenshots/A33-dfd.png?raw=true)

* Автоматизация процесса А43

![A43](https://github.com/alexvolk228/VolkovAlexey.github.io/blob/master/Course%20project/Screenshots/A43-dfd.png?raw=true)

### 4. Описание выбранного процесса [✋](https://github.com/stankin/design-part-2/wiki/LR-3) в формате прецедента (Use Case) [✋](https://github.com/stankin/design-part-2/wiki/LR-4)

[Диаграмма UML Use Case](https://github.com/alexvolk228/VolkovAlexey.github.io/blob/master/Course%20project/use_case.txt)
![UML](https://github.com/alexvolk228/VolkovAlexey.github.io/blob/master/Course%20project/Screenshots/uml.png?raw=true)

**4.1 Идентификатор прецедента:**  A13

**4.2 Название прецедента:** Обработка заказа

**4.3 Контекст:** A1 Управление продажами

**4.4 Участники (actors) и цели (goals):**

| Участник  | Категория  | Цель (goal) |
|---|---|---|
| Клиент | Внешний  | Оформление заказа |
| Администратор | Основной  | Управление БД и сотрудниками |
| Менеджер | Основной  | Управление заказами |
| Технолог | Основной  | Проверка деталей на совместимость |
| Курьер | Основной  | Доставка деталей |
| CRM-система | Инструмент| Предоставление средств для работы с клиентами |
| База данных | Инструмент| Хранение данных о заказах, клиентах, сотрудниках и товарах |

**4.5 Предусловия (pre-conditions):**

* Установлены программные средства для работы с CRM-системой
* Создана БД 
* Добавлены сотрудники
* Определён порядок обработки заказов

**4.6 Постусловия (post-conditions):**

* Полностью рабочая CRM-система, обеспечивающая обработку заказов

**4.7 Основной поток выполнения (main flow)**:

| Участник  | Действие (activity)  | Ожидаемый результат |
|---|---|---|
| Администратор | Установка программных средств | Установленное ПО |
| Администратор | Создание БД | Структура таблиц |
| Администратор | Добавление сотрудников | БД сотрудников |
| Менеджер | Формирование порядка обработки заказов | Порядок обработки заказов |

**4.8 Исключения (exceptions):**

| Условие (риск) | Последствия | Реакция |
|---|---|---|
| Ошибка в установке ПО | Невожможность работы CRM-системы | Переустановка ПО |

**4.9 Альтернативы (alternates):**

| Участник  | Действие (activity)  | Ожидаемый результат |
|---|---|---|
| Поставщик ПО | Предоставление подробной инструкции по установке ПО | Отсутствие ошибок при установке ПО |

**4.10 Временные параметры:**

* **Триггер (событие, стартующее прецедент):** поступление заказа. 

* **Номинальная частота повторения прецедента:** 50 раз в сутки

* **Продолжительность прецедента:** 5 сек

### 5. Описание структуры объекта [✋](https://github.com/stankin/design-part-2/wiki/LR-3) в формате ERD (Class) [✋](https://github.com/stankin/design-part-2/wiki/LR-5)

* **Описываемый объект:** БД заказы

* **Диаграмма UML Class:**
![p5](http://www.plantuml.com/plantuml/proxy?idx=0&src=https://raw.githubusercontent.com/<user/user.github.io/master/<path><file>)

### 6. Описание алгоритма [✋](https://github.com/stankin/design-part-2/wiki/LR-3) в формате UML (Sequence) [✋](https://github.com/stankin/design-part-2/wiki/LR-6)

* **Описываемые процессы и потоки данных:** A13 Обработка заказа

* **Диаграмма UML Sequence:**
![p6](http://www.plantuml.com/plantuml/proxy?idx=0&src=https://raw.githubusercontent.com/<user/user.github.io/master/<path><file>)

### 7. Описание состава [✋](https://github.com/stankin/design-part-2/wiki/LR-3) в формате UML (Component) [✋](https://github.com/stankin/design-part-2/wiki/LR-7)

* **Описываемый объект:** структура программных средств CRM-системы

* **Диаграмма UML Component:**
![p7](http://www.plantuml.com/plantuml/proxy?idx=0&src=https://raw.githubusercontent.com/<user/user.github.io/master/<path><file>)

### 8. Демонстрация реализации (личная страница)

Личная страница на [Github]()

### 9. Подготовка к интерпретации построенных моделей

**9.1 Используемые паттерны проектирования и разработки [✋](https://github.com/stankin/design-part-2/wiki/sem2):**

* **Процессная модель для сравнения:**

* **Используемые в разработке паттерны и фреймворки:**

**9.2 Используемые паттерны выявления проблем [✋](https://github.com/stankin/design-part-2/wiki/sem3):**
* Муда: <муда>
* Мура: <мура>
* Мури: <мури>

**9.3 Возможные антипаттерны [✋](https://github.com/stankin/design-part-2/wiki/sem4):**

| Категория  | Антипаттерн (риск) | Действие по избежанию |
|---|---|---|
| Разработка | <антипаттерн> | <действие> |
| Архитектура | <антипаттерн> | <действие> |
| Организация | <антипаттерн> | <действие> |
| Среда | <антипаттерн> | <действие> |

### 10. Интерпретация построенных моделей

**10.1 Определение числовых показателей для поставленной цели моделирования:**

**10.2 Определение числовых показателей для цели потенциального проекта автоматизации: [✋](https://github.com/stankin/design-1/wiki/interpret_process)**

**10.3 Расчет потенциального эффекта от автоматизации:**

**10.4 Определение числовых показателей и расчет трудозатрат на разработку программных средств:**

**ВЫВОДЫ**

