Для распознавания текста я использовала сайт https://teamlogs.ru (к сожалению, бесплатно он размечает только пятнадцать минут, но, мне кажется, по пятнадцати минутам можно сделать выводы о качеств его работы,поэтому давайте представим, что у меня есть деньги на подписку)
С этого сайта я импортировала текст с таймкодами в формате субтитров
В поисках бесплатного распознавателя текстов, я наткнулась на сайт https://app.shopot.ai , то, как распозналось видео на нем сохранено в слое asr2@yds2006f, но, так как эта попытка автоматического распознавания оказалась существенно менее удачной (многие достаточно крупные фрагменты речи вообще не отражены в расшифровке), более подробно анализировать я буду первый вариант распознавания
Ошибки и неточности в автоматически распознанном тексте:
1) пропущенны многие хезитативы (э, м и др.)
2) пропущенны некоторые частицы (вот)
3) пропущенны некоторые союзы (и)
4) пропущены некоторые местоимения (это)
5) "ну" распознано как "но"
6) полностью не отражен фрагмент "и ещё так"
7) "вбивалось" распознано как "убивалось"
8) "так" распознано как "это"
9) "оно" распознано как "она" и "оставалось" распознано как "оставалась" в том же предложении

Возможные причины ошибок 1, 2, 3, 4 - незначительная длина данных слов, т.е. их сложнее отличить от постороннего шума, или обучение нейросети на основе письменных текстов, в которых слов-паразитов гораздо меньше; учитывая то, что почти все звуки, заполняющие паузы были убраны, можно также предположить, что нейросеть закономерно не отражает их на письме, считая несущественными, так как скорее всего создавалась она для отражения содержания текста в максимально приближенной к письменной речи форме 
Причиной ошибки 5 может быть то, что данное слово встретилось между двумя простыми предложениями, там, где слово "но" тоже вполне могло встретиться синтаксически, также слова "но" и "ну" достаточно схожи фонетически, поэтому в случае, если сеть распознала два возможных варианта, она могла выбрать более частотный
Причиной ошибки 6 может быть то, что здесь второстепенные члены оказались не между главными и они могли были быть удалены как хезитативы 
Причиной ошибки 7 может быть отсутствие в литературном языке слова "вбиваться" в значении "принуждать усвоить какую-либо информацию"
Причиной ошибки 8 может быть редуцированное произношение данного слова и контекст, в котором есть слово "устраивать, которое может употребляться и с "так"
Причиной ошибок 9 служит то, чтов потоке речи звуки [а] и [о] часто бывает трудно различить, а также то, что нейросеть стремится согласовать слова внутри предложения
