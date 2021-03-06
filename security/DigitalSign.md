# Электронная подпись
*Электронная подпись* (ЭП), *Электронная цифровая подпись* (ЭЦП)  — это криптографическое средство, которое позволяет удостовериться в отсутствие искажений в тексте электронного документа, а в соответствующих случаях - идентифицировать лицо, создавшее такую подпись.

##Виды электронной подписи

*   •	*Простая электронная подпись* (ПЭП) Предназначена для документооборота, позволяет подтвердить авторство, но не гарантирует неизменность документа после его подписания и не обеспечивают юридическую значимость. Простая электронная подпись применяется для получения доступа к возможностям Единого портала госуслуг. 
*   •	*Неквалифицированная электронная подпись* (НЭП) Позволяет определить автора подписанного документа и доказать неизменность содержащейся в нем информации. В неквалифицированную электронную подпись заложены криптографические алгоритмы, которые обеспечивают защиту документов. Такая подпись подойдет для внутреннего документооборота, а также для отправки электронных документов из одной компании в другую. Во втором случае, стороны должны заключить между собой соглашение, устанавливающие правила использования и признания электронных подписей. Неквалифицированная электронная подпись также подходит для участия в электронных торгах. 
*   •	*Квалифицированная электронная подпись* (КЭП) Квалифицированная электронная подпись обладает всеми признаками неквалифицированной, однако она может быть получена только в удостоверяющем центре, аккредитованном Минкомсвязи России. Программное обеспечение, необходимое для работы с КЭП, должно быть сертифицировано Федеральной службой безопасности. Следовательно, квалифицированная электронная подпись наделяет документы полной юридической силой и соответствует всем требованиям о защите конфиденциальной информацию. КЭП используется для сдачи отчетности в контролирующие органы государственной власти и для участия в электронных торгах.

##   Где используется электронная подпись? 

*   •	Электронные торги Электронные торги — это современная форма торговли, при которой заказы на поставку товаров или услуг размещаются на специализированных электронных площадках, которые находятся в Интернете. Участники электронных торгов имеют доступ к государственным закупкам и закупкам коммерческих фирм. Электронные торги открыты для юридических и физических лиц. Электронная подпись необходима для прохождения аккредитации на торговых площадках. Также электронной подписью заверяются документы, необходимые для участия в конкурсе, подачи ценового предложения и подписания контракта с победителем. Вид используемой электронной подписи определяется самой площадкой, на которой проходят торги.
*   •	Электронный документооборот. Электронный документооборот — это способ обмена документами, который осуществляется с помощью специализированной электронной системы, через сеть Интернет. Систему электронного документооборота используют крупные и мелкие компании с целью отправки информации сотрудникам внутри компании и внешним контрагентам, а также физические лица. Электронная подпись необходима для того, чтобы обмениваться через Интернет не только чисто информативными письмами, но также юридически значимыми документами: договорами, актами, счетами-фактур и другим. Для организации такого документооборота можно использовать любой вид электронной подписи: все зависит от целей, стоящих перед пользователем, а также от его договоренности с другими участниками электронного обмена.
*   •	Электронная отчетность. Процесс сдачи отчетности в контролирующие органы власти становится намного проще благодаря электронной подписи. Ежеквартальные отчеты для налоговой, пенсионного фонда и другое теперь можно заполнять в электронных бланках, заверять электронной подписью и отправлять через Интернет. Система электронной отчетности значительно экономит рабочее время, гарантирует конфиденциальность данных, а также сканирует отчет на наличие в нем ошибок, что является неоспоримым преимуществом. Для сдачи отчетности будет необходима квалифицированная электронная подпись.

Существует несколько схем построения цифровой подписи:

*   На основе алгоритмов симметричного шифрования. Данная схема предусматривает наличие в системе третьего лица — арбитра, пользующегося доверием обеих сторон. Авторизацией документа является сам факт зашифрования его секретным ключом и передача его арбитру 
*   На основе алгоритмов асимметричного шифрования. На данный момент такие схемы ЭП наиболее распространены и находят широкое применение.

