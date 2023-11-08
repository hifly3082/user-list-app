## Задание

- Сверстать по макету отчет. В отчете вывести список юзеров.
- На странице есть поиск по юзерам. При вводе в строке поиска список фильтруется. При клике по карточке выводить в pop-up дополнительную информацию по юзеру. При нажатии вне окна с информацией или крестик окно закрывается.
- Список юзеров получаем с бэкенда. Для этого нужно установить и запустить локально сервер. Ссылка будет такой [http://127.0.0.1:3000](http://127.0.0.1:3000/). Для получения всего списка отправляем запрос без параметров, для получения совпадений ФИО со строкой ввода добавляем параметры query (term), например [http://127.0.0.1:3000?term=fer](http://127.0.0.1:3000/?term=fer)
- [Ссылка на макет](https://www.figma.com/file/sVohAvXP1UpHzN3MMLwmkB/%D0%97%D0%B0%D0%B4%D0%B0%D1%87%D0%B0-30080?node-id=0%3A1&t=kenPBeTH1t4zLitJ-0)
- [Ссылка на архив в бэкендом](https://drive.google.com/file/d/1bRxaW02JMJA1Z4CBWLv_-j6UzeHSrzJ_/view?usp=sharing)

## Решение

### Технологии

- Vite: версия 4.4.5
- React: версия 18.2.0
- TypeScript: версия 5.0.2

### Структура папок

- `/src`
  - `/components`
    - `AppLayout.tsx`
    - `Modal.tsx`
    - `Search.tsx`
    - `UserCard.tsx`
    - `UserCardList.tsx`
    - `UserInfo.tsx`
  - `/hooks`
    - `index.ts`
    - `useUsers.ts`
    - `useDebounce.ts`
- `App.css`
- `App.tsx`
- `main.tsx`

### Установка и запуск

1. Убедитесь, что у вас установлен Node.js и npm.
2. Клонируйте репозиторий проекта или создайте новый Vite проект.

```bash
git clone https://github.com/hifly3082/test-globexit.git
cd test-globexit
```

3. Перейдите в корневую директорию проекта.
4. Установите зависимости с помощью команды:

```bash
npm install
```

### Использование

Для запуска приложения

```bash
npm run dev
```

Также необходимо запустить [бэкэнд-сервер](https://github.com/hifly3082/backend-server).
