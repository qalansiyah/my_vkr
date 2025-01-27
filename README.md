# Composition material 

<h1><strong>Прогнозирование конечных свойств композиционных материалов</strong></h1>

***
<p>В данной работе:
<ul type='circle'>
  <li>Изучены теоретические основы и методы решения поставленной задачи.</li>
  <li>Проведен разведочный анализ предложенных данных. Нарисованы гистограммы распределения каждой из переменной, диаграммы ящика с усами, попарные графики   рассеяния точек. Для каждой колонки получены среднее, медианное значение, проведен анализ и исключение выбросов, проверено наличие пропусков.</li>
  <li>Проведена предобработка данных (удаление шумов, добавление синтетических данных, нормализация).</li>
  <li>Обучены нескольких моделей для прогноза модуля упругости при растяжении и прочности при растяжении. При построении моделей был проведен поиск гиперпараметров моделей с помощью поиска по сетке с перекрестной проверкой.</li>
  <li>Написана нейронная сеть, которая будет рекомендовать соотношение матрица-наполнитель.</li>
  <li>Разработано веб-приложение с графическим интерфейсом на Flask, которое выдает прогнозы модуля упругости при растяжении, прочности при растяжении, соотношение матрица-наполнитель с помощью обученной нейронной сети.</li>
  <li>Оценены точности моделей на тренировочном и тестовом датасете.</li>
  <li>Папка notebooks состоит из из 4 файлов для каждого этапа работы: В файле preprocessing.ipynb - разведочный анализ данных и предобработка,
В файле elasticity.ipynb - обучение модели для "Модуля упругости при растяжение, ГПа", В файле strenght.ipynb - обучение модели для
"Прочность при растяжении, МПа" и в файле matrix_fill.ipynb - модель для рекомендации "Соотношение матрица-наполнитель"
  <li>Создан данный репозиторий в GitHub, в котором выложены все материалы по ВКР.</li>
  <li>Веб-приложение загружена на хостинг  <a href="https://vkr-deploy.onrender.com/" target="_blank">https://vkr-deploy.onrender.com</a>
</ul>
</p>
<strong> Веб-приложение на Flask. Инструкция.</strong>
<p>В разработанном веб-приложении можно спрогнозировать с помощью обученных нейронных сетей конечные свойства композиционных материалов, такие как "Матрица-наполнитель", "Прочность при растяжении", "Модуль упругости при растяжении", на основе введенных пользователем значений.</p>
<p>Пользователь изначально попадает на главную страницу, на которой находятся описание приложения и меню выбора прогнозируемой переменной. При нажатии на кнопку прогноза необходимой переменной пользователь попадает на новую страницу. На странице прогноза выбранной переменной пользователю предлагается ввести значения параметров  необходимых для прогноза. Диапазон вводимых значений от 0 до 1,"угол нашивки" принимает значение 0 или 1. После ввода всех параметров и нажатии кнопки "Предсказать" пользователю в виде сообщения отображается прогнозное значение переменной. Также на странице прогноза выбранной переменной находятся кнопка «Обновить»  для сброса введенных значений и кнопка возврата в главное меню.</p>

                                                                                                                 
***

                                                                                         