*   Кроме этого, существуют другие разновидности цифровых подписей (групповая подпись, неоспоримая подпись, доверенная подпись), которые являются модификациями описанных выше схем. Их появление обусловлено разнообразием задач, решаемых с помощью ЭП.

##Использование хэш-функций 

Поскольку подписываемые документы — переменного (и как правило достаточно большого) объёма, в схемах ЭП зачастую подпись ставится не на сам документ, а на его хэш. Для вычисления хэша используются криптографические хэш-функции, что гарантирует выявление изменений документа при проверке подписи. Хэш-функции не являются частью алгоритма ЭП, поэтому в схеме может быть использована любая надёжная хэш-функция.

Использование хэш-функций даёт следующие преимущества:

*Вычислительная сложность*. Обычно хэш цифрового документа делается во много раз меньшего объёма, чем объём исходного документа, и алгоритмы вычисления хэша являются более быстрыми, чем алгоритмы ЭП. Поэтому формировать хэш документа и подписывать его получается намного быстрее, чем подписывать сам документ.

*Совместимость*. Большинство алгоритмов оперирует со строками бит данных, но некоторые используют другие представления. Хэш-функцию можно использовать для преобразования произвольного входного текста в подходящий формат.

*Целостность*. Без использования хэш-функции большой электронный документ в некоторых схемах нужно разделять на достаточно малые блоки для применения ЭП. При верификации невозможно определить, все ли блоки получены и в правильном ли они порядке.

Использование хэш-функции не обязательно при электронной подписи, а сама функция не является частью алгоритма ЭП, поэтому хэш-функция может использоваться любая или не использоваться вообще.

В большинстве ранних систем ЭП использовались функции с секретом, которые по своему назначению близки к односторонним функциям. Такие системы уязвимы к атакам с использованием открытого ключа, так как, выбрав произвольную цифровую подпись и применив к ней алгоритм верификации, можно получить исходный текст. Чтобы избежать этого, вместе с цифровой подписью используется хэш-функция, то есть, вычисление подписи осуществляется не относительно самого документа, а относительно его хэша. В этом случае в результате верификации можно получить только хэш исходного текста, следовательно, если используемая хэш-функция криптографически стойкая, то получить исходный текст будет вычислительно сложно, а значит атака такого типа становится невозможной.

##Симметричная схема

Симметричные схемы ЭП менее распространены чем асимметричные, так как после появления концепции цифровой подписи не удалось реализовать эффективные алгоритмы подписи, основанные на известных в то время симметричных шифрах. Первыми, кто обратил внимание на возможность симметричной схемы цифровой подписи, были основоположники самого понятия ЭП Диффи и Хеллман, которые опубликовали описание алгоритма подписи одного бита с помощью блочного шифра. Асимметричные схемы цифровой подписи опираются на вычислительно сложные задачи, сложность которых ещё не доказана, поэтому невозможно определить, будут ли эти схемы сломаны в ближайшее время, как это произошло со схемой, основанной на задаче об укладке ранца. Также для увеличения криптостойкости нужно увеличивать длину ключей, что приводит к необходимости переписывать программы, реализующие асимметричные схемы, и в некоторых случаях перепроектировать аппаратуру. 

Симметричные схемы основаны на хорошо изученных блочных шифрах. В связи с этим симметричные схемы имеют следующие преимущества:

Стойкость симметричных схем ЭП вытекает из стойкости используемых блочных шифров, надежность которых также хорошо изучена.

Если стойкость шифра окажется недостаточной, его легко можно будет заменить на более стойкий с минимальными изменениями в реализации.

Однако у симметричных ЭП есть и ряд недостатков:

Нужно подписывать отдельно каждый бит передаваемой информации, что приводит к значительному увеличению подписи. Подпись может превосходить сообщение по размеру на два порядка.

Сгенерированные для подписи ключи могут быть использованы только один раз, так как после подписывания раскрывается половина секретного ключа.

Из-за рассмотренных недостатков симметричная схема ЭЦП Диффи-Хелмана не применяется, а используется её модификация, разработанная Березиным и Дорошкевичем, в которой подписывается сразу группа из нескольких бит. Это приводит к уменьшению размеров подписи, но к увеличению объёма вычислений. Для преодоления проблемы «одноразовости» ключей используется генерация отдельных ключей из главного ключа.

