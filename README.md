# hse_hw1_meth

 Сcылки на collab:
 
1) https://colab.research.google.com/drive/1EAQ--U6d-vnOH-hS-Qp4WENh4_HRfhNd#scrollTo=7f_1-58NuqHN
 
2) https://colab.research.google.com/drive/1SzB-IGd4unkwrRR0RrA1EVTIPSS2X35Z?usp=sharing
 
# 1.Анализ QC прочтений

<img width="544" alt="image" src="https://user-images.githubusercontent.com/93148512/154522657-a8164b40-9f0d-49f1-8db1-6621992ccc7b.png">

<img width="852" alt="image" src="https://user-images.githubusercontent.com/93148512/154522748-343983aa-74c9-4b0d-9dc0-3c830efcc54c.png">

Мной был выбран образец из стадии 8 клеток, для которого предположительно увеличивается уровень метеллирования. На графике видно, что это действительно так и наблюдается значительное преобладание GC нуклеотидов в сравнении с остальными (per sequence GC content). Происходит это потому, что метилированные цитозины остаются неизменными, в то время как неметилированные цитозины при данном секвенировании превращаются в урацилы, которые комплементарны тиминам.

# 2. Работа с 3 образцами
 # а)Работа с bam-files с выравниваниями BS-seq ридов на 11-ю хромосому мыши
<img width="535" alt="image" src="https://user-images.githubusercontent.com/93148512/154526314-1bdd033d-7820-4b06-8b29-15d18ad84fdf.png">

 # b)Дедупликация
 
 <img width="411" alt="image" src="https://user-images.githubusercontent.com/93148512/154526647-2e5ca26b-c772-47a8-9064-f3481cfed61f.png">
 
*bash-скрипт:

<img width="981" alt="image" src="https://user-images.githubusercontent.com/93148512/154527077-2c680a5a-14de-49a0-a5b2-ff1ebd06ed5c.png">
 
 # с)Метелирование цитозинов проведено
 
 # d)Описание M-bias plot
 
 В отчётах приведены графики с долей метилирования на хромосоме. Большая доля метилирования наблюдается на образце Epiblast (77-78%), затем образец 8_cell (42-45%), а самая маленькая у образца icm (22-24%)

Epiblast:

<img width="1185" alt="image" src="https://user-images.githubusercontent.com/93148512/154532230-8b76fe45-08db-467e-9d0d-a15620ad28bc.png">

<img width="1203" alt="image" src="https://user-images.githubusercontent.com/93148512/154532320-2bc6c8a0-2078-4626-9084-a1b916854be3.png">

8_cell:

<img width="1257" alt="image" src="https://user-images.githubusercontent.com/93148512/154532407-03489e7f-6be1-48ad-b747-8d40dd80e6e3.png">

<img width="1222" alt="image" src="https://user-images.githubusercontent.com/93148512/154532476-2dfd3365-761e-4e29-ac9c-74d5d97e6fca.png">

ICM:

<img width="1224" alt="image" src="https://user-images.githubusercontent.com/93148512/154532559-8dd6137c-e328-46bc-a1bf-51dcd66dc148.png">

<img width="1248" alt="image" src="https://user-images.githubusercontent.com/93148512/154532632-c422e272-6adb-41f0-acec-7742757d91d7.png">

# e)Гистограмма распределения метилирования цитозинов по хромосоме 

![image](https://user-images.githubusercontent.com/93148512/154533342-8a7ed6d1-6c9b-4020-8141-6456272cec35.png)

![image](https://user-images.githubusercontent.com/93148512/154533400-8b5cdeeb-fee1-40a7-ad24-96c54f0be570.png)

![image](https://user-images.githubusercontent.com/93148512/154533468-5f7aaf99-0270-45ae-b0bd-07ddcf33266a.png)

Максимальный уровень метилирования ДНК наблюдается для образца Epiblast, для 8_cell метилирование небольшое, а для ICM его практически нет. Соответсвенно, можно предположить, что уровень метилирования может меняться на разных этапах развития эмбриона. Пример скрипта для построения графиков приведён в ноутбуке

# f) Уровень метилирования и покрытия
Покрытие:

![cov](https://user-images.githubusercontent.com/93148512/154534407-4ca87633-f67f-45d5-a01e-360da22a78d5.png)

Метилирование:
![meth](https://user-images.githubusercontent.com/93148512/154534429-908f40e0-9a83-4a46-aa24-10b8dd3fac15.png)



