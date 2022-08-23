# Rote-Language-Memorization-Tool-Apps-Script-
I mainly learn through rote memorization, so I made a tool that would help me learn languages that I wanted to learn, I then made it so that it could be used to learn many of the world's major languages. 

Things to note before setting up:
1. The tool requires subscriptions to WordsAPI and the DeepLAPI, which both have free subscription ( which I personally use ) and should be enough for personal use.
2. The tool generally uses a translation which starts from english. For example, if I wanted to translate from Italian to Spanish, the program would translate the word from English to Italian, which it would display, and then to check your answer it would take the same word from English and translate to Spanish, therefore there may be some error on how correct the translated words may be.
3. The DeepLAPI only returns one word when translating, therefore a specific answer has to be given for the translation. I will keep looking to see if there is a translation API which translates to high accuracy and provides multiple answers. 


How to set up:
1. Open the google sheets document and make a copy, link is here: https://docs.google.com/spreadsheets/d/16gB8reD5KVKrqrr57dgxsl-DFaVZUZuTAp4YHllLXIU/edit#gid=882358459
2. Go to the extension tab and click "Apps Script", this will take you to the code which allows for the whole program to work. 
3. Get your WordsAPI key and type into the "WordsAPI" funciton after 'X-RapidAPI-Key'
4. Get your DeepL key and replace "https://api-free.deepl.com/v2/translate?auth_key=<YOUR DEEPL KEY>" with your url key.
5. Save
6. You need to set up two triggers, the first is the "punti function, which should trigger everyday between 00:00 and 01:00, and the second is the "event" function which should activate as on edit or on change of the spreadsheet.
7. Back on the spreadsheet, click the box which says "New Word", a window will pop-up asking for authorization to run the code( if it doesn't it' fine), authorize everything and enjoy the tool.

The last thing few things to note are:
1. The program will autmoatically produce a new word if you change the first language ( the language one the left which is alos the one which you are translating from )
2. Google Sheets only recognises that a cell has been changed when you press enter, so if nothing is happening it may be because you have not pressed enter.
3. If you click the "Swap" button, a new word with be produced, this is the same for the changing of difficulty.
4. The easy difficulty may include proper names so you can remove the row in the "Parole Inglese" sheet.

If there are any issues please tell and I will try my best to fix them, thank you and enjoy!
