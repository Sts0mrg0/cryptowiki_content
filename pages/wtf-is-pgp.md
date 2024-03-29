Title: PGP / GnuPG

### Шифрование с публичными ключами, a.k.a. Асимметричная криптография

Классические методы шифрования используют только один ключ (пароль). Отправитель шифрует сообщение с этим паролем, принимающий должен иметь тот же самый пароль для расшифровки. Пароль должен быть передан таким образом, чтобы никто не мог его перехватить. Но если кто-то на стороне узнает пароль, то он легко сможет все расшифровать/прочитать переписку.

Использование системы шифрования с публичным ключом решает эту проблему. В этой системе используется два ключа. Один ключ **публичный** (открытый), который может передаваться по любым каналам и быть известен всем. Другой ключ - **приватный** (секретный). Этот ключ держится в тайне и не должен быть известен никому, кроме владельца. Когда криптосистема правильно реализована, становится невозможным получить приватный ключ из публичного. Итак, теперь отправитель шифрует сообщение **публичным** ключом получателя. Расшифровка сообщения осуществляется **приватным** ключом получателя.

Критический момент в этой схеме: приватный ключ должен быть доступен только его владельцу и никому более! Его ни в коем случае нельзя передавать через интернет.

### Что такое PGP?

PGP — прикладная криптосистема, разработаная математиком Филиппом Циммерманом. Это первый продукт подобного уровня, который стал доступен простым смертным (ранее серьезные криптосистемы были только у военных и спецслужб). Изначальной целью разработки была защита гражданских прав пользователей Интернета, а основной задачей программы стало шифрование переписки по электронной почте.

Программа основана на криптографии с публичными ключами. Кроме шифрования данных, PGP так же применяется для электронной подписи.

Программа является условно-бесплатной, но распрострается с открытым исходным кодом. Для совместимости программ основанных на PGP был создан открытый стандарт OpenPGP.

### Что такое GPG / GnuPG?

GnuPG (GPG)  — свободный некоммерческий аналог PGP, основанный на стандарте OpenPGP. Разработка программы финансируется Федеральным министерством Германии по экономике и технике. 

Изначально разработка была нацелена на Linux, однако позднее была адаптирована и под Windows. GnuPG обладает аналогичными PGP возможностями шифрования / подписания текста и файлов. Работа с GnuPG осуществляется только из командной строки. Однако, благодаря простым интерфейсам программы, для нее существует ряд графических оболочек (напр. gpg4usb) и плагинов к популярным программам (напр. Enigmail для почтового клиента Mozilla Thunderbird).

### Читать далее

- [PGP на Windows (GPG4USB)]({filename}/pages/gpg4usb.md)
- [PGP на GNU/Linux (GnuPG)]({filename}/pages/gnupg.md)

*Основано на материалах с pgpru.com*