##Асимметричная схема

	
![Схема](https://upload.wikimedia.org/wikipedia/commons/thumb/c/c4/Digital_Signature_diagram_ru.png/714px-Digital_Signature_diagram_ru.png "Рис.1")
 
Схема, поясняющая алгоритмы подписи и проверки

Асимметричные схемы ЭП относятся к криптосистемам с открытым ключом. В отличие от асимметричных алгоритмов шифрования, в которых шифрование производится с помощью открытого ключа, а расшифровка — с помощью закрытого, в асимметричных схемах цифровой подписи подписание производится с применением закрытого ключа, а проверка подписи — с применением открытого.

Общепризнанная схема цифровой подписи охватывает три процесса:
•	  Генерация ключевой пары. При помощи алгоритма генерации ключа равновероятным образом из набора возможных закрытых ключей выбирается закрытый ключ, вычисляется соответствующий ему открытый ключ.

•	  Формирование подписи. Для заданного электронного документа с помощью закрытого ключа вычисляется подпись.

• 	Проверка (верификация) подписи. Для данных документа и подписи с помощью открытого ключа определяется действительность подписи.

Для того, чтобы использование цифровой подписи имело смысл, необходимо выполнение двух условий:

*   Верификация подписи должна производиться открытым ключом, соответствующим именно тому закрытому ключу, который использовался при подписании.

*   Без обладания закрытым ключом должно быть вычислительно сложно создать легитимную цифровую подпись.

Следует отличать электронную цифровую подпись от кода аутентичности сообщения (MAC).

###Виды асимметричных алгоритмов

Как было сказано выше, чтобы применение ЭП имело смысл, необходимо, чтобы вычисление легитимной подписи без знания закрытого ключа было вычислительно сложным процессом.

Обеспечение этого во всех асимметричных алгоритмах цифровой подписи опирается на следующие вычислительные задачи:

*   Задачу дискретного логарифмирования (EGSA)

*   Задачу факторизации, то есть разложения числа на простые множители (RSA)

Вычисления тоже могут производиться двумя способами: на базе математического аппарата эллиптических кривых (ГОСТ Р 34.10-2012, ECDSA) и на базе полей Галуа(ГОСТ Р 34.10-94, DSA). В настоящее время самые быстрые алгоритмы дискретного логарифмирования и факторизации являются субэкспоненциальными. Принадлежность самих задач к классу NP-полных не доказана.

Алгоритмы ЭП подразделяются на обычные цифровые подписи и на цифровые подписи с восстановлением документа. При верификации цифровых подписей с восстановлением документа тело документа восстанавливается автоматически, его не нужно прикреплять к подписи. Обычные цифровые подписи требуют присоединение документа к подписи. Ясно, что все алгоритмы, подписывающие хэш документа, относятся к обычным ЭП. К ЭП с восстановлением документа относится, в частности, RSA.

Схемы электронной подписи могут быть одноразовыми и многоразовыми. В одноразовых схемах после проверки подлинности подписи необходимо провести замену ключей, в многоразовых схемах это делать не требуется.

Также алгоритмы ЭП делятся на детерминированные и вероятностные. Детерминированные ЭП при одинаковых входных данных вычисляют одинаковую подпись. Реализация вероятностных алгоритмов более сложна, так как требует надежный источник энтропии, но при одинаковых входных данных подписи могут быть различны, что увеличивает криптостойкость. В настоящее время многие детерминированные схемы модифицированы в вероятностные.

В некоторых случаях, таких как потоковая передача данных, алгоритмы ЭП могут оказаться слишком медленными. В таких случаях применяется быстрая цифровая подпись. Ускорение подписи достигается алгоритмами с меньшим количеством модульных вычислений и переходом к принципиально другим методам расчёта.

###Перечень алгоритмов ЭП

Асимметричные схемы:

FDH (Full Domain Hash), вероятностная схема RSA-PSS (Probabilistic Signature Scheme), схемы стандарта PKCS#1 и другие схемы, основанные на алгоритме RSA

Схема Эль-Гамаля

Американские стандарты электронной цифровой подписи: DSA, ECDSA (DSA на основе аппарата эллиптических кривых)

Российские стандарты электронной цифровой подписи: ГОСТ Р 34.10-94 (в настоящее время не действует), ГОСТ Р 34.10-2012

Украинский стандарт электронной цифровой подписи ДСТУ 4145-2002

Белорусский стандарт электронной цифровой подписи СТБ 1176.2-99 (в настоящее время не действует), СТБ 34.101.45-2013

Схема Шнорра

Pointcheval-Stern signature algorithm

Вероятностная схема подписи Рабина

Схема BLS (Boneh-Lynn-Shacham)

Схема GMR (Goldwasser-Micali-Rivest)

На основе асимметричных схем созданы модификации цифровой подписи, отвечающие различным требованиям:

Групповая цифровая подпись

Неоспоримая цифровая подпись

«Слепая» цифровая подпись и справедливая «слепая» подпись

Конфиденциальная цифровая подпись

Цифровая подпись с доказуемостью подделки

Доверенная цифровая подпись

Разовая цифровая подпись

##Управление открытыми ключами 

Важной проблемой всей криптографии с открытым ключом, в том числе и систем ЭП, является управление открытыми ключами. Так как открытый ключ доступен любому пользователю, то необходим механизм проверки того, что этот ключ принадлежит именно своему владельцу. Необходимо обеспечить доступ любого пользователя к подлинному открытому ключу любого другого пользователя, защитить эти ключи от подмены злоумышленником, а также организовать отзыв ключа в случае его компрометации.

Задача защиты ключей от подмены решается с помощью сертификатов. Сертификат позволяет удостоверить заключённые в нём данные о владельце и его открытый ключ подписью какого-либо доверенного лица. Существуют системы сертификатов двух типов: централизованные и децентрализованные. В децентрализованных системах путём перекрёстного подписывания сертификатов знакомых и доверенных людей каждым пользователем строится сеть доверия. В централизованных системах сертификатов используются центры сертификации, поддерживаемые доверенными организациями.

Центр сертификации формирует закрытый ключ и собственный сертификат, формирует сертификаты конечных пользователей и удостоверяет их аутентичность своей цифровой подписью. Также центр проводит отзыв истекших и компрометированных сертификатов и ведёт базы(списки) выданных и отозванных сертификатов. Обратившись в сертификационный центр, можно получить собственный сертификат открытого ключа, сертификат другого пользователя и узнать, какие ключи отозваны.

##Хранение закрытого ключa 

Закрытый ключ является наиболее уязвимым компонентом всей криптосистемы цифровой подписи. Злоумышленник, укравший закрытый ключ пользователя, может создать действительную цифровую подпись любого электронного документа от лица этого пользователя. Поэтому особое внимание нужно уделять способу хранения закрытого ключа. Пользователь может хранить закрытый ключ на своем персональном компьютере, защитив его с помощью пароля. Однако такой способ хранения имеет ряд недостатков, в частности, защищённость ключа полностью зависит от защищённости компьютера, и пользователь может подписывать документы только на этом компьютере.

В настоящее время существуют следующие устройства хранения закрытого ключа:

Дискеты

Смарт-карты

USB-брелоки

Таблетки Touch-Memory

реестр (в защищённой памяти компьютера)

Кража или потеря одного из таких устройств хранения может быть легко замечена пользователем, после чего соответствующий сертификат должен/может быть немедленно отозван.

Наиболее защищённый способ хранения закрытого ключа — хранение на смарт-карте. Для того, чтобы использовать смарт-карту, пользователю необходимо не только её иметь, но и ввести PIN-код, то есть, получается двухфакторная аутентификация. После этого подписываемый документ или его хэш передаётся в карту, её процессор осуществляет подписывание хэша и передаёт подпись обратно. В процессе формирования подписи таким способом не происходит копирования закрытого ключа, поэтому все время существует только единственная копия ключа. Кроме того, произвести копирование информации со смарт-карты немного сложнее, чем с других устройств хранения.

В соответствии с законом «Об электронной подписи», ответственность за хранение закрытого ключа владелец несёт сам.
