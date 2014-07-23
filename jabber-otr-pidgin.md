Использование Jabber (XMPP) и плагина для шифрования OTR с помощью клиента Pidgin 
---------------------------------------------------------------------------------
* [Что и зачем](#Что-и-зачем)
* [Установка Pidgin](#Установка-pidgin)
  * [Ubuntu и Linux Mint](#ubuntu-и-linux-mint)
  * [Windows 7 (Портативная версия)](#windows-7-Портативная-версия)
* [Создание и использование аккаунта](#Создание-и-использование-аккаунта)
* Установка и настройка плагина для OTR
* Чаты для нескольких пользователей

### Что и зачем
Jabber (XMPP) - это открытый протокол для обмена мгновенными сообщениями, который позволяет обеспечивать конфиденциальное общение за счет открытой инфраструктуры. Это означает, что мы сами можем выбрать сервер для своего аккаунта, избежать сохранения и контроля над своей перепиской третьей стороной, которой мы не доверяем (как в случае со Skype), дополнительно использовать средства шифрования OTR (Off-the-Record) для защиты от прослушки.

Мы рассмотрим свободный клиент Pidgin для использования Jabber и OTR.

### Установка Pidgin
#### Ubuntu и Linux Mint
В системах Ubuntu и Linux Mint Pidgin может быть уже установлен. Если приложение не установлено, открываем Terminal и устанавливаем его с помощью команды:

	sudo apt-get install pidgin

#### Windows 7 (Портативная версия)
Скачиваем Pidgin с сайта [portableapps.com](http://portableapps.com/apps/internet/pidgin_portable).

<p align="center">
  <img src="/images/jabber-otr-pidgin/pidgin-download.png" alt="<Скачиваем Pidgin>"/>
</p>

После скачивания запускаем программу установки приложения PidginPortable_x.x.x.paf.exe  (версия программы будет меняться в зависимоасти от времени скачивания). Выбираем язык.

<p align="center">
  <img src="/images/jabber-otr-pidgin/pidgin-installation-language.png" alt="<Выбираем язык>"/>
</p>

В следующих окнах жмем "Далее" и переходим в окно выбора папки установки (а точнее распаковки) программы. Выбираем нужную папку на компьютере или флешке и жмем "Далее".

<p align="center">
  <img src="/images/jabber-otr-pidgin/pidgin-installation-folder.png" alt="<Выбор папки установки программы>"/>
</p>

Нажимаем "Установить", ждем завершения процесса установки, выбираем "Запустить Pidgin Portable" и затем жмем "Готово".

<p align="center">
  <img src="/images/jabber-otr-pidgin/pidgin-installation-done.png" alt="<Запустить Pidgin Portable>"/>
</p>

### Создание и использование аккаунта
При первом запуске Pidgin мы увидим окно приветствия.

<p align="center">
  <img src="/images/jabber-otr-pidgin/pidgin-account-welcome.png" alt="<Добро пожаловать в Pidgin!>"/>
</p>

Жмем "Добавить..." и переходим в окно добавления учетной записи.

<p align="center">
  <img src="/images/jabber-otr-pidgin/pidgin-account-new.png" alt="<Добавить учетную запись>"/>
</p>

Если вам нужно создать новый аккаунт, вы можете воспользоваться любым сервером из этого [списка публично доступных XMPP-серверов](https://list.jabber.at) (из которого мы рекомендуем использовать **jabber.ccc.de**) или **dukgo.com**. Однако мы советуем пользоваться сервисами, которые предоставляют либертарные технические коллективы, определенная репутация которых говорит о доверии к ним множества активистов. Ниже приведена таблица коллективов, предоставляющих jabber-аккаунт, название домена для выбора и условия создания аккаунта.

<table>
    <tr valign="top">
        <td><b>Коллектив&nbsp;&nbsp;&nbsp;</b></td>
        <td colspan="2"><b>Варианты домена&nbsp;&nbsp;&nbsp;</b></td>
        <td><b>Условия создания аккаунта&nbsp;&nbsp;&nbsp;</b></td>
    </tr>
    <tr valign="top">
        <td><a href="https://riseup.net">RiseUp</a></td>
        <td colspan="2">riseup.net</td>
        <td>Подать <a href="https://user.riseup.net/forms/new_user/first">запрос на создание аккаунта</a> (этот же аккаунт будет являться почтовым ящиком с таким же именем); ввести 2 кода-приглашения от уже существующих аккаунтов или подождать несколько дней</td>
    </tr>
    <tr valign="top">
        <td><a href="https://www.autistici.org">Autistici/Inventati</a>&nbsp;&nbsp;&nbsp;</td>
        <td>autistici.org<br>onenetbeyond.org<br>paranoici.org<br>hacari.com<br>hacari.net<br>insicuri.net<br>logorroici.org<br>stronzi.org<br>grrlz.net<br>anche.no<br>krutt.org<br>autoproduzioni.net&nbsp;&nbsp;&nbsp;<br>distruzione.org<br></td>

<td>inventati.org<br>bastardi.net<br>hacari.org<br>insiberia.net<br>bruttocarattere.org<br>mortemale.org<br>autistiche.org<br>canaglie.org<br>canaglie.net<br>subvertising.org<br>cryptolab.net<br>privacyrequired.com&nbsp;&nbsp;&nbsp;</td>
        <td>Подать <a href="https://www.autistici.org/services">запрос на создание почтового ящика</a> (jabber-аккаунт с таким же именем будет создан автоматически)</td>
    </tr>
    <tr valign="top">
        <td><a href="https://mayfirst.org">mayfirst.org</a></td>
        <td colspan="2"></td>
        <td></td>
    </tr>
</table>


