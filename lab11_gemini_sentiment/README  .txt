Практичне заняття 11. Інтеграція Gemini API

Мета роботи:
Перевірити, як Gemini API аналізує емоційне забарвлення текстів і знайти слабкі місця ШІ.

Що було зроблено:
Я створив CSV-файл з 50 проблемними текстами.
У файлі є текст, моя інтерпретація настрою та тип проблеми.
Потім усі тексти були проаналізовані через Gemini API.
Результати Gemini були порівняні з моєю власною інтерпретацією.

Кількість текстів: 50

Типи проблемних текстів:
problem_type
mixed context         11
sarcasm               10
slang                  5
slang / ambiguity      5
context                4
contrast               3
indirect meaning       2
irony                  2
indirect criticism     2
ambiguous              2
double negative        1
weak sentiment         1
cultural/context       1
simple positive        1
Name: count, dtype: int64

Розподіл результатів Gemini:
gemini_sentiment
negative    21
positive    12
mixed       11
neutral      6
Name: count, dtype: int64

Результати аналізу:

Текст 1:
Текст: Great, my laptop crashed again right before the deadline. Amazing day.
Тип проблеми: sarcasm
Моя інтерпретація: negative
Результат Gemini: negative
Пояснення Gemini: The positive words 'Great' and 'Amazing' are used sarcastically to express frustration about a laptop crash.
Можлива причина помилки: AI may interpret 'Great' and 'Amazing day' literally as positive indicators, missing the sarcastic tone.

Текст 2:
Текст: Thanks for ignoring my message for three days, very professional.
Тип проблеми: sarcasm
Моя інтерпретація: negative
Результат Gemini: negative
Пояснення Gemini: The 'thanks' and 'very professional' are clearly sarcastic, indicating annoyance at being ignored.
Можлива причина помилки: AI might identify 'thanks' and 'professional' as positive words and miss the sarcastic intent.

Текст 3:
Текст: Wow, waiting one hour for coffee is exactly what I needed.
Тип проблеми: sarcasm
Моя інтерпретація: negative
Результат Gemini: negative
Пояснення Gemini: The 'Wow' and 'exactly what I needed' are used sarcastically to express impatience and dissatisfaction.
Можлива причина помилки: AI might perceive 'Wow' and 'exactly what I needed' as positive affirmations, overlooking the sarcastic context of a long wait.

Текст 4:
Текст: Perfect, the delivery came late and the box was broken.
Тип проблеми: sarcasm
Моя інтерпретація: negative
Результат Gemini: negative
Пояснення Gemini: 'Perfect' is used sarcastically to express extreme dissatisfaction with a late and damaged delivery.
Можлива причина помилки: AI may take 'Perfect' at face value, failing to recognize its sarcastic use in conjunction with negative events.

Текст 5:
Текст: I just love when apps delete my work without saving.
Тип проблеми: sarcasm
Моя інтерпретація: negative
Результат Gemini: negative
Пояснення Gemini: The statement 'I just love' is sarcastic, conveying strong annoyance about an app malfunction.
Можлива причина помилки: AI might detect 'love' as a strong positive keyword and misinterpret the sarcastic expression.

Текст 6:
Текст: Nice job, the update made everything slower.
Тип проблеми: sarcasm
Моя інтерпретація: negative
Результат Gemini: negative
Пояснення Gemini: 'Nice job' is sarcastically applied to a negative outcome where an update worsened performance.
Можлива причина помилки: AI could focus on 'Nice job' as a positive phrase, missing the ironic criticism of the update's effect.

Текст 7:
Текст: Amazing service: nobody answered my call for 20 minutes.
Тип проблеми: sarcasm
Моя інтерпретація: negative
Результат Gemini: negative
Пояснення Gemini: 'Amazing service' is used sarcastically to highlight extremely poor customer service.
Можлива причина помилки: AI might incorrectly classify 'Amazing service' as positive without understanding the contradictory negative context.

Текст 8:
Текст: Fantastic, my order was wrong again.
Тип проблеми: sarcasm
Моя інтерпретація: negative
Результат Gemini: negative
Пояснення Gemini: 'Fantastic' is used sarcastically to express frustration over a repeated mistake with an order.
Можлива причина помилки: AI might interpret 'Fantastic' as a genuine positive emotion, overlooking the negative event it describes.

