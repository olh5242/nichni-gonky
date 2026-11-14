# Нічні гонки: збірка APK

## Спосіб 1. Без Android Studio (через GitHub, безкоштовно)
1. Створи акаунт на github.com і новий репозиторій (наприклад, nichni-gonky).
2. Завантаж у нього ВСІ файли з цього zip (кнопка Add file → Upload files). Папка .github теж має потрапити в репозиторій.
3. Відкрий вкладку Actions. Збірка запуститься сама (або натисни Run workflow).
4. Через 3-5 хвилин відкрий завершений запуск і внизу в Artifacts завантаж nichni-gonky-apk.
5. Розпакуй, скинь app-debug.apk на телефон, відкрий і дозволь встановлення з невідомих джерел.

## Спосіб 2. Через Android Studio
1. Встанови Node.js 20 і Android Studio.
2. У папці проєкту: npm install, потім npx cap add android, потім npx cap sync android.
3. npx cap open android, у Android Studio: Build → Build APK(s).

## Зміни в грі
Уся гра лежить у www/index.html. Після змін у способі 2 виконай npx cap sync android.
