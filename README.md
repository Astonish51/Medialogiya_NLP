## Тестовое задание по классификации текстов

### Описание задачи

Необходимо разработать классификатор каналов YouTube.  

### Набор данных

Датасет содержит 5500 размеченых ссылок на каналы и категорию (11 категорий + микс категорий).   
Данные сбалансированны.  

### Решение  

Задача представляет собой многоклассовую классификацию текстов.  
На основании предоставленных ссылок и категорий выгрузил текстовые данные последних 50 видео каналов, затем использовал их как признаки для обучения моделей.
В качестве решения используется предсказаний Logistic Regression с TF-IDF
Задание выполнено на языке Python.  
В качестве метрика используется f1-macro, т.к. в задании не было указания, какую использовать.  
Решение в файле **Medialogia_models.ipynb**
Выгрузка данных по API в файле **Medialogiya_data_youtube.ipynb**

### Требование к оборудованию

Для воспроизведения результатов приведенных в ноутбуке может потребоваться CPU.
Других специфичных требований к ПК нет.  

### Используемые библиотеки

Cписок библиотек и фреймворков, которые используются в проекте:

- PyTorch
- Scikit-learn
- NLTK
- transformers
- scipy
- pandas
- numpy

## Требования к подготовке среды

1. **Python 3.9+** : Убедитесь, что на вашем компьютере установлена версия Python 3.9+ [Официальный сайт Python](https://www.python.org/)

2. **Виртуальное окружение (рекомендуется)**: Рекомендуется создать виртуальное окружение для изоляции зависимостей.

   python -m venv venv
   source venv/bin/activate  # Для Linux / macOS  
   .\venv\Scripts\activate   # Для Windows  

   pip install -r requirements.txt  

   Для установки зависимостей в jupyter notebook используйте  
   ! pip install -r requirements.txt  
3. Импорт PyTorch (import torch) имеет ряд особенностей, лучше уточнить причину ошибок, если они возникли, на официальном сайте [Официальный сайт pytorch](https://pytorch.org/) или на [stackoverflow](https://stackoverflow.com/)

### Структура 

В папке data выгруженные данные по API плюс исходный файл.
Medialogia_models.ipynb - решение
Medialogiya_data_youtube.ipynb - выгрузка данных по API.

├── data  
|	├── channals_1000.csv  
	├── channals_2000.csv 
	├── channals_3000.csv 
	├── channals_4000.csv 
	├── channals_5000.csv 
	├── channals_5499.csv 
	├── yt_topics_10_500.xlsx
├── Medialogia_models.ipynb 
├── Medialogiya_data_youtube.ipynb
├── README.md  
├── requirements.txt  