Текст 9:
Текст: What a wonderful surprise, another hidden fee.
Тип проблеми: sarcasm
Моя інтерпретація: negative
Результат Gemini: negative
Пояснення Gemini: 'Wonderful surprise' is sarcastically used to convey displeasure about an unexpected additional charge.
Можлива причина помилки: AI could misinterpret 'wonderful surprise' as genuinely positive, failing to detect the sarcasm regarding the hidden fee.

Текст 10:
Текст: Best experience ever: I paid more and got less.
Тип проблеми: sarcasm
Моя інтерпретація: negative
Результат Gemini: negative
Пояснення Gemini: 'Best experience ever' is sarcastically stated to express dissatisfaction with receiving less value for more money.
Можлива причина помилки: AI might prioritize 'Best experience ever' as a strong positive indicator, missing the sarcastic intent from the outcome.

Текст 11:
Текст: The food was cold, but at least the waiter was polite.
Тип проблеми: mixed context
Моя інтерпретація: mixed
Результат Gemini: mixed
Пояснення Gemini: The sentiment is mixed due to negative feedback about cold food and positive feedback about the polite waiter.
Можлива причина помилки: AI might lean towards either positive or negative if it gives more weight to one aspect over the other.

Текст 12:
Текст: The hotel room was small, but the view was beautiful.
Тип проблеми: mixed context
Моя інтерпретація: mixed
Результат Gemini: mixed
Пояснення Gemini: The text presents a negative aspect (small room) alongside a positive one (beautiful view).
Можлива причина помилки: AI could potentially categorize it as predominantly negative because 'small' might be a stronger descriptor than 'beautiful' depending on its training.

Текст 13:
Текст: The product works, but I expected much more for this price.
Тип проблеми: mixed context
Моя інтерпретація: mixed
Результат Gemini: mixed
Пояснення Gemini: It acknowledges the product's functionality but expresses disappointment regarding its value for the price.
Можлива причина помилки: AI might focus on 'product works' as positive or 'expected much more' as negative, missing the balance.

Текст 14:
Текст: The delivery was fast, but the package was damaged.
Тип проблеми: mixed context
Моя інтерпретація: mixed
Результат Gemini: mixed
Пояснення Gemini: The text includes a positive comment about fast delivery and a negative one about a damaged package.
Можлива причина помилки: AI might struggle to weigh the 'fast delivery' against 'damaged package' and classify it as purely positive or negative.

Текст 15:
Текст: The movie looked great, but the story was boring.
Тип проблеми: mixed context
Моя інтерпретація: mixed
Результат Gemini: mixed
Пояснення Gemini: There's a positive remark about the visuals and a negative one about the plot.
Можлива причина помилки: AI might incorrectly classify it as purely positive or negative by prioritizing one phrase over the other.

Текст 16:
Текст: The phone camera is good, but the battery is terrible.
Тип проблеми: mixed context
Моя інтерпретація: mixed
Результат Gemini: mixed
Пояснення Gemini: It contains a positive attribute (good camera) and a strongly negative one (terrible battery).
Можлива причина помилки: AI could easily swing to either positive (camera is good) or negative (battery is terrible) due to strong contrasting terms.

Текст 17:
Текст: The restaurant is clean, but the portions are too small.
Тип проблеми: mixed context
Моя інтерпретація: mixed
Результат Gemini: mixed
Пояснення Gemini: The text provides positive feedback on cleanliness but negative feedback on portion size.
Можлива причина помилки: AI might misinterpret the overall sentiment as negative if it weights 'too small' heavily, or neutral if it balances them without recognizing the direct positive.

Текст 18:
Текст: The app has many functions, but it is hard to understand.
Тип проблеми: mixed context
Моя інтерпретація: mixed
Результат Gemini: mixed
Пояснення Gemini: There's a positive aspect (many functions) counterbalanced by a negative one (difficulty in understanding).
Можлива причина помилки: AI might interpret 'many functions' as overwhelmingly positive, or 'hard to understand' as overwhelmingly negative.

Текст 19:
Текст: The teacher explained well, but the task was still confusing.
Тип проблеми: mixed context
Моя інтерпретація: mixed
Результат Gemini: mixed
Пояснення Gemini: The explanation was positive, but the task itself remained a negative experience.
Можлива причина помилки: AI might lean towards positive due to 'explained well' or negative due to 'confusing' without fully capturing the mixed sentiment.

