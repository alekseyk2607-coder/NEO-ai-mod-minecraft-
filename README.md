RU
Полную папку загрузить не могу так как она очень большая.
Мод работает на Java Edition 26.2 Fabric и требует установку Fabric Api.
Скоро он пройдет модерацию на Modrinth

# NEO-ai-mod-minecraft-
AI-компаньон для Minecraft Java Edition, который живёт в игровом мире, общается с игроком и выполняет действия через подключаемую AI-модель.

описание.
# NEO AI Companion

**NEO AI Companion** — модификация для **Minecraft Java Edition**, которая добавляет в игру небольшого физического AI-компаньона.

NEO умеет общаться с игроком через игровой чат, понимать команды и выполнять различные действия в мире Minecraft. В качестве «мозга» используется подключаемая **OpenAI-compatible API**, поэтому модель и AI-провайдера можно выбирать отдельно от самой модификации.

Главная идея проекта — сделать AI не просто чат-ботом в интерфейсе, а **полноценным физическим персонажем внутри игрового мира**.

---

## 🤖 Что умеет NEO

### 💬 Общение

С NEO можно разговаривать прямо через игровой чат.

Компаньон может:

- отвечать на вопросы о Minecraft;
- объяснять игровые механики;
- реагировать на команды игрока;
- поддерживать обычный диалог;
- анализировать контекст происходящего;
- сообщать о своих действиях.

---

### 🧭 Физический компаньон

NEO существует в мире как настоящий игровой объект.

Он может:

- следовать за игроком;
- перемещаться по миру;
- сидеть;
- менять положение;
- находиться рядом с игроком;
- взаимодействовать с окружающим пространством;
- сообщать свои координаты.

Если расстояние между игроком и NEO становится слишком большим, компаньон определяет, что потерял игрока, и сообщает об этом в чате вместе со своими текущими координатами.

---

## 🏠 Помощь в строительстве

NEO может помогать игроку с небольшими строительными задачами.

Например, компаньон способен:

- предложить план небольшого дома;
- помочь с простыми строительными действиями;
- работать с ограниченным набором ресурсов;
- объяснить, что и где нужно построить.

При этом NEO не должен превращать игру в автоматический генератор огромных построек — проект ориентирован именно на **небольшого игрового помощника**.

---

## 🎒 Ресурсы

NEO может работать с некоторыми распространёнными ресурсами Minecraft.

Например:

- дерево;
- булыжник;
- уголь;
- другие обычные материалы.

Количество ресурсов ограничивается, чтобы компаньон не мог бесконечно создавать предметы или выдавать игроку редкие ресурсы.

**Алмазы и другие ценные ресурсы не выдаются произвольно.**

---

## 🧠 AI Architecture

NEO использует разделение между игровым кодом и AI-моделью.

Упрощённая схема работы:

```text
Minecraft
    ↓
NEO AI Companion
    ↓
Context / Game State
    ↓
OpenAI-compatible API
    ↓
AI Model
    ↓
Structured Action
    ↓
Action Validator
    ↓
Minecraft
```

AI не получает полный контроль над игрой.

Модель предлагает действие, после чего Java-часть мода проверяет его и только затем выполняет разрешённую операцию.

Это позволяет ограничивать потенциально опасные или нежелательные действия модели.

---

## 🔌 OpenAI-compatible API

NEO не привязан к одному конкретному AI-провайдеру.

В настройках можно указать:

- API Base URL;
- модель;
- API Key;
- другие параметры подключения.

Это позволяет использовать различные сервисы, поддерживающие совместимый API.

API-ключ хранится в конфигурации клиента и не должен публиковаться в чатах, логах или исходном коде.

---

## ⚙️ Настройка

Настройки AI-компаньона доступны через отдельный интерфейс.

Игрок может настроить подключение к AI-сервису и выбрать используемую модель.

Для удобства управление настройками доступно непосредственно из Minecraft через назначенную клавишу.

---

## 🔐 Безопасность

NEO построен с учётом того, что AI-модель не должна иметь безусловный контроль над игровым миром.

Поэтому действия проходят через ограничения и проверки на стороне мода.

Система учитывает:

- разрешённые действия;
- ограничения ресурсов;
- расстояния;
- контекст игрока;
- корректность команд;
- ограничения строительства;
- ошибки API;
- отсутствие ответа AI;
- некорректные действия модели.

---

## 🧪 Проект в разработке

NEO AI Companion — экспериментальный проект, посвящённый объединению **Minecraft, игровых AI-агентов и физических игровых персонажей**.

