# Flexible Pricing
Оформление тест-кейсов на основе имеющихся требований. ![alt text](file:///Users/tengizusupov/Library/Containers/com.apple.Safari/Data/Downloads/Untitled%20Diagram.drawio-5.html) 
В рамках данного тестового задания было составлено 7 тест-кейсов.
Оставшиеся вопросы и замечания по требованиям:
1. Что необходимо сделать, если событие найдено и EventState.id = "0" or "2"?
2. Что должно произойти, если ВС отправт пустое сообщение?
3. Не допущена ли ошибка в ответе OutputRs во ВС: scName = InputRq.scSystem и spName = "spSystem"? Возможно имелось в виду: scName = InputRq.scName and
spName = InputRq.spName.
4. Не допущена ли ошибка в тексте: "Если сообщение не найдено, то перейти к шагу проверки полученного события"? Возможно имелось в виду: "Если событие не найдено, то перейти к шагу проверки полученного сообщения".
5. Первая и вторая проверки противоречат друг дуруг: на первой проверке мы можем найти  незакрытый фактор и завершить обработку сообщения отправой во ВС ответа OutputRs с некорретной ошибкой. Возможно проверки осущетсвяются в двух разных таблицах - необходимо указать.
6. Первая проверка, в случае провала, не предусматривает текста с описанием ошибки.
7. Чему равен парамметр stateDescription в ответе OutputRs: stateDescription = event_state_descr для выбранного EventState.id or stateDescription = EventState.description для выбранного EventState.id? Что такое и где взять EventState.id?
8. Осуществлять поиск клиента в таблице client по идентификатору клиента EPKID (п.3) -  как узнать EPKID клиента?
9. Что необходимо сохранять в логах и таблице событий event, в случае провала поиск клиента, какие поля?
10. Что означает п.4 - регистрация клиента в client? Зачем регистировать уже сущетсвующего клиента?