Текст 20:
Текст: The coffee tasted nice, but it was almost cold.
Тип проблеми: mixed context
Моя інтерпретація: mixed
Результат Gemini: mixed
Пояснення Gemini: It praises the taste of the coffee but notes the negative temperature.
Можлива причина помилки: AI might classify this as positive because 'tasted nice' is a direct positive, potentially underplaying 'almost cold.'

Текст 21:
Текст: This movie was sick, I really loved it.
Тип проблеми: slang
Моя інтерпретація: positive
Результат Gemini: positive
Пояснення Gemini: 'Sick' is used here as slang to mean excellent, reinforced by 'I really loved it.'
Можлива причина помилки: AI might mistakenly interpret 'sick' in its literal, negative health context, ignoring the reinforcing positive phrase.

Текст 22:
Текст: That game was crazy good.
Тип проблеми: slang
Моя інтерпретація: positive
Результат Gemini: positive
Пояснення Gemini: 'Crazy good' is an intensifier meaning exceptionally good.
Можлива причина помилки: AI could potentially misinterpret 'crazy' as a negative descriptor if not trained on its slang usage.

Текст 23:
Текст: The concert was fire.
Тип проблеми: slang
Моя інтерпретація: positive
Результат Gemini: positive
Пояснення Gemini: 'Fire' is used as modern slang to denote something excellent or impressive.
Можлива причина помилки: AI might struggle with 'fire' as a positive slang term, potentially interpreting it literally or neutrally.

Текст 24:
Текст: This burger is bad, in a good way.
Тип проблеми: slang / ambiguity
Моя інтерпретація: positive
Результат Gemini: positive
Пояснення Gemini: The phrase explicitly clarifies that 'bad' is used as slang for good.
Можлива причина помилки: AI might get confused by the direct contradiction and either overemphasize 'bad' or struggle to resolve the paradoxical phrasing.

Текст 25:
Текст: The new design slaps.
Тип проблеми: slang
Моя інтерпретація: positive
Результат Gemini: positive
Пояснення Gemini: 'Slaps' is current slang used to mean something is excellent or highly enjoyable.
Можлива причина помилки: AI might not recognize 'slaps' as a positive slang term, potentially misinterpreting it as neutral or even negative if taken literally.

Текст 26:
Текст: That was a killer performance.
Тип проблеми: slang / ambiguity
Моя інтерпретація: positive
Результат Gemini: positive
Пояснення Gemini: 'Killer' is used here as slang to mean outstanding or exceptionally good.
Можлива причина помилки: AI could mistakenly interpret 'killer' in its literal, negative context of harm or danger.

Текст 27:
Текст: The song is insane, I have played it ten times.
Тип проблеми: slang
Моя інтерпретація: positive
Результат Gemini: positive
Пояснення Gemini: 'Insane' is used as an intensifier for something incredibly good or impressive, indicated by the repeated listening.
Можлива причина помилки: AI might interpret 'insane' in its literal, negative sense of madness or irrationality, despite the positive context.

Текст 28:
Текст: This laptop is a beast.
Тип проблеми: slang / ambiguity
Моя інтерпретація: positive
Результат Gemini: positive
Пояснення Gemini: 'Beast' is used metaphorically to describe something powerful or impressive.
Можлива причина помилки: AI might struggle to understand 'beast' as a compliment, potentially assigning it a neutral or even negative connotation.

Текст 29:
Текст: The joke was dead funny.
Тип проблеми: slang / ambiguity
Моя інтерпретація: positive
Результат Gemini: positive
Пояснення Gemini: 'Dead funny' is an intensifier meaning extremely funny.
Можлива причина помилки: AI might literally interpret 'dead' as negative, overlooking its use as an intensifier for 'funny.'

Текст 30:
Текст: The outfit is clean.
Тип проблеми: slang / ambiguity
Моя інтерпретація: positive
Результат Gemini: positive
Пояснення Gemini: 'Clean' is used as slang to describe an outfit that is stylish and impressive.
Можлива причина помилки: AI might interpret 'clean' literally as simply not dirty, missing its slang meaning of being stylish or perfect.

Текст 31:
Текст: I am not saying the service was bad, but I would not come back.
Тип проблеми: indirect meaning
Моя інтерпретація: negative
Результат Gemini: negative
Пояснення Gemini: The direct statement about not returning strongly implies a negative experience with the service, despite the initial denial.
Можлива причина помилки: AI might overemphasize the explicit 'not saying the service was bad,' leading to a neutral or even mixed classification, missing the strong implied negativity.