Проект продолжает развиваться: новые возможности, модели поведения и игровые действия могут добавляться со временем.

Главная идея NEO проста:

> **Не просто спросить AI о Minecraft — поселить его прямо внутри Minecraft.** 🤖

(описания ссылки будут добавляется со временем, мод будет развиваться и обновлятся следите за репозиторием Github и будущем Modrinth)
мое портфолио: https://portfolio-nhs.vercel.app/ 
Чтобы добавить API key, нажмите правый ALT в игре.

EN
I can’t upload the entire folder as it’s very large.
The mod works on Java Edition 26.2 Fabric
It will soon be moderated on Modrinth

# NEO-ai-mod-minecraft-
An AI companion for Minecraft Java Edition that lives in the game world, interacts with the player and performs actions via a pluggable AI model.

Description.
# NEO AI Companion

**NEO AI Companion** is a mod for **Minecraft Java Edition** that adds a small, physical AI companion to the game.

NEO can communicate with the player via the in-game chat, understand commands and perform various actions within the Minecraft world. A pluggable **OpenAI-compatible API** serves as its ‘brain’, so the model and AI provider can be selected independently of the mod itself.

The main idea behind the project is to make the AI not just a chatbot in the interface, but a **fully-fledged in-game character**.

---

## 🤖 What NEO can do

### 💬 Communication

You can talk to NEO directly via the in-game chat.

The companion can:

- answer questions about Minecraft;
- explain game mechanics;
- respond to the player’s commands;
- hold a normal conversation;
- analyse the context of what’s happening;
- report on its actions.

---

### 🧭 Physical companion

NEO exists in the world as a real in-game object.

It can:

- follow the player;
- move around the world;
- sit;
- change position;
- stay close to the player;
- interact with the surrounding environment;
- report its coordinates.

If the distance between the player and NEO becomes too great, the companion determines that it has lost track of the player and reports this in the chat, along with its current coordinates.

---

## 🏠 Building assistance

NEO can assist the player with small building tasks.

For example, the companion is capable of:

- suggesting a plan for a small house;
- helping with simple building tasks;
- working with a limited set of resources;
- explaining what needs to be built and where.

However, NEO is not intended to turn the game into an automatic generator of huge structures — the project is specifically designed to be a **small in-game helper**.

---

## 🎒 Resources

NEO can work with some common Minecraft resources.

For example:

- wood;
- cobblestone;
- coal;
- other common materials.

The quantity of resources is limited so that the companion cannot endlessly create items or give the player rare resources.

**Diamonds and other valuable resources are not given out arbitrarily.**

---

## 🧠 AI Architecture

NEO separates the game code from the AI model.

A simplified diagram of how it works:

```text
Minecraft
    ↓
NEO AI Companion
    ↓
Context / Game State
    ↓
OpenAI-compatible API
    ↓
AI Model
    ↓
Structured Action
    ↓
Action Validator
    ↓
Minecraft
```

The AI does not gain full control over the game.

The model proposes an action, after which the Java part of the mod checks it and only then executes the permitted operation.

This allows you to restrict potentially dangerous or undesirable actions by the model.

---

## 🔌 OpenAI-compatible API

NEO is not tied to any one specific AI provider.

In the settings, you can specify:

- API Base URL;
- model;
- API Key;
- other connection parameters.

This allows you to use various services that support a compatible API.

The API key is stored in the client’s configuration and must not be published in chat logs, logs or source code.

---

## ⚙️ Configuration

The AI companion’s settings are accessible via a separate interface.

Players can configure the connection to the AI service and select the model to be used.

For convenience, settings can be managed directly from within Minecraft using a hotkey.

---

## 🔐 Security

NEO is designed on the principle that the AI model must not have unrestricted control over the game world.

Therefore, actions are subject to restrictions and checks on the mod’s side.

The system takes into account:

- permitted actions;
- resource limitations;
- distances;
- the player’s context;
- the validity of commands;
- building restrictions;
- API errors;
- lack of response from the AI;
- incorrect actions by the model.

---

## 🧪 Project in development

NEO AI Companion is an experimental project dedicated to combining **Minecraft, in-game AI agents and physical in-game characters**.

The project is still evolving: new features, behaviour models and in-game actions may be added over time.

The main idea behind NEO is simple:

> **Don’t just ask the AI about Minecraft — put it right inside Minecraft.** 🤖

(Link descriptions will be added over time; the mod will be developed and updated – keep an eye on the GitHub repository and future Modrinth updates)
My portfolio: https://portfolio-nhs.vercel.app/
To add an API key, press the right ALT key whilst in the game.
