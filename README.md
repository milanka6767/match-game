# 1. Запуск и начальное состояние
# При запуске приложения открывается игровое окно. Пользователь видит перед собой сетку 4 на 4, состоящую из 16 синих карточек, под которыми скрыты иконки.
<img width="428" height="423" alt="image" src="https://github.com/user-attachments/assets/e033881e-2bb5-4cc8-a054-c2ae4ce5942a" />

# 2. Подготовка игрового поля
# При загрузке программы вызывается метод, который случайным образом распределяет иконки по карточкам. Каждая иконка встречается ровно два раза.
<img width="735" height="544" alt="image" src="https://github.com/user-attachments/assets/5074948f-63ca-4d29-85ae-7b8cc9ff9bb2" />
<img width="854" height="414" alt="image" src="https://github.com/user-attachments/assets/9763630d-fae5-42c4-b59d-b17318d89405" />

# 3. Ход игрока и проверка на совпадение
# Пользователь кликает по карточке левой кнопкой мыши. Срабатывает обработчик label1_Click. Программа запоминает первую нажатую карточку и делает её иконку видимой. Когда пользователь открывает вторую карточку, программа сравнивает текст на них. Если иконки совпали, карточки остаются открытыми, а переменные сбрасываются для поиска следующей пары.
<img width="766" height="383" alt="image" src="https://github.com/user-attachments/assets/0dd97e34-1951-49d1-8c9c-7e49dfd120a0" />
<img width="765" height="520" alt="image" src="https://github.com/user-attachments/assets/b00b672d-c056-48ad-9743-ae277e6858fe" />

# 5. Обработка ошибки (несовпадение)
# Если иконки не совпали, запускается таймер (интервал 0,75 сек). В это время игрок не может кликать по другим карточкам. По истечении времени таймер скрывает обе карточки обратно.
<img width="892" height="491" alt="image" src="https://github.com/user-attachments/assets/65e6d48c-9fb9-46ab-8ff2-1b88a8fa1531" />

# 6. Завершение игры
# Игра продолжается, пока не будут найдены все 8 пар. Как только закрытых карточек не остается, метод CheckForWinner() выводит окно с поздравлением.
<img width="692" height="655" alt="image" src="https://github.com/user-attachments/assets/c9b5e53d-0d46-40b7-b9e4-babb92fc3b2e" />
<img width="691" height="552" alt="image" src="https://github.com/user-attachments/assets/d189265c-fab8-4ae4-bd08-be7cd2b12f71" />
