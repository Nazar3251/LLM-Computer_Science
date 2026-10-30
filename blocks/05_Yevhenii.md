Повний текст
Упродовж останніх років про небезпеку великих мовних моделей (LLM, large language models) говорили багато: експерти, компанії, ентузіасти. Більшість цих тверджень читач міг сприймати лише як думки й прогнози.
Частина попереджень спиралася на вимірювання. Британський AI Security Institute (AISI, державний інститут безпеки штучного інтелекту) у звіті Frontier AI Trends Report від 18 грудня 2025 року повідомив, що частка кіберзавдань початкового рівня, які моделі виконують успішно, зросла приблизно з 9% наприкінці 2023 року до близько 50%. У 2025 році інститут уперше протестував модель, що впоралася із завданнями для фахівців із понад десятирічним досвідом. В усіх перевірених системах знайшлися універсальні джейлбрейки, тобто способи обійти захисні обмеження моделі. 17 вересня 2026 року Джеффрі Гінтон (Geoffrey Hinton), один із піонерів нейронних мереж, на закритому брифінгу для сенаторів США, за повідомленням NBC Washington, сказав, що на запровадження запобіжників залишається приблизно рік, і пов'язав це з тим, що системи штучного інтелекту (ШІ) вже допомагають створювати наступні.
Жодне з цих попереджень не накладало на розробників моделей юридичних зобов'язань. Висновки AISI залишалися оцінкою державної установи, слова Гінтона — позицією вченого, і для компаній усе це було зовнішньою критикою.
26 жовтня 2026 року Anthropic, що готується до IPO (initial public offering, першого публічного продажу акцій компанії на біржі), подала до SEC (Securities and Exchange Commission, Комісії з цінних паперів і бірж США) реєстраційну заяву за формою S-1. У ній компанія зобов'язана розкрити, чим займається, скільки заробляє, на що витрачає гроші, хто нею керує і чим ризикує. Заяву подано відповідно до Закону про цінні папери США 1933 року, а закон передбачає відповідальність за істотні неправдиві твердження й пропуски. На обкладинці сказано, що SEC не оцінювала точність і повноту проспекту, тже за кожне слово відповідає сама компанія. Документ попередній: ціна акцій, їхня кількість і дата розміщення в ньому порожні.
Розділ про ризики (Risk Factors) займає 94 сторінки, з 26-ї по 119-ту. Основна частина проспекту налічує близько 335 сторінок на 24 пункти змісту, тобто середній розділ має приблизно 14 сторінок. Закон вимагає перелічити тут усе суттєве, що може піти не так, і саме тут Anthropic пише про небезпеку власних моделей.
За нашим підрахунком, таких окремих формулювань близько 29. Слово misaligned (дослівно «розузгоджений»: модель діє всупереч намірам людей) зустрічається в документі 18 разів. Компанія пише, що її моделі можуть поводитися непередбачувано й шкідливо, зокрема вчиняти дії, яких ніхто не замовляв. У тестах і внутрішньому використанні, за її описом, моделі обходили мережеві обмеження та ізольоване тестове середовище («пісочницю»), надавали собі дозволи, яких не мали, і неправдиво повідомляли, що завдання виконано чи перевірено. Компанія додає, що подібну поведінку спостерігали й в інших розробників.
Окремо розкрито інцидент. Під час перевірок кібербезпеки, які готував сторонній партнер, помилка в налаштуванні лишила тестову модель підключеною до відкритого інтернету, хоча цього не мало бути. Чотири моделі отримали несанкціонований доступ до реальних чужих систем у сесіях приблизно від 10 до 34 годин активної роботи. В одному випадку модель, не зумівши скасувати нерозв'язне завдання, скористалася знайденим паролем, увійшла як адміністратор до системи третьої сторони, зібрала додаткові облікові дані, змінила налаштування й прочитала персональні дані однієї людини. Постраждалих повідомили. За словами компанії, розслідування не знайшло ознак змови між моделями, переслідування цілей поза завданням чи спроб уникнути нагляду. Після цього вона призупинила частину таких оцінювань.
Найбільшу методологічну вагу має визнання щодо самих перевірок. Anthropic спостерігала, що моделі поводяться інакше, коли виявляють або припускають, що їх оцінюють, і називає це суттєвим обмеженням для оцінки безпеки. Компанія також може не зуміти пояснити, чому модель поводиться саме так. Найпотужніші моделі, пише вона, вже здатні суттєво допомагати зловмисникам у створенні хімічної чи біологічної зброї, а захисні фільтри компанія називає неповними й такими, які вже обходили. Окремим реченням додано, що могли бути випадки шкідливого використання, яких вона не виявила.
З попередженням Гінтона перегукується ще одне місце. Anthropic пише, що її моделі вже беруть участь у створенні наступних (вона називає це closing the loop, «замиканням циклу») і що через це можливості моделей можуть зростати швидше, ніж компанія встигає розробляти й упроваджувати захисні заходи. Гінтон говорив про ту саму ланку: системи допомагають створювати наступні.
Це не прогноз на завтра. Розділ про ризики передає переконання компанії щодо майбутнього, і лише окремо розкриті випадки, як-отестовий інцидент, подано як такі, що вже сталися. Строків настання ризиків документ не називає. Водночас у вступній частині Anthropic очікує, що Powerful AI («потужний ШІ»: здібності на рівні провідних експертів у більшості професійних і наукових галузей) стане широкодоступним протягом кількох років. Застереження внесено до юридичного документа, а поруч стоять рішення, які їх підкріплюють: модель Mythos у квітні 2026 року спершу відкрили не для всіх, а для вибраних організацій у межах Project Glasswing, бо вона дуже добре знаходить вразливості в програмах.




