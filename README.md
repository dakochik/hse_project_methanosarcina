# Проект
В репозитории содержатся следующие директории:
* `data` - геномы 5 выбранных организмов
* `predictions` - предсказания участков Z-DNA для 5 выбранных геномов. Формат файлов: 1 столбец - начало участка, 2 - конец, 3 - zh-score; столбцы разделяются табуляцией  
  
[Ссылка](https://www.meme-arsenal.com/memes/fae5e7084042aa90eb6e86ae3590c9c1.jpg) на ноутбук с кодом
## 1. Таблица аннотированных генов
|Название организма             |Кол-во генов |Процент генов в геноме |Кол-во участков Z-ДНК* |Общая длина участков Z-ДНК*  |
|:-----------------------------:|:-----------:|:---------------------:|:---------------------:|:---------------------------:|
|Methanosarcina mazei Go1       |3417         |74.78                  |1848                   |18642                        |
|Methanosarcina thermophila TM-1|2741         |74.88                  |1191                   |11872                        |
|Methanosarcina vacuolata Z-761 |3632         |70.56                  |1610                   |16364                        |
|Methanosarcina flavescens      |2822         |74.58                  |1407                   |14016                        |
|Methanosarcina lacustris Z-7289|3339         |71.17                  |1544                   |15588                        |
  
*- участков Z-ДНК с zh-score > 500
## 2. Распределение участнов Z-ДНК
Распределение Z-ДНК по промоторам, гену и межгенному пространству:  
![image](https://user-images.githubusercontent.com/55440084/171504166-46885ae6-55cb-449a-bb5c-8168cdab35b8.png)

 
## 3. Гистограмма значений zh-score 
Попытка отобразить распредление значений zh-score по всему геному. Зеленым обозначены участки Z-DNA, размер столбца описывает величину zh-score. Красным - аннотированные гены.  
GCF_001304615 2_ASM130461v2:  
![GCF_001304615 2_ASM130461v2_genomic](https://user-images.githubusercontent.com/55440084/170326236-eb3bc7b0-ea4b-40aa-9916-57aa10b16d19.png)  
  
GCF_000970265 1_ASM97026v1:  
![GCF_000970265 1_ASM97026v1_genomic](https://user-images.githubusercontent.com/55440084/170326262-c197fc8c-1e7f-4486-aa97-0ef4adf9f9f7.png) 
  
CF_000969905 1_ASM96990v1:  
![GCF_000969905 1_ASM96990v1_genomic](https://user-images.githubusercontent.com/55440084/170326268-54d25147-87c7-4758-b8f5-f52ef49da1c9.png)  
  
GCF_000969885 1_ASM96988v1:  
![GCF_000969885 1_ASM96988v1_genomic](https://user-images.githubusercontent.com/55440084/170326454-b027b359-eaae-4eed-b13e-e352d85f6298.png)  
  
GCF_000007065 1_ASM706v1:  
![GCF_000007065 1_ASM706v1_genomic](https://user-images.githubusercontent.com/55440084/170326465-11b20abb-b9a9-4803-bdb0-03779c7808b6.png)  
  
## 4. Z-ДНК и гомологичные гены разных организмов
Для демонстрации было выбрано 8 кластеров. В некоторых из них во всех гомологичных белках сохраняются участки Z-ДНК, в некоторых - нет (такие кластеры были выбраны специально для иллюстрации). Порядок орагнизмов соответсвует порядку в приведенной ранее таблице (см. п. 1).  
![image](https://user-images.githubusercontent.com/55440084/172065655-85332378-cf7a-408f-b83c-c658056cbc7f.png)
![image](https://user-images.githubusercontent.com/55440084/172065671-5a5df8b1-12e2-4191-ac9b-21b34b790145.png)
![image](https://user-images.githubusercontent.com/55440084/172065683-626d00af-8a21-4487-920f-7bfbc017fda2.png)
![image](https://user-images.githubusercontent.com/55440084/172065691-d4949f77-fbb2-495f-98c9-cecee9bca7be.png)
![image](https://user-images.githubusercontent.com/55440084/172065697-7381de26-8fdd-484f-8389-e918dda58cee.png)
![image](https://user-images.githubusercontent.com/55440084/172065704-12bb725b-974e-4260-9549-c10c93476efa.png)
![image](https://user-images.githubusercontent.com/55440084/172065718-583bb523-0d86-415b-8b76-94f70ba19acb.png)
![image](https://user-images.githubusercontent.com/55440084/172065740-1adb1176-d796-4d38-8a48-be2398e66fc6.png)


## 5. Предсказание G-квадруплексов
