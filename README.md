# cmd-lab
cmd laboratory

C:\Windows\system32>CD\

C:\>MD F (создание католога F)

C:\>CD F (смена текущего каталога на F)

C:\F>MD AUTO

C:\F>MD BIG

C:\F>MD BAG

C:\F>MD WP
![image](https://github.com/KurakAlina/cmd-lab/assets/148537804/cbaedeff-3b4f-4a85-8ed2-6ed6d4a5ea78)

C:\F>CD AUTO

C:\F\AUTO>MD USER

C:\F\AUTO>CD USER

C:\F\AUTO\USER>MD XXX

C:\F\AUTO\USER>MD TTT

C:\F\AUTO\USER>MD PPP

C:\F\AUTO\USER>CD\ (выход из всех каталогов)

C:\>CD F

C:\F>CD WP

C:\F\WP>MD IBM

C:\F\WP>CD IBM

C:\F\WP\IBM>MD PC

C:\F\WP\IBM>MD XT

C:\F\WP\IBM>TREE C:\F (вывод дерева)
Folder PATH listing
Volume serial number is D6DE-B126
C:\F
├───AUTO
│   └───USER
│       ├───PPP
│       ├───TTT
│       └───XXX
├───BAG
├───BIG
└───WP
    └───IBM
        ├───PC
        └───XT

C:\F\WP\IBM>CD ..

C:\F\WP>CD ..

C:\F>RD /s /q C:\F\AUTO\USER\PPP (удаление подкаталога PPP)

C:\F>TREE C:\F\AUTO\USER (вывод дерева каталога USER без PPP)
Folder PATH listing
Volume serial number is D6DE-B126
C:\F\AUTO\USER
├───TTT
└───XXX

C:\F>CD WP

C:\F\WP>CD IBM

C:\F\WP\IBM>CD XT

C:\F\WP\IBM\XT>COPY CON KURAK.TXT (создание текстового файла ФАМИЛИЯ)
KURAK A.V.
^Z
        1 file(s) copied.

C:\F\WP\IBM\XT>COPY CON ALINA.TXT (создание текстового файла ИМЯ)
UIR
^Z
        1 file(s) copied.

C:\F\WP\IBM\XT>COPY CON VLADIMIROVNA.TXT (создание текстового файла ОТЧЕСТВО)
ECONOMIC
^Z
        1 file(s) copied.
        ![image](https://github.com/KurakAlina/cmd-lab/assets/148537804/142651fd-b185-480a-aa8a-2bf6494075e6)


C:\F\WP\IBM\XT>COPY KURAK.TXT + ALINA.TXT + VLADIMIROVNA.TXT (объединение файлов в ФАМИЛИЮ)
KURAK.TXT
ALINA.TXT
VLADIMIROVNA.TXT
        1 file(s) copied.

C:\F\WP\IBM\XT>TYPE KURAK.TXT (просмотр содержимого файла ФАМИЛИЯ)
KURAK A.V.
UIR
ECONOMIC
![image](https://github.com/KurakAlina/cmd-lab/assets/148537804/b0540cfa-4e4f-4d6e-a9b0-cf4e0225bcc2)


C:\F\WP\IBM\XT>DEL KURAK.TXT (удаление файла ФАМИЛИЯ)
![image](https://github.com/KurakAlina/cmd-lab/assets/148537804/b271d712-2e9e-4f87-a791-595f169412e7)


C:\F\WP\IBM\XT>REN ALINA.TXT LANA.TXT (переименование файла ИМЯ)

C:\F\WP\IBM\XT>COPY VLADIMIROVNA.TXT C:\F\AUTO\USER\XXX (копирование файла ОТЧЕСТВО)
        1 file(s) copied.

C:\F\WP\IBM\XT>MOVE LANA.TXT C:\F\BAG (перенос переименованого файла в каталог BAG)
        1 file(s) moved.

C:\F\WP\IBM\XT>CD\

C:\>CD F

C:\F>XCOPY C:\F\WP\IBM C:\F\AUTO\FIO /e (копирование каталога IBM в каталог AUTO под новым именем FIO)
Does C:\F\AUTO\FIO specify a file name
or directory name on the target
(F = file, D = directory)? d
C:\F\WP\IBM\XT\VLADIMIROVNA.TXT
1 File(s) copied

C:\F>
C:\F>MOVE C:\F\WP\IBM C:\F\AUTO\USER (перенос каталога IBM со всем содержимым в каталог USER с прежним именем)
        1 dir(s) moved.

C:\F>RD /s /q C:\F\AUTO\USER\IBM (удаление каталога IBM)

C:\F>TREE C:\F (вывод на печать дерево каталогов с файлами)
Folder PATH listing
Volume serial number is 00000282 D6DE:B126
C:\F
├───AUTO
│   ├───FIO
│   │   ├───PC
│   │   └───XT
│   └───USER
│       ├───TTT
│       └───XXX
├───BAG
├───BIG
└───WP

C:\F>CD ..

C:\>RD /s /q F (удаление каталога F)

C:\>
