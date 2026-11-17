# Привет! Я Unity-разработчик

Проектирую и реализую игровые системы на **Unity / C#**: от взаимодействия с игровым миром и UI до кооперативного геймплея, ECS и серверных сохранений.

В проектах стараюсь разделять игровые правила, инфраструктуру и представление — так проще добавлять механики, проверять их и поддерживать код по мере роста игры.

## Избранные проекты

### [DoubleAdventure — кооперативная игра](https://github.com/Artemii0056/DoubleAdventure)

**Entitas (ECS) · FishNet · Zenject · UniTask · HTTP/JSON**

Игровые системы для кооператива на двух игроков: бой и противники на ECS, сетевые сессии, лобби, матчмейкинг, переподключения и прогресс аккаунта.

**Что посмотреть в коде:**
- [Управление сетевой сессией](https://github.com/Artemii0056/DoubleAdventure/blob/main/Scripts/Code/Core/SessionCoordinator.cs) — допуск игроков, готовность и запуск матча.
- [ECS и обработка урона](https://github.com/Artemii0056/DoubleAdventure/blob/main/Scripts/Code/Ecs/Modules/Damage/Systems/Resolution/ApplyDamageSystem.cs) — расчёт урона и взаимодействие боевых систем.
- [Сохранения через backend](https://github.com/Artemii0056/DoubleAdventure/blob/main/Scripts/Code/Infrastructure/Backend/Saves/BackendAccountSaveClient.cs) — ревизии данных и обработка конфликтов.

> В репозитории опубликован код игровых систем, а не полный проект для запуска в Unity.

### [Pick-up-adventure — взаимодействие с игровым миром](https://github.com/Artemii0056/Pick-up-adventure)

**Unity 6 · VContainer · New Input System · State Machine**

Тестовый 3D-проект с единой системой взаимодействий: нажатие и удержание, осмотр и перенос предметов, слоты с правилами размещения, NPC, диалоги и игровые механизмы.

**Что посмотреть в коде:** [диспетчер взаимодействий](https://github.com/Artemii0056/Pick-up-adventure/blob/main/Assets/_ProjectFiles/Interaction/Scripts/Core/InteractionFeatureService.cs) · [обработчики действий](https://github.com/Artemii0056/Pick-up-adventure/blob/main/Assets/_ProjectFiles/Interaction/Scripts/Core/TapFeatureServices/TapInteractionFeatureResolver.cs) · [перенос предметов](https://github.com/Artemii0056/Pick-up-adventure/blob/main/Assets/_ProjectFiles/Interaction/Scripts/Core/TransferServices/ItemTransferService.cs).

### [TestTaskInventory — система инвентаря](https://github.com/Artemii0056/TestTaskInventory)

**Unity · C# · MVP · VContainer · JSON**

Инвентарь на 50 слотов со стаками, последовательной разблокировкой ячеек, расходованием патронов, расчётом веса и сохранением прогресса. UI отделён от игровых правил.

**Что посмотреть в коде:** [логика инвентаря](https://github.com/Artemii0056/TestTaskInventory/blob/main/Assets/Scripts/Core/Systems/InventorySystem.cs) · [MVP Presenter](https://github.com/Artemii0056/TestTaskInventory/blob/main/Assets/Scripts/UI/InventoryScreen/Presenters/InventoryScreenPresenter.cs) · [маппинг сохранений](https://github.com/Artemii0056/TestTaskInventory/blob/main/Assets/Scripts/GameSaveDatas/InventorySaveMapper.cs).

## Технологии и направления

- **Gameplay:** C#, Unity, ECS (Entitas), State Machine, системы способностей, взаимодействий и инвентаря.
- **Архитектура:** DI (VContainer / Zenject), композиция, разделение логики и представления, MVP.
- **Multiplayer / backend:** FishNet, HTTP API, UniTask, сетевые сессии, JSON-сохранения.
- **Unity-инструменты:** ScriptableObject, New Input System, Addressables, uGUI, Git.

## Демонстрации

[Видео геймплея и реализованных механик (Google Drive)](https://drive.google.com/drive/folders/1H0HYuZB-G8zoUY_jYC058Y7hRHo4fglJ?usp=drive_link)

---

**Интересуют задачи на стыке gameplay-программирования, архитектуры игровых систем и сетевого взаимодействия.**
