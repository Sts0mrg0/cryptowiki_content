Title: Gpg4Usb

Gpg4Usb - портативная программа для шифрования и электронной подписи данных.

Фактически, Gpg4Usb является графической надстройкой над GnuPG с текстовым редактором и удобным графическим интерфейсом.

### Создание пары ключей

Чтобы принимать зашифрованные сообщения, вам нужно сперва сгенерировать ключи шифрования.

Программа предлагает оптимальные параметры по-умолчанию, желательно указать уникальный e-mail и имя.

![1]({filename}/images/gpg4usb/genkey_step1_small.jpg)

![2]({filename}/images/gpg4usb/genkey_step2_small.jpg)

![3]({filename}/images/gpg4usb/genkey_step3_small.jpg)

![4]({filename}/images/gpg4usb/genkey_step4_small.jpg)

### Экспорт своего публичного ключа

Вы создали пару ключей, теперь вам нужно экспортировать свой публичный ключ и раздавать его всем желающим.

Откройте менеджер ключей:

![1]({filename}/images/gpg4usb/exportkey_open_keymgmt_small.jpg)

Выберите ключи, которые хотите экспортировать (на картинке выбрано два ключа, но вы отмечаете только свой):

![2]({filename}/images/gpg4usb/exportkey_choose_keys_small.jpg)

![3]({filename}/images/gpg4usb/exportkey_menu_selection_small.jpg)

![3]({filename}/images/gpg4usb/exportkey_file_selection_small.jpg)

В созданном файле теперь содержится ваш публичный ключ, этот текст вам и нужно раздавать в качестве публичного ключа.

### Импорт публичного ключа собеседника

Собеседник передал вам свой публичный ключ. Чтобы им воспользоваться, необходимо его импортировать.

![1]({filename}/images/gpg4usb/importkey_menu_small.jpg)

Выберите текстовый файл, в котором содержится публичный ключ для импорта:

![2]({filename}/images/gpg4usb/importkey_00_small.jpg)

![3]({filename}/images/gpg4usb/importkey_01_small.jpg)

Ключ импортирован:

![3]({filename}/images/gpg4usb/importkey_keylist_small.jpg)

### Шифрование сообщений публичным ключом

Введите сообщение для шифровки в текстовое поле программы:

![1]({filename}/images/gpg4usb/encrypt_step1_small.jpg)

Выберите в списке ключей для кого вы шифруете сообщение:

![2]({filename}/images/gpg4usb/encrypt_step2_small.jpg)

Нажмите зашифровать:

![3]({filename}/images/gpg4usb/encrypt_step3_small.jpg)

Получившийся текст передайте собеседнику.

### Расшифровка сообщения

Кто-то передал вам зашифрованное сообщение, вставьте его в текстовое поле программы:

![2]({filename}/images/gpg4usb/decrypt_step1_small.jpg)

Отметьте свой приватный ключ и нажмите кнопку расшифровать:

![3]({filename}/images/gpg4usb/decrypt_step2_small.jpg)

![4]({filename}/images/gpg4usb/decrypt_step3_small.jpg)

В текстовом поле появится расшифрованное сообщение:

![5]({filename}/images/gpg4usb/decrypt_step4_small.jpg)

### Перенос приватных ключей

Если требуется использовать одну пару ключей на нескольких устройствах, понадобится выполнить экспорт/импорт приватных ключей.

Откройте менеджер ключей:

![1]({filename}/images/gpg4usb/exportkey_open_keymgmt_small.jpg)

Правой кнопкой нажмите на свой ключ и выберите показать свойства ключа:

![2]({filename}/images/gpg4usb/exportkey_show_keydetails_small.jpg)

Нажмите экспортировать приватный ключ:

![3]({filename}/images/gpg4usb/exportkey_hit_export_private_key_small.jpg)

![4]({filename}/images/gpg4usb/exportkey_warn_message_small.jpg)

Выберите файл, в который будет сохранен ключ:

![5]({filename}/images/gpg4usb/exportkey_00_small.jpg)

Перенесите получившийся файл на другое устройство, только ни в коем случае не используйте для этого интернет!

Импорт приватного ключа производится так же, как и публичного (см. выше).

### Подпись сообщений

Подпись сообщений нужна для того, чтобы подтвердить авторство сообщения.
Если кто-то изменит текст оригинального сообщения, то при проверке подписи будет выдаваться ошибка.

Чтобы подписать сообщение, выберите свой ключ и нажмите подписать:

![1]({filename}/images/gpg4usb/signature_text_00_small.jpg)

![2]({filename}/images/gpg4usb/signature_text_01_small.jpg)

В текстовом поле содержится сообщение с вашей цифровой подписью.

### Проверка подписи сообщения

Чтобы проверить подпись в сообщении, вставьте его в текстовое поле, выберите ключ отправителя и нажмите проверить:

![3]({filename}/images/gpg4usb/signature_text_02_small.jpg)

Внизу окна появится результат проверки.

*Основано на материалах с сайта opennet.ru и xmail.net*
