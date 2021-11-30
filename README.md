Случайным образом были выбраны 10 000 записей, построена таблица со сравнением транскрипции ручной и автоматической, также вычислено расстояние Левенштейна. Из них, часть записей была удалена (там, где расстояние слишком большое или разница длины между двумя строками слишком большая).
Итого, для обучения использовалось 9590 файлов. На пробном запуске с одной эпохой и learning_rate равном 0.001, WER = 0.9998806967310905.
Также я пробовала увеличить количество записей для обучения примерно в два раза без очистки (так как получение автоматической транскрипции занимает слишком много времени), но Google Collab не позволил мне больше использовать GPU из-за лимитов.
Без GPU модель дообучить не получилось, так как на cpu технология AMP не поддерживается.
