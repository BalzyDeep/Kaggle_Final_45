Задача: использовать обучающую выборку для создания модели, которая даст наилучшие предсказания.

Для оценки используется метрика MAPE (https://en.wikipedia.org/wiki/Mean_absolute_percentage_error) - средняя абсолютная ошибка в процентах.

Данные для конкурса:


train.csv - данные для обучения

test.csv - тест и валидация, данные из этого файла используются для сабмита

sample_submission.csv - пример формата файла предсказаний (поля: id, score)


Колонки
Будем предсказывать оценку отелю по отзывам.

Hotel_Address - Адрес отеля, object

Review_Date - Дата публикации отзыва, object

Average_Score - Средяя оценка отеля, расчитанная на основе комментарияев за последний год, float64

Hotel_Name - Название отеля, object

Reviewer_Nationality - Национальность рецензента, object

Negative_Review - Отрицательный отзыв, оставленный рецензентом отелю. В случае отсутствия заполняется значением "No Negative", object

Review_Total_Negative_Word_Counts - Количество слов в отрицательном отзыве, int64

Positive_Review - Положительный отзыв, оставленный рецензентом отелю. В случае отсутствия заполняется значением "No Positive", object

Review_Total_Positive_Word_Counts - Количество слов в положительном отзыве, int64

Total_Number_of_Reviews_Reviewer_Has_Given - Количество отзывов, написанных рецензентом в прошлом, int64

Total_Number_of_Reviews - Количество отзывов об отеле, int64

Tags - Теги, данные рецензентом отелю, object

days_since_review - Количество дней между написанием отзыва и чисткой, int64

Additional_number_of_soring - Средний балл отеля, на основе всех оценок - с тектом отзыва и без, int64

lat - Широта отеля, float64

lng - Протяженность отеля, float64

Reviewer_Score - Оценка, данная рецензентом отелю, float64. Целевая переменная
