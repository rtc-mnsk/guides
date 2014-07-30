Использование Jabber (XMPP) и плагина для шифрования OTR с помощью клиента Pidgin
---------------------------------------------------------------------------------
* [Что и зачем](#Что-и-зачем)
* [Установка Pidgin](#Установка-pidgin)
  * [Ubuntu и Linux Mint](#ubuntu-и-linux-mint)
  * [Windows 7 (Портативная версия)](#windows-7-Портативная-версия)
* [Создание и использование аккаунта](#Создание-и-использование-аккаунта)
  * [Публичные серверы XMPP](#Публичные-серверы-xmpp)
  * [Либертарные технические коллективы](#Либертарные-технические-коллективы)
* Установка и настройка плагина для OTR
* Чаты для нескольких пользователей

### Что и зачем
Jabber (XMPP) - это открытый протокол для обмена мгновенными сообщениями, который позволяет обеспечивать конфиденциальное общение за счет открытой инфраструктуры. Это означает, что мы сами можем выбрать сервер для своего аккаунта, избежать сохранения и контроля над своей перепиской третьей стороной, которой мы не доверяем (как в случае со Skype), дополнительно использовать средства шифрования OTR (Off-the-Record) для защиты от прослушки.

Мы рассмотрим свободный клиент Pidgin для использования Jabber вместе с OTR.

### Установка Pidgin
#### Ubuntu и Linux Mint
В системах Ubuntu и Linux Mint Pidgin может быть уже установлен. Если приложение не установлено, открываем Terminal и устанавливаем его с помощью команды:

	sudo apt-get install pidgin

#### Windows 7 (Портативная версия)
Скачиваем Pidgin с сайта [portableapps.com](http://portableapps.com/apps/internet/pidgin_portable).

<p align="center">
  <img src="/images/jabber-otr-pidgin/pidgin-download.png" alt="<Скачиваем Pidgin>"/>
</p>

После скачивания запускаем программу установки приложения PidginPortable_x.x.x.paf.exe  (версия программы будет меняться в зависимости от времени скачивания). Выбираем язык.

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
#### Регистрация нового аккаунта
##### Публичные серверы XMPP
Если у вас еще нет jabber-аккаунта и вам нужно его создать, вы можете воспользоваться любым сервером из этого [списка публичных серверов XMPP](https://list.jabber.at). Из этого списка мы рекомендуем использовать _jabber.ccc.de_. Создать аккаунт можно и на _dukgo.com_.

##### Либертарные технические коллективы
Однако мы советуем пользоваться сервисами, которые предоставляют либертарные технические коллективы, определенная репутация которых говорит о доверии к ним множества активистов. Ниже приведена таблица коллективов, предоставляющих jabber-аккаунт, название домена для выбора и условия создания аккаунта.

<table>
    <tr valign="top">
        <td><b>Коллектив</b></td>
        <td colspan="2"><b>Варианты домена</b></td>
        <td><b>Условия создания аккаунта</b></td>
    </tr>
    <tr valign="top">
        <td><a href="https://riseup.net">RiseUp</a></td>
        <td colspan="2">riseup.net</td>
        <td>Подать <a href="https://user.riseup.net/forms/new_user/first">запрос на создание аккаунта</a> (этот же аккаунт будет являться почтовым ящиком с таким же именем); ввести 2 кода-приглашения от уже существующих аккаунтов или подождать несколько дней</td>
    </tr>
    <tr valign="top">
        <td><a href="https://www.autistici.org">Autistici/Inventati</a>&nbsp;&nbsp;&nbsp;</td>
        <td>autistici.org<br>onenetbeyond.org<br>paranoici.org<br>hacari.com<br>hacari.net<br>insicuri.net<br>logorroici.org<br>stronzi.org<br>grrlz.net<br>anche.no<br>krutt.org<br>autoproduzioni.net<br>distruzione.org<br></td>
        <td>inventati.org<br>bastardi.net<br>hacari.org<br>insiberia.net<br>bruttocarattere.org<br>mortemale.org<br>autistiche.org<br>canaglie.org<br>canaglie.net<br>subvertising.org<br>cryptolab.net<br>privacyrequired.com</td>
        <td>Подать <a href="https://www.autistici.org/services">запрос на создание почтового ящика</a> (jabber-аккаунт с таким же именем будет создан автоматически)</td>
    </tr>
    <tr valign="top">
        <td><a href="https://www.draugr.de">Draugr.de</a></td>
        <td>draugr.de<br>deshalbfrei.org<br>brauchen.info<br>xabber.de</td>
        <td>ubuntu-jabber.de<br>ubuntu-jabber.net<br>verdammung.org</td>
        <td>Предварительная регистрация на сайте не требуется, аккаунт можно создать через клиент (есть защита от спама, придется ввести captcha)</td>
    </tr>
    <tr valign="top">
        <td><a href="https://www.free.de">Free!</a></td>
        <td colspan="2">free.de</td>
        <td><a href="https://faq.free.de/?action=register">Зарегистрироваться</a> для получения почтового ящика и автоматически jabber-аккаунта с таким же именем</td>
    </tr>
    <tr valign="top">
        <td><a href="https://www.systemli.org">systemli.org</a></td>
        <td colspan="2">jabber.systemli.org</td>
        <td>Аккаунт создается через клиент с перенаправлением на сайт, где нужно ввести пароль от создаваемого аккаунта (+ есть защита от спама)</td>
    </tr>
</table>

#### Использование аккаунта
При первом запуске Pidgin мы увидим окно приветствия.

<p align="center">
  <img src="/images/jabber-otr-pidgin/pidgin-account-welcome.png" alt="<Добро пожаловать в Pidgin!>"/>
</p>

Жмем "Добавить..." и переходим в окно добавления учетной записи.

<p align="center">
  <img src="/images/jabber-otr-pidgin/pidgin-account-new.png" alt="<Добавить учетную запись>"/>
</p>

Заполняем поля следующим образом:
_Протокол_: XMPP
_Имя пользователя_: уникальное имя пользователя вашего аккаунта (до символа @); естественно вы помните, что оно не должно содержать ваших реальных данных (имя, фамилия, дата рождения и т.д.)
_Домен_: название домена сервера XMPP (см. [Публичные серверы XMPP](#Публичные-серверы-xmpp) или таблицу с информацией о вариантах доменов различных [либертарных технических коллективов](#Либертарные-технические-коллективы))
_Ресурс_: необязательное поле; если вы пользуетесь своим jabber-аккаунтом в различных местах или с помощью различных устройств, вы можете указать в этом поле к примеру work, home, android и т.д.
_Пароль / Запомнить пароль_: пароль от вашего аккаунта; мы рекомендуем не вводить здесь пароль и не указывать, чтобы клиент его запоминал, в этом случае если злоумышленник получит доступ к вашей системе, то он не сможет автоматически зайти под вашим jabber-аккаунтом

Если вы создаете новый аккаунт с помощью самого клиента (напр., в случае dukgo.com или draugr.de), вам нужно выбрать "Создать эту новую учетную запись на сервере".

Заполнение остальных параметров пользователя остается на ваше усмотрение. В конце жмем на кнопку "Добавить".

<p align="center">
  <img src="/images/jabber-otr-pidgin/pidgin-add-account.png" alt="<Добавить учетную запись>"/>
</p>

Если вы создавали аккаунт с помощью клиента, то должно появиться окно для регистрации новой учетной записи, в котором вы указываете имя пользователя и пароль для вашего аккаунта и жмете "Зарегистрировать".

<p align="center">
  <img src="/images/jabber-otr-pidgin/pidgin-create-account.png" alt="<Зарегистрировать новую учетную запись>"/>
</p>

В случае успешной регистрации вы увидите подтверждение.

<p align="center">
  <img src="/images/jabber-otr-pidgin/pidgin-successful-registration.png" alt="<Регистрация завершена успешно>"/>
</p>

Если регистрацию выполнить не удалось, то вы увидите уведомление с пояснением причины: напр., имя пользователя может быть уже занято (конфликт имен) или сервер в данный момент может быть перегружен.

<p align="center">
  <img src="/images/jabber-otr-pidgin/pidgin-registration-conflict.png" alt="<Конфликт>"/>
  <img src="/images/jabber-otr-pidgin/pidgin-server-overload.png" alt="<Сервер перегружен>"/>
</p>


