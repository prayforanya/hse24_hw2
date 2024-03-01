# hse24_hw2

[Ссылка на Colab]()

Для данного домашнего задания мной был выбран эксперимент Encode с клеточной линией K562 и гистоновой меткой H3K4me3.

### Анализ FastQC 
HTML-файлы лежат в папке data
Все риды были хорошего качество, поэтому подрезать их не потребовалось 
ENCFF894KBP |	ENCFF010SAE |	ENCFF994FIB
___ | ___ | ___
![image](https://github.com/prayforanya/hse24_hw2/blob/main/data/ENCFF894KBP_scores.png) | ![image](https://github.com/prayforanya/hse24_hw2/blob/main/data/ENCFF010SAE_scores.png) | ![image](https://github.com/prayforanya/hse24_hw2/blob/main/data/ENCFF994FIB_scores.png) 
![image](https://github.com/prayforanya/hse24_hw2/blob/main/data/ENCFF894KBP_quality.png) | ![image](https://github.com/prayforanya/hse24_hw2/blob/main/data/ENCFF010SAE_quality.png) | ![image](https://github.com/prayforanya/hse24_hw2/blob/main/data/ENCFF994FIB_quality.png) 

### Таблица со статистикой по каждому из 3 образцов

index | Количество ридов | Выравнилось уникально | (%) | Выравнилось неуникально | (%) | Не выравнилось | (%)
--- | --- | --- | --- | --- | --- | --- | ---
ENCFF894KBP | 38184025 | 1247987 | 3.27% | 3039385 | 7.96% | 33896653 | 88.77%
ENCFF010SAE | 35494854 | 1150650 | 3.24% | 2744423 | 7.73% | 31599781 | 89.03%
ENCFF994FIB | 10438657 | 390293 | 3.74% | 1335446 | 12.79% | 8712918 | 83.47%

Процент выравнивания получился таким низким, так как мы выравнивали только на одну хромосому. 

### Диаграмма Венна

Диаграммы лежат в папке data
Пересечений доволь мало, я предполагаю, что это связано с тем, что в нашем небольшом исследовании мы проводили выравнивание только на 1 хромосому.