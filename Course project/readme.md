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

![A4](https://github.com/alexvolk228/VolkovAlexey.github.io/blob/master/Course%20project/Screenshots/A41–A43.png?raw=true)

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

![A32](https://github.com/alexvolk228/VolkovAlexey.github.io/blob/master/Course%20project/Screenshots/A32–dfd.png?raw=true)

* Автоматизация процесса А33

![A33](https://github.com/alexvolk228/VolkovAlexey.github.io/blob/master/Course%20project/Screenshots/A33-dfd.png?raw=true)

* Автоматизация процесса А43

![A43](https://github.com/alexvolk228/VolkovAlexey.github.io/blob/master/Course%20project/Screenshots/A43–dfd.png?raw=true)

### 4. Описание выбранного процесса [✋](https://github.com/stankin/design-part-2/wiki/LR-3) в формате прецедента (Use Case) [✋](https://github.com/stankin/design-part-2/wiki/LR-4)

[Диаграмма UML Use Case](https://github.com/alexvolk228/VolkovAlexey.github.io/blob/master/Course%20project/use_case.txt)
![UML](http://www.plantuml.com/plantuml/png/ZPJDJXin4CVlVWehTn0E7vHBXTHpBts1A0hRDX8bKhBSar2fbJXmR5LL_P3w04kIBUw6NLvXvetw7tkpBawK8hG6U-Ot7_ynFXsbtM5w-UvSdIUlKvqEzB3_vcsgp_h3f9Vs1nTATNlfOAXRz8aoAl3TyGUoLBGQmrVAgSIteD-KypWOlb15z_Z18PYS9-0j_Ud0q_8OHC5JglubFbE98_XBG9vs06SqbwG0oyRlnQkN7KIpF15lSMefTJbAUjrHecKnkZj2k9yeOERIVtGrMierGjLzY37YsfxxZW8g9BZ7EkMn5d-UWbc2cQzbs_VKB-a5ZFGcURDLna8ClWM-ZjW3ptxZzpMzt5HfdF7GKpzWl0M7qZHF7W5IHmGTrQdebiSD2FVjaXpNaeYCRiWPPXapcaevUt2TMvpDy7iXuv6_eeZFDXTVrWA8qXOOj98cD59MLF0LDhbSZuszdOI1tm5OIUzAdaFJBD0HQVR-Cxq7CV0DBRnMLIIVtIwVCU5AYNgLY0BVMHWqklT6hvSqlEGR7RBmjHEe06AtQ61MjvSg1BZ2c3RVUIqn7uVpTJ_v7rRlx3pterH-eBkxVdyIxSsUKl73qS16kRLnRaVx_MX_e5JyrZIn3fLR6z-ZQ7yCTllZ4ifgAxN-m0IpKQV9nHcUpBy0)

**4.1 Идентификатор прецедента:**  A1

**4.2 Название прецедента:** Управление продажами

**4.3 Контекст:** A0 Управление взаимоотношениями с клиентами

**4.4 Участники (actors) и цели (goals):**

| Участник  | Категория  | Цель (goal) |
|---|---|---|
| Заказчик  | Внешний | Формирование заказа |
| Коммерческий директор | Внутренний | Создание регламента |
| Коммерческий директор | Внутренний | Формирование порядка обработки заказа |
| Менеджер | Внутренний | Обработка заказов |
| Менеджер | Внутренний | Передача заказов на производство |
| Интернет-магазин | Инструмент| Получение заказов от клиентов |
| CRM-система | Инструмент| Предоставление средств для работы с клиентами |

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

* **Описываемый объект:** БД CRM

* **Диаграмма UML Class:**
![Class](https://github.com/alexvolk228/VolkovAlexey.github.io/blob/master/Course%20project/Screenshots/uml-class.png?raw=true)

### 6. Описание алгоритма [✋](https://github.com/stankin/design-part-2/wiki/LR-3) в формате UML (Sequence) [✋](https://github.com/stankin/design-part-2/wiki/LR-6)

* **Описываемые процессы и потоки данных:** A14 Передача заказа на производство

* [**Диаграмма UML Sequence:**](https://github.com/alexvolk228/VolkovAlexey.github.io/blob/master/Course%20project/sequence.txt)
![Sequence](http://www.plantuml.com/plantuml/png/dPBFIiD04CRl-nHBxtq13rBmxCKtsBOB1arIacszcjO_We9uqeCeuWjinRJ1jkahpBoHtsonj2Y27cPWij_-vfkTj79dCjUFZrL-52KzavbOnscITWwpDBRQPNshbEcuDDFqI2Kj4EyqeP9FjSbrFxUPmYqNTQAUIPnkx1tiDxcWYWiUGZidtn3XYMrlw-X56FGcEIX06gYkSQPjSelpE_8q9Q_HpgFjWg_vF0ZbN2abhNLpLyXwHzC3n7Cn6AAYKWS7deSyua8uWD772YeJHGFZRF25490O4D8zD4jOgxdGGE5czJzsc4YIqCMrq9ze34QDmMTh6jA2pwX6qpce5wYhDMOrhwHDaw_ekwIIhmAi_Aj7mMmythDiGJOB_IMqePZoY6Py8n29hsUITm-3u6DDOqWzJTPDVxhvpHpV_cgkQxTdtwZ5D-gjzRLiqiKF_0a0)

### 7. Описание состава [✋](https://github.com/stankin/design-part-2/wiki/LR-3) в формате UML (Component) [✋](https://github.com/stankin/design-part-2/wiki/LR-7)

* **Описываемый объект:** структура программных средств CRM-системы

* [**Диаграмма UML Component:**](https://github.com/alexvolk228/VolkovAlexey.github.io/blob/master/Course%20project/component.txt)

![Component](http://www.plantuml.com/plantuml/png/SoWkIImgAStDuIhEpimhI2nAp5L8piyjoCzBpIjHgEPoIapEJY_AByrBSSxFoIzI2C_8B4dbSYmgoY-723Zb05LmEUKNfQGM8OlKSY6Pc9bNabgKbfYSIfc928T5NvXuOSE5xHSsA5pO0cJilR3tOlV5rbY5n6855oTaTSv1lhh95tPSRBpOT67hXJqNDe3Lk3cZcBNmmjQB3HSsWKYmT71gKLbg4HUNXgQ2ae-Zdn98p0VCymW92G1pFRYut9mLT86q1v24Qe1GGBuFbm-G1Bh48JKl1HYu0000)

### 8. Демонстрация реализации (личная страница)

Личная страница на [Github](https://alexvolk228.github.io/#!/topics)

### 9. Подготовка к интерпретации построенных моделей

**9.1 Используемые паттерны проектирования и разработки [✋](https://github.com/stankin/design-part-2/wiki/sem2):**

* **Процессная модель для сравнения:**

Задача: создание системы для наиболее эффективного взаимодействия с клиентами.

**Решение задачи при помощи методологии PDCA:**

1. **Plan (Планирование):**

 + Выявленные проблемы :

   + неэффективная работа с заказами;
   + отсутствие истории взаимодействия с клиентами;
   + аналитика продаж и её визуализация занимает много времени;

 + Цели: 

   + сокращение временных затрат на обработку заказов;
   + ведение истории взаимодействия с клиентами;
   + автоматическое создание отчётов. 

 + Требования: конечная система должна быть проста в использовании, как для администратора, так и для остальных сотрудников.

 + Ожидаемый результат: увеличение количества продаж.

 + Ресурсы, необходимые для достижения ожидаемого результата: 

   + CRM-система;
   + БД;
   + Веб-сервер;
   + Сервер. 

 + Процессы (запланированные действия):

   + Проектирование;
   + Верстка;
   + Настройка и подключение БД;
   + Fullstack - разработка модуля;
   + Ручное тестирование. 

2. Do (Выполнение) : Выполнение поставленных задач сотрудниками, обладающими правами на использование системы. 

3. Check (Проверка) : Оценка эффективности на основе результатов внедрения и использования системы. 

4. Act (Улучшение) : При успешной работе системы (при сокращении временных затрат на обработку заказов), он внедряется в информационную систему предприятия, с возможностью доработки или расширения функционала в дальнейшем. 

* **Используемые в разработке паттерны и фреймворки:**
  + Фреймворк: Materialize CSS

**9.2 Используемые паттерны выявления проблем [✋](https://github.com/stankin/design-part-2/wiki/sem3):**
* Муда: создание отчётности вручную. 
* Мура: обработка всех заказов в конце недели. 
* Мури: один менеджер при 100 заказах в день. 

**9.3 Возможные антипаттерны [✋](https://github.com/stankin/design-part-2/wiki/sem4):**

| Категория  | Антипаттерн (риск) | Действие по избежанию |
|---|---|---|
| Разработка | Таинственный код (Cryptic code) - использование аббревиатур вместо понятных имен | Задания имён переменным и функциям, в соотвествии с их назначением |
| Архитектура | Большой комок грязи (Big ball of mud) - программа с нераспознаваемой структурой | На этапе проектирования чётко определить структуру программы |
| Организация | Раздутый улучшизм (Creeping featurism) - добавление новых улучшений в ущерб суммарному качеству программы | Добавление только тех функций, которые действительно необходимы |
| Среда | Увлечение модными словами (Buzzword Mania) - руководство жонглирует словами, которые мало кто из подопечных понимает | Использование простых формулировок при общении с сотрудниками |

### 10. Интерпретация построенных моделей

**10.1 Определение числовых показателей для поставленной цели моделирования:**

Стандарт цели: определение автоматизируемых функций. 

**10.2 Определение числовых показателей для цели потенциального проекта автоматизации: [✋](https://github.com/stankin/design-1/wiki/interpret_process)**

**10.3 Расчет потенциального эффекта от автоматизации:**

**10.4 Определение числовых показателей и расчет трудозатрат на разработку программных средств:**

**ВЫВОДЫ**

