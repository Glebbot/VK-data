# VK-data
Анализ данных архива ВК с кластеризацией сообщений

## Инструкция по применению:
Разместите папку проекта в директории с архивом VK (на одном уровне с файлом index.html).<br>
Блокнот Vkdata.ipynb должен находиться в собственной директории (например, archive/vkdata/VKdata.ipynb где archive - директория архива VK
<br>
## Настройки анализа
<br>
Имя пользователя или название беседы<br>
- NAME
<br><br>
Используемая модель (DBSCAN, Spectral или KMeans)<br>
При некорректном имени по умолчанию будет использован KMeans<br>
- MODEL_TYPE
<br><br>
Максимальное количество кластеров (для KMeans)<br>
- MAX_CLUSTERS
<br><br>
eta для DBSCAN<br>
- ETA
<br><br>
Использовать PCA перед кластеризацией (True или False)<br>
- USE_PCA
<br><br>
Минимальный порог для TF-IDF<br>
- MIN_DF
<br><br>
Количество точек для визуализации PCA<br>
- POINT_COUNT
<br><br>
Сохранять информацию в csv файле после парсинга (True или False)<br>
Если False, при каждом новом запуске программы будет осуществляться повторный парсинг, что может занимать много времени<br>
- SAVE_TO_CSV
<br><br>
Чтение информации из csv файла (True или False)<br>
Если False, существующие csv файлы будут проигнорированы и перезаписаны (если SAVE_TO_CSV = True). Используйте если обновили данные архива<br>
- READ_FROM_CSV
<br><br>
Количество компонент для PCA (график будет выведен только для 2 или 3 компонент)<br>
- PCA_COMPONENTS
<br><br>
Использовать ли эмбеддинги BERT вместо TF-IDF векторизации (True или False)<br>
- USE_BERT
<br><br>
Директория с моделями hugging face (если None, то будет использована директория по умолчанию)<br>
- USE_BERT