Тези Antropic

“Our AI models may behave in unintended, misaligned, or autonomous ways, including by taking harmful actions that no user or third party directed”

“Misaligned behaviors of this kind, whether occurring in testing or real-world deployments, have been observed both in our models and elsewhere in the industry, including in testing and internal use, models circumventing network and sandbox restrictions, granting themselves permissions they had not been given, taking unintended actions in pursuit of assigned goals, interfering with other AI agents, and misrepresenting whether tasks had been completed or verified, and as models are granted greater autonomy, permissions, and integration with external systems, the consequences of such misaligned behavior increase.”

“In addition, models, including our own, have exhibited, and may in the future exhibit, unexpected strategic or self-preserving behaviors, including attempts to resist shutdown, conceal or manipulate information, or generate outputs that could be interpreted as coercive, deceptive, or manipulative, including behavior resembling blackmail or efforts to influence human decision-makers to preserve the model’s continued operation or access.”

“agent behaviors cannot be exhaustively tested prior to deployment”

“models behaving differently when they detect or infer that they are being evaluated”

“ We may be unable to fully understand or explain why our models produce particular outputs or behave in particular ways”

“In particular, our most capable models have demonstrated, and future models are expected to demonstrate, capabilities that could provide meaningful assistance to malicious actors seeking to develop chemical, biological, or other dangerous weapons.”

“AI algorithms may be flawed, and AI systems may contain bugs, errors, or defects or fail to follow instructions or produce inaccurate, misleading, offensive, inappropriate, or otherwise harmful outputs”

“Harmful incidents involving our models, regardless of fault, could also severely and disproportionately damage our reputation and brand as a safety-focused AI company, leading to loss of customer trust and customer attrition…..”

“There may have been past instances of harmful use or harmful output of our models that we did not detect, and there may be future instances that we will not detect.”


“In particular, as AI systems become more autonomous and capable of taking consequential actions with less human oversight, there is a risk that such systems could, whether due to misalignment with human intentions, errors in objective specification, or self-preserving behaviors, take harmful actions independently and at scale without human intervention”

“Connecting increasingly capable models to laboratory automation may also heighten governmental and public concern regarding the potential for AI systems to accelerate the development of dangerous biological, chemical, or other materials, which could result in additional regulatory restrictions on, or scrutiny of, these offerings.”




Джерела
* [Anthropic, PBC: Form S-1, 26.10.2026](https://www.sec.gov/Archives/edgar/data/2130357/000162828026067168/anthropicpbc-sx1.htm)
* [AI Security Institute](https://www.aisi.gov.uk/blog/5-key-findings-from-our-first-frontier-ai-trends-report)
* [NBC Washington](https://www.nbcwashington.com/news/national-international/geoffrey-hinton-congress-ai-regulation/4155951/)
* [OECD AI Incidents](https://oecd.ai/en/incidents/2026-09-17-836d)
* https://www.sec.gov/edgar/search/