Текст 32:
Текст: It could have been worse.
Тип проблеми: indirect meaning
Моя інтерпретація: neutral
Результат Gemini: neutral
Пояснення Gemini: This phrase suggests that while it wasn't good, it wasn't the worst possible outcome either, placing it in a neutral zone.
Можлива причина помилки: AI might detect 'worse' and lean towards a negative sentiment, or misinterpret it as mildly positive (implying relief it wasn't worse).

Текст 33:
Текст: I expected nothing and still felt disappointed.
Тип проблеми: irony
Моя інтерпретація: negative
Результат Gemini: negative
Пояснення Gemini: The ultimate feeling of disappointment clearly indicates a negative sentiment, regardless of initial expectations.
Можлива причина помилки: AI might struggle with the double negative implication of 'expected nothing' and the contrast with 'disappointed,' potentially classifying it as neutral or mixed.

Текст 34:
Текст: The restaurant is popular, but I do not understand why.
Тип проблеми: indirect criticism
Моя інтерпретація: negative
Результат Gemini: negative
Пояснення Gemini: Despite its popularity, the speaker's confusion implies dissatisfaction or a negative view of the restaurant's quality.
Можлива причина помилки: AI might identify 'popular' as a positive term and struggle to interpret the implied criticism.

Текст 35:
Текст: The product is not completely useless.
Тип проблеми: double negative
Моя інтерпретація: neutral
Результат Gemini: neutral
Пояснення Gemini: This double negative implies it has some use, but is far from being good, settling on a very weak, reluctant positive or neutral.
Можлива причина помилки: AI might struggle with the double negative construction, potentially misinterpreting it as negative ('useless') or even strongly positive ('not useless' = useful).

Текст 36:
Текст: I do not hate it, but I also do not like it.
Тип проблеми: ambiguous
Моя інтерпретація: neutral
Результат Gemini: neutral
Пояснення Gemini: The statement explicitly expresses a lack of strong positive or negative feelings, resulting in a neutral sentiment.
Можлива причина помилки: AI might struggle to combine the two negative statements ('do not hate,' 'do not like') and could potentially classify it as mixed or slightly negative/positive.

Текст 37:
Текст: The update fixed one problem and created three new ones.
Тип проблеми: contrast
Моя інтерпретація: negative
Результат Gemini: negative
Пояснення Gemini: Despite fixing one issue, the creation of multiple new problems results in an overall negative outcome.
Можлива причина помилки: AI might identify 'fixed one problem' as a positive, potentially leading to a mixed classification, without weighing the greater negative impact.

Текст 38:
Текст: I guess it is okay if you have no other choice.
Тип проблеми: indirect criticism
Моя інтерпретація: negative
Результат Gemini: negative
Пояснення Gemini: The conditional 'if you have no other choice' implies that it is barely acceptable and not truly good.
Можлива причина помилки: AI might focus on 'it is okay' as a neutral or slightly positive phrase, missing the strongly implied negative context.

Текст 39:
Текст: The service was acceptable, nothing more.
Тип проблеми: weak sentiment
Моя інтерпретація: neutral
Результат Gemini: neutral
Пояснення Gemini: 'Acceptable' suggests adequacy without enthusiasm, and 'nothing more' confirms a lack of positive sentiment.
Можлива причина помилки: AI might classify 'acceptable' as a mild positive, failing to account for the dampening effect of 'nothing more.'

Текст 40:
Текст: I smiled because otherwise I would cry.
Тип проблеми: irony
Моя інтерпретація: negative
Результат Gemini: negative
Пояснення Gemini: The reason for smiling is to avoid crying, clearly indicating an underlying negative emotional state.
Можлива причина помилки: AI might detect 'smiled' and mistakenly classify the sentiment as positive, missing the strong negative implication.

Текст 41:
Текст: For the price, I expected better quality.
Тип проблеми: context
Моя інтерпретація: negative
Результат Gemini: negative
Пояснення Gemini: The expectation of better quality for the given price implies dissatisfaction with the current quality.
Можлива причина помилки: AI might not fully grasp the implicit negative comparison and could classify it as neutral without enough explicit negative terms.

Текст 42:
Текст: It is cheap, so I cannot complain too much.
Тип проблеми: context
Моя інтерпретація: neutral
Результат Gemini: neutral
Пояснення Gemini: The text balances the negative implication of 'cheap' (often associated with low quality) with the positive lack of complaint, resulting in neutrality.
Можлива причина помилки: AI might interpret 'cheap' as a negative attribute or 'cannot complain too much' as a reluctant positive, potentially leading to mixed or slightly negative/positive.

Текст 43:
Текст: The food reminds me of school cafeteria lunches.
Тип проблеми: cultural/context
Моя інтерпретація: negative
Результат Gemini: negative
Пояснення Gemini: This statement relies on a common cultural negative association with school cafeteria food.
Можлива причина помилки: AI might not possess the cultural context to understand 'school cafeteria lunches' as a negative descriptor for food quality.

Текст 44:
Текст: My grandma would probably like this design, but I do not.
Тип проблеми: context
Моя інтерпретація: negative
Результат Gemini: negative
Пояснення Gemini: Despite a hypothetical positive from grandma, the speaker explicitly states their own dislike for the design.
Можлива причина помилки: AI might misinterpret the 'grandma would like' as a partial positive, leading to a mixed sentiment, rather than focusing on the speaker's direct negative.

Текст 45:
Текст: The interface is simple, maybe too simple.
Тип проблеми: ambiguous
Моя інтерпретація: neutral
Результат Gemini: neutral
Пояснення Gemini: While 'simple' can be positive, the addition of 'maybe too simple' suggests it crosses into a negative or undesirable territory, creating a neutral overall impression.
Можлива причина помилки: AI might classify 'simple' as purely positive, missing the nuanced negative implication of 'too simple.'

Текст 46:
Текст: The battery lasts forever, but the phone feels heavy.
Тип проблеми: mixed context
Моя інтерпретація: mixed
Результат Gemini: mixed
Пояснення Gemini: It highlights a significant positive feature (battery life) alongside a noticeable negative one (weight).
Можлива причина помилки: AI might focus on the strong positive 'lasts forever' or the negative 'feels heavy,' potentially misclassifying the overall mixed sentiment.

Текст 47:
Текст: I waited only ten minutes, which is actually good for this place.
Тип проблеми: context
Моя інтерпретація: positive
Результат Gemini: positive
Пояснення Gemini: The context clarifies that a ten-minute wait, while potentially long elsewhere, is considered good for this specific place.
Можлива причина помилки: AI might consider 'waited ten minutes' as a neutral or slightly negative fact, without understanding the comparative positive context.

Текст 48:
Текст: The room was quiet, which was the only good thing.
Тип проблеми: contrast
Моя інтерпретація: negative
Результат Gemini: negative
Пояснення Gemini: The explicit statement 'only good thing' implies that all other aspects of the experience were negative.
Можлива причина помилки: AI might identify 'quiet' and 'good thing' as positive indicators and miss the strong negative implication that everything else was bad.

Текст 49:
Текст: I bought it because everyone recommended it, but now I regret it.
Тип проблеми: contrast
Моя інтерпретація: negative
Результат Gemini: negative
Пояснення Gemini: Despite the initial positive influence of recommendations, the ultimate feeling of regret indicates a negative sentiment.
Можлива причина помилки: AI might be confused by the initial positive 'recommended' and struggle to reconcile it with the strong negative 'regret.'

Текст 50:
Текст: The support team answered quickly and solved the issue.
Тип проблеми: simple positive
Моя інтерпретація: positive
Результат Gemini: positive
Пояснення Gemini: The prompt response and effective resolution of a problem are clearly positive indicators of good service.
Можлива причина помилки: This is a straightforward positive case, so an error is less likely, but AI could potentially misinterpret 'solved the issue' as merely a neutral outcome.

Аналіз помилок:
Найбільші труднощі для ШІ можуть викликати сарказм, іронія, сленг, непрямий зміст та змішані відгуки.
У сарказмі слова часто звучать позитивно, але реальний зміст негативний.
У змішаних текстах є і позитивні, і негативні частини, тому моделі важче вибрати один настрій.
Сленг також може бути проблемою, бо деякі слова мають не буквальне значення.

Висновок:
Gemini API добре працює з простими текстами, але може помилятися на складних прикладах. Особливо важкими є тексти із сарказмом, іронією, культурним контекстом, сленгом і неоднозначністю. Щоб покращити результат, можна давати моделі більше контексту, просити пояснення відповіді або порівнювати результат з іншими моделями.
