# Architecture scraps


## About 3 layer architecture in enterprise programmer's sphere

Martin Fowler's articles:
* "PresentationDomainDataLayering"
https://martinfowler.com/bliki/PresentationDomainDataLayering.html

* "LayeringPrinciples"
https://martinfowler.com/bliki/LayeringPrinciples.html


## What is the difference between 3 tier architecture and a mvc?

I googled it and find 2 interested comments:
1) "... At first glance, the three tiers may seem similar to the model-view-controller (MVC) concept; however, topologically they are different. A fundamental rule in a three tier architecture is the client tier never communicates directly with the data tier; in a three-tier model all communication must pass through the middle tier. Conceptually the three-tier architecture is linear. However, the [model-view-controller] MVC architecture is triangular: the view sends updates to the controller, the controller updates the model, and the view gets updated directly from the model..."
https://stackoverflow.com/questions/10739914/what-is-the-difference-between-3-tier-architecture-and-a-mvc/10740184#10740184
Source: https://stackoverflow.com/a/10740045/6385361

2)
"... MVC is a pattern used to make UI code easier to maintain and test. When the MVC pattern is used a larger portion of the UI code can be unit tested.

Here is a good article which describes the MVC pattern in more detail: http://martinfowler.com/eaaDev/uiArchs.html

3 tier architecture is a pattern used for a completely different reason. It separates the entire application into meaningful "groups": UI, Business Logic, Data Storage.

So 3 tier application refers to all code in the application. The MVC pattern is a pattern used in the UI tier.

Here is a good article on the 3 tier architecture: http://dotnetslackers.com/articles/net/IntroductionTo3TierArchitecture.aspx

For further information you can search the internet and find a gazzilion articles on both subjects..."

Source: https://stackoverflow.com/a/10740184/6385361

.

"MVC - один из шаблонов реализации presentation-layer'а)
вообще в Microsoft application architecture guid очень подробно разжевано

в ms гайде есть четкое разделение - логический "слой" переводят как "layer" (DataAccess layer, Business logic layer, Service layer, Presentation layer), а физический - как "tier" (сюда отностися client/server, 3-tiers deployment, n-tiers deployment, сервера, распределяющие запросы, и т.д.)"
А. Иванов

.
###### Microservice architecutre

"... Как только в программе появляются повторяющиеся моменты или дублирующиеся функции, тогда и возникает необходимость в переходе на микросервисные компоненты. Чтобы не плодить в разных частях системы тысячи микрофункций, лучше разбить большой модуль на атомарные функции. Причем деление происходит до тех пор, пока не получается вычленить отдельные функции.

Если ранее монолитные сервисы реализовывали конкретные бизнес-функции, то сегодня микросервисы самостоятельных бизнес-функций не несут. Огромный плюс такой архитектуры в том, что можно реализовывать новые бизнес-функции, используя набор существующих микросервисов..."
http://hawkhouse.ru/blog/kogda-opravdano-ispolzovanie-mikroservisnoj-arhitektury/

.



"Что нужно знать, чтобы стать системным архитектором" - https://habrahabr.ru/company/technoserv/blog/344702/

"Chapter 21: Designing Web Applications" - https://msdn.microsoft.com/en-us/library/ee658099.aspx

"Создание архитектуры программы или как проектировать табуретку" - https://habrahabr.ru/post/276593/

"... То что она формироваться должна не по принципу «надо все продумать» а по принципу «не знаешь какое решение тут лучше, сделай проще и так, что бы было удобно переделать», это уже другое..."
https://habrahabr.ru/post/276593/

