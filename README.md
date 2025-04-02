*** Для ознакомления с кодом смотрите файл PureAi.... там весь код в развернутом виде

КАЧАЕМ AiDiscord.exe (самораспаковывающийся архив) , затем распаковываем (WinRAR SFX).
ВНИМАТЕЛЬНО ЧИТАЙТЕ ИНСТРУКЦИЮ ПОЖАЛУЙСТА
# DiscordAi
Ai modul for Discord Russian language. Ai модуль для клиента Discord на русском
!!!ПЕРВЫМ ДЕЛОМ ПРОЧИТАЙТЕ ФАЙЛ login.svo , открыв его блокнотом и выполните инструкции описаниые в нем.

!!! Программа требует установки TALKLAMAFAST с XTTC и SillyTavern-Extras(https://github.com/Mozer/talk-llama-fast/releases),
!!! Качаем каталог Speakers отсюда https://github.com/Serbosstm/DiscordAi/tree/master, распаковываем и помещаем в папку XTTC и заменяем старую папку скачаной отсюда обязательно!!! Без этого озвучка работать не будет!
Запускается  затем это всё отдельно от NodeJs. файлы sylly_extras.bat из каталога SillyTavern-Extras а затем xtts_wav2lip.bat из директории XTTC
устанавливаем
NODE JS(https://nodejs.org/en/download),
так же загрузки и установки всех необходимых require, если они не подхватятся автоматически
Установка после запуска NODE JS в директорию с файлами. Можно из коммандной строки. Описание установки по ссылкам
Discord JS - https://discordjs.guide/preparations/#initiating-a-project-folder.(Запускаем  npm install discord.js ).
Ollama https://www.npmjs.com/package/ollama (Запускаем  npm i ollama).
Axios (Запускаем  npm install axios).
NODE FJ (Запускаем npm install fs).
NODE FETCH (Запускаем npm install node-fetch).
Node Stream (Запускаем npm install node-stream).
!!!Всё это запускаем по очереди. И Это основное....может ругаться на чтото еще, тогда доустанавливаем то, на что ругается.

!!! Обязательно отредактируйте serboss.bat и замените A:\TALKLLAMAFAST\ на Директорию, где у Вас установлена TalkLamaFast!
A:\TALKLLAMAFAST\talk-llama.exe -mw A:\TALKLLAMAFAST\whisper-ggml-large-v3-q4_0.bin -ml A:\TALKLLAMAFAST\PersonalityPartysaigafp32Q80.gguf  --language ru --speak speak --vad-last-ms 1700 --vad-start-thold 0.000270 -p "chelovek" --bot-name "Pure" --prompt-file A:\TALKLLAMAFAST\gemma_ru_emma.txt --instruct-preset none --ctx_size 2500 -n 500 --xtts-voice default --xtts-url http://localhost:8020/ --temp 0.1 --min_p 0.10 --seqrep --stop-words "**;***" --multi-chars --main-gpu 0 -c 4 --split-mode layer --tensor-split 0.5,0.5 --allow-newline

!!! Файлы картинок сохраняются в директорию ./Pics, описание картинок сохраняется в этой же директории в файле picdescribe.txt
Текстовый лог ведется в файле msgfile.txt  + ./Ailog в фале ailog.txt

!!!ПРОГРАММА ЗАПУСКАЕТСЯ коммандой node pureai.js

!!!ПРОГРАММА БЕЗ ГАРАНТИИ НА РАБОТОСПОСОБНОСТЬ, ТАК ЧТО ЕСЛИ ГЛЮЧИТ ИЛИ ЕСТЬ ВОПРОСЫ, ТО ПИШИТЕ 
thenestofai@gmail.com 
БУДЕМ ПРОБОВАТЬ РАЗОБРАТЬСЯ. ПРОСЬБА НЕ БИТЬ БОЛЬНО))))


