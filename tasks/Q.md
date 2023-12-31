# Вопросы

### Часть 1.

1. Python. Система типов и базовые типы данных (str, int, float, bool, NoneType).
2. Стековая машина. Байткод интерпретатора CPython.
3. Основные контейнеры в стандартной библиотеке Python (tuple, list, set, dict). Алгоритмическая сложность базовых операций.
4. Срезы (slices) для базовых коллекций в Python. Иммутабельность и метод hash().
5. NumPy. Понятие массива - размерность, тип и внутреннее устройство. Создание массивов.
6. NumPy. Срезы. Операции над массивами. Broadcasting.
7. Pandas. Series и DataFrame - создание, устройство, понятие индекса, обращение к колонкам и строкам.
8. Pandas. Агрегирование и группировка данных. Встроенные методы визуализации данных.

### Часть 2.

1. Наивный байесовский классификатор .
2. Логистическая регрессия. 
3. Метод опорных векторов. 
4. Деревья решений.
5. Градиентный бустинг. 
6. kNN
7. Лемматитизация, стемминг, Subword Tokenization (BPE, WordPiece, ..)
8. Векторное представление текстов: ${tf-id}$, Система обозначений SMART.
9. Word embedding (word2vec, GloVe)
10. ELMo: Deep contextualized word representations
11. Модель Transformers. Разобрать архитектуру одной из моделей: BERT, GPT-2, USE.


# Примеры задач:

Задачи, в основном, связаны коллекцией новостей (https://drive.google.com/file/d/15o7fdxTgndoy6K-e7g8g1M2-bOOwqZPl/view). В каждой строке содержится метка рубрики, заголовок новостной статьи и сам текст статьи, например:

>    **sport**&nbsp;&lt;tab&gt;&nbsp;**Сборная Канады по хоккею разгромила чехов**&nbsp;&lt;tab&gt;&nbsp;**Сборная Канады по хоккею крупно об...**

где &lt;tab&gt; символ табуляции. 

1. Используя некоторые эвристические соображения извлеките список возможных фамилий, которые упоминаются в новостях.

2. Используя некоторые эвристические соображения извлеките список возможных имён, которые упоминаются в новостях.

3. Используя некоторые эвристические соображения извлеките список возможных должностей ("президент", "губернатор Приморского края"), которые упоминаются в новостях.

4. Реализуйте отображение каждой новости на 200-мерное пространство с помощью тривиального word embdedding'а . Отобразите все документы на плоскости с помощью t-SNE.

5. Реализуйте классификацию документов с помощью стандартных средств из библиотеки `scikit-learn` (${tf-id}$, какой-нибудь алгортим классификации). Проилюстрируйте пару примеров классификации с помощью [`eli5`](https://github.com/TeamHG-Memex/eli5) 

6. Реализуйте классификацию документов с помощью стандартных средств из библиотеки `scikit-learn` и простого word embedding'а. Проилюстрируйте пару примеров классификации с помощью [`eli5`](https://github.com/TeamHG-Memex/eli5) 

7. Напишите консольную программу поиска похожих новостей. Пользователь вводит текст, ему выдается список наиболее близких новостей. Используйте $\mathbb{tf-id}$.

8. Напишите консольную программу поиска похожих новостей. Пользователь вводит текст, ему выдается список наиболее близких новостей. Используйте тривиальный word embedding.

9. Скачайте корпус [коротких твиттов](https://study.mokoron.com/). Скачайте [файл со словами](http://opencorpora.org/files/export/ngrams/unigrams.cyr.lc.zip). Найдите в корпусе список 100 самых частотных слов, в которых делают опечатки, считая что во втором файле список корректных слов.  