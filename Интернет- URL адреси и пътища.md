# Интернет, URL адреси и пътища

## Интернет

Ах, магията на интернет...

Технически погледнато, това, което наричаме "интернет" днес, е просто една голяма група компютри, които са свързани помежду си по някакъв начин. За простота, можем да предполагаме, че са свързани с кабел. Поради огромния брой устройства с достъп до тази мрежа, очевидно няма директен кабел от всеки до всеки. От друга страна, има **път** между всеки две устройства, минаващ през други междинни такива. Може да си го представите ето така:

![](http://www.ecse.monash.edu.au/twiki/pub/InFocus/LargePacket-switchingNetworkTopologies/30h15r_pkswitch_net.png)

Може да си представите, че node15 е вашият компютър, а node44 е компютърът, на който се намира, да кажем, Facebook и всичките му данни.

## URL

URL (ю-ер-ел) е съкращение от [uniform resource locator](http://en.wikipedia.org/wiki/Uniform_resource_locator). Иначе казано, това е едно уникално име на ресурс (уеб страница, картинка, видео клип, ...), който се намира някъде в интернет. Браузърите използват URL адресите, когато се обръщат към всякакви ресурси, било то онлайн, или на вашия компютър.

Това е общият вид на един URL и отделните му съставни части:

**`scheme://hostname:port/path?query_string#fragment_id`**

Ето няколко примера на валидни URL-и:

1.  [](https://www.facebook.com/groups/RailsGirlsSofia/search/?query=ruby#search_form)https://www.facebook.com/groups/RailsGirlsSofia/search/?query=ruby#search_form
2.  [](http://dir.bg)http://dir.bg
3.  [](http://rubystudygroups.deedee.hno3.org/)http://rubystudygroups.deedee.hno3.org/
4.  [](file:///Users/dimitardimitrov/Rails%20Girls/Study%20Groups/homepage/index.html)file:///Users/dimitardimitrov/Rails%20Girls/Study%20Groups/homepage/index.html

Ще разгледаме всеки от компонентите на примерните URL-и и ще обясним каква роля има всеки един от тях.

**Scheme**

Схемата указва начина, по който браузърът (клиентът) трябва да се обърне към сървъра, за да поиска дадения ресурс. Още се нарича протокол (на комуникация). Най-често е или `http://`, или `https://`. И двете означават, че ще се ползва протокол за комуникация [HTTP](http://en.wikipedia.org/wiki/Hypertext_Transfer_Protocol), като разликата е, че в случая на HTTPS, връзката е криптирана, за да не могат трети страни да виждат какво се точи по "жиците", или пък да се намесват в целостта на данните. "Протокол за комуникация" е просто набор от правила, по които да се осъществява диалогът между клиент (браузър) и сървър.

В примерите по-горе, схемата има следните стойности:

1.  `https://` – криптирана връзка, протокол за комуникация - HTTP
2.  `http://` – некриптирана връзка, протокол за комуникация - HTTP
3.  `http://` – същото като т. 2
4.  `file://` – файлът се намира на същия компютър, на който е пуснат браузърът

**Hostname (domain)**

Този компонент идентифицира кой е компютърът из интернет, към който трябва да се обърне клиентът (браузърът), за да поиска въпросният ресурс (файл, картинка, ...) Понякога може да се срещне и като домейн (domain) или само хост (host).

В примерите от по-горе:

1.  www.facebook.com
2.  dir.bg
3.  rubystudygroups.deedee.hno3.org
4.  _няма –_ предполага се, че файлът е на същия компютър, на който е и браузърът

<undefined><li>IP адреси</li></undefined>

Всеки hostname (домейн) крие зад себе си едно число, грубо казано от нула до около 4 милиарда. Това загатва как е организирана комуникацията в интернет. Всеки сървър

порт: няма в примера; за протокол `https://` (= secure HTTP) се подразбира порт 443; за обикновено HTTP (`http://`) се подразбира порт 80, ако не е написано друго

път: `/groups/RailsGirlsSofia/search/`; ако няма нищо, се подразбира път `/`

query string: `?query=ruby`

fragment: `search_form`

## Пътища

"Път" е общо понятие, обикновено използвано за да се обозначи "адресът" (мястото), където се намира даден файл на нашия компютър.

**Абсолютни пътища**

**Релативни пътища**