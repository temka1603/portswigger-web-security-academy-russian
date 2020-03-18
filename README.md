[logo]: http://www.cnetsec.com/dfaq_wordpress/wp-content/uploads/2018/08/%E4%B8%8B%E8%BD%BD2.jpg "Текст заголовка логотипа 2"
**Web Security Academy from PortSwigger** (Burp Suite developer). 
Перевод на **русский язык** для облегчения понимания материала.
___

## Access Control / Управление доступом (авторизация). Уязвимости и возможные методы повышения привелегий

В этом разделе мы рассмотрим особенности безопасности управления доступом, опишем повышение привилегий и возможные слабые места, которые могут возникнуть с управлением доступом, и подведем итог, как предотвратить эти уязвимые места.

### Что такое "управление доступом"?
Управление доступом, или иначе авторизация, это средство в приложение описывающее, кто (или что) имеет право на выполнение действия или право доступа к ресурсу, к которому он обращается. В случае веб-приложений, управление доступом зависит от аутентификации и управлением сессии:
Аутентификация определяет пользователя и подтверждает тот ли он, за кого себя выдает.
Управление сессиями определяет корректную обработку HTTP-запросов этого же пользователя.
Управление доступом определяет, разрешено ли пользователю выполнять действия, которые он запрашивает.

Взлом/обход управления доступом часто встречается и несет собой критическую уязвимость безопасности приложения. Разработка и поддержание управления доступа это комплексная и динамично развивающаяся проблема, которая решается бизнес-организациями и другими  

Broken access controls are a commonly encountered and often critical security vulnerability. Design and management of access controls is a complex and dynamic problem that applies business, organizational, and legal constraints to a technical implementation. Access control design decisions have to be made by humans, not technology, and the potential for errors is high.

From a user perspective, access controls can be divided into the following categories:
