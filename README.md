# 🍽️ Автоматизация калькуляции в школьной столовой (EduCater)

**Конфигурация для платформы 1С:Предприятие**

## 📄 Описание

Конфигурация **EduCater**, разработанная на платформе 1С, предназначена для автоматизации учета и калькуляции в школьных столовых. Она позволяет эффективно управлять меню, блюдами, рецептами, регистрировать питание учеников и сотрудников, а также вести складской учет сырья и формировать необходимую отчетность.

## 🚀 Установка конфигурации

**Требования:**

*   Платформа **1С:Предприятие 8**, версия **не ниже 8.3.24.1342**.

**Порядок установки:**

1.  Запустите 1С:Предприятие в режиме "Конфигуратор".
2.  **Если вы хотите создать новую, пустую базу данных с этой конфигурацией:**
    *   В меню выберите `Конфигурация` -> `Открыть конфигурацию`.
    *   Затем выберите `Конфигурация` -> `Загрузить конфигурацию из файла...`
    *   Укажите путь к файлу конфигурации (`.cf`).
    *   На вопрос об обновлении конфигурации базы данных ответьте утвердительно.
3.  **Если вы хотите загрузить базу данных с демонстрационными данными (если имеется файл `.dt`):**
    *   В меню выберите `Администрирование` -> `Загрузить информационную базу...`
    *   Укажите путь к файлу выгрузки информационной базы (`.dt`).
    *   **Внимание:** Это действие полностью заменит текущую информационную базу (если она была открыта). Рекомендуется выполнять на пустой или специально созданной для этого информационной базе.
4.  После загрузки конфигурации или информационной базы запустите 1С:Предприятие в режиме "Предприятие" для начала работы.

## 🌟 Основные возможности

*   **Управление меню и рецептами:** Создание меню на определенные даты, управление блюдами, их видами и рецептами (калькуляционными картами).
*   **Калькуляция и списание:** Автоматический расчет потребности в сырье согласно меню и его списание со склада.
*   **Учет питания:** Регистрация фактов питания учеников и сотрудников, прием заявок на питание.
*   **Складской учет:** Управление приходом, расходом, перемещением и списанием сырья (ингредиентов).
*   **Управление НСИ:** Ведение справочников сырья, единиц измерения, складов, поставщиков, сотрудников, классов, должностей.
*   **Отчетность:** Формирование отчетов по движению сырья (приход, расход, остатки), регистрации питания и списанию продуктов по меню.

## 📥 Входная информация

Система обрабатывает следующую входную информацию:

1.  Информация о сырье (ингредиентах)
2.  Информация о складах
3.  Информация о блюдах и их рецептах
4.  Информация о поставщиках
5.  Информация о сотрудниках
6.  Информация о классах (учебных группах)
7.  Данные для составления меню
8.  Заявки на питание

## 📤 Выходная информация (Отчеты)

На основе введенных данных система позволяет формировать следующие отчеты:

1.  Отчет по приходам сырья
2.  Отчет по остаткам сырья на складах
3.  Отчет по расходам сырья
4.  Отчет по регистрации питания
5.  Отчет по списанию сырья на меню (калькуляция)

## ⚙️ Структура Конфигурации (Подсистемы)

Конфигурация состоит из следующих функциональных подсистем:

### 🧑‍🍳 **Подсистема «Управление меню и блюдами»**

Обеспечивает планирование рациона и управление рецептурой.

*   Составление меню на конкретную дату.
*   Автоматический расчет и списание сырья по меню (калькуляция).
*   Управление блюдами (создание, редактирование карточек).
*   Управление рецептами блюд (состав ингредиентов, нормы закладки).
*   Управление единицами измерения.
*   Управление видами блюд (категории).
*   Формирование отчета по списанию на меню.

### 📋 **Подсистема «Управление питанием»**

Организация учета питающихся и регистрация предоставленных услуг.

*   Регистрация фактов питания (кто и когда питался).
*   Подача заявок на питание от классов и сотрудников.
*   Управление списком сотрудников.
*   Управление списком классов.
*   Управление должностями сотрудников.
*   Формирование отчета по регистрации питания.

### 📦 **Подсистема «Управление складом и запасами»**

Ведение учета сырья и материалов на складах столовой.

*   Учет прихода сырья (поступление от поставщиков).
*   Учет расхода сырья (кроме списания по меню, например, порча).
*   Учет перемещения сырья между складами (если их несколько).
*   Учет списания сырья (по разным причинам).
*   Редактирование номенклатуры сырья.
*   Редактирование информации о складах.
*   Редактирование информации о поставщиках.
*   Формирование отчетов по приходу, расходу и остаткам сырья.

## 📄 Лицензия

Этот проект лицензирован на условиях лицензии MIT - подробности см. в файле [LICENSE](LICENSE) (или `LICENSE.txt`), который должен находиться в корне репозитория. Автор: [Quvgard](https://github.com/Quvgard).
