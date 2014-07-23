Использование Jabber (XMPP) и плагина для шифрования OTR с помощью клиента Pidgin 
-------------
**(Что это такое, для чего это нужно, альтернативой чему является)**

Jabber (XMPP) - это открытый протокол для обмена мгновенными сообщениями, который позволяет обеспечивать конфиденциальное общение за счет открытой инфраструктуры. Это означает, что мы сами можем выбрать сервер для своего аккаунта, избежать сохранения и контроля над своей перепиской третьей стороной, которой мы не доверяем (как в случае со Skype), дополнительно использовать средства шифрования OTR (Off-the-Record) для защиты от прослушки.

Мы рассмотрим свободный клиент Pidgin для использования Jabber и OTR.

---

* Установка Pidgin
  * Ubuntu и Linux Mint
  * Windows 7 (Переносимая версия)
* Создание и использование аккаунта
* Установка и настройка плагина для OTR
* Чаты для нескольких пользователей

---------

Установка и настройка Pidgin
---------
### Ubuntu и Linux Mint
В системах Ubuntu и Linux Mint Pidgin может быть уже установлен. Если приложение не установлено, открываем Terminal и устанавливаем его с помощью команды:

	sudo apt-get install pidgin

### Windows 7 (Переносимая версия)
Скачиваем Pidgin с сайта [portableapps.com](http://portableapps.com/apps/internet/pidgin_portable).

![<Скачиваем Pidgin>](/images/pidgin/pidgin-download.png)

После скачивания запускаем программу установки приложения PidginPortable_x.x.x.paf.exe  (версия программы будет меняться в зависимоасти от времени скачивания). Выбираем язык.

![<Выбираем язык>](/images/pidgin/pidgin-installation-language.png)

В следующих окнах жмем "Далее" и переходим в окно выбора папки установки (а точнее распаковки) программы. Выбираем нужную папку на компьютере или флешке и жмем "Далее".

![<Выбор папки установки программы>](/images/pidgin/pidgin-installation-folder.png)

Нажимаем "Установить", ждем завершения процесса установки, выбираем "Запустить Pidgin Portable" и затем жмем "Готово".

![<Запустить Pidgin Portable>](/images/pidgin/pidgin-installation-done.png)

Создание и использование аккаунта
--------
При первом запуске Pidgin мы увидим окно приветствия.

![<Добро пожаловать в Pidgin!>](/images/pidgin/pidgin-account-welcome.png)

Жмем "Добавить..." и переходим в окно добавления учетной записи.

![<Добавить учетную запись>](/images/pidgin/pidgin-account-new.png)

Если вам нужно создать новый аккаунт, вы можете воспользоваться любым сервером из этого [списка публично доступных XMPP-серверов](https://list.jabber.at) (из которого мы рекомендуем использовать **jabber.ccc.de**) или **dukgo.com**. Однако мы советуем пользоваться сервисами, которые предоставляют либертарные технические коллективы, определенная репутация которых говорит о доверии к ним множества активистов. Ниже приведена таблица коллективов, предоставляющих jabber-аккаунт, название домена для выбора и условия создания аккаунта.

<table>
    <tr>
        <td><b>Коллектив&nbsp;&nbsp;&nbsp;</b></td>
        <td><b>Варианты домена&nbsp;&nbsp;&nbsp;</b></td>
        <td><b>Условия создания аккаунта&nbsp;&nbsp;&nbsp;</b></td>
    </tr>
    <tr>
        <td><a href="https://riseup.net">RiseUp</a></td>
        <td>riseup.net</td>
        <td>Подать <a href="https://user.riseup.net/forms/new_user/first">запрос на создание аккаунта</a> (этот же аккаунт будет являться почтовым ящиком с таким же именем); ввести 2 кода-приглашения от уже существующих аккаунтов или подождать пару дней</td>
    </tr>
    <tr>
        <td><a href="https://www.autistici.org">Autistici/Inventati</a>&nbsp;&nbsp;&nbsp;</td>
        <td>autistici.org<br>inventati.org<br>onenetbeyond.org<br>bastardi.net<br>paranoici.org<br>hacari.org<br>hacari.com<br>hacari.net<br>insiberia.net<br>insicuri.net<br>bruttocarattere.org<br>logorroici.org<br>mortemale.org<br>stronzi.org<br>autistiche.org<br>grrlz.net<br>canaglie.org<br>anche.no<br>canaglie.net<br>krutt.org<br>subvertising.org<br>autoproduzioni.net<br>cryptolab.net<br>distruzione.org<br>privacyrequired.com&nbsp;&nbsp;&nbsp;</td>
        <td>Подать <a href="https://www.autistici.org/services">запрос на создание почтового ящика</a> (jabber-аккаунт с таким же именем будет создан автоматически)</td>
    </tr>
    <tr>
        <td><a href="https://mayfirst.org">mayfirst.org</a></td>
        <td></td>
        <td></td>
    </tr>
</table>


