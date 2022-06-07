# Проект
В репозитории содержатся следующие директории:
* `data` - геномы 5 выбранных организмов
* `predictions` - предсказания участков Z-DNA для 5 выбранных геномов. Формат файлов: 1 столбец - начало участка, 2 - конец, 3 - zh-score; столбцы разделяются табуляцией  
* `alignments` - все белковые выравнивания для выбранных кластеров  
  
[Ссылка](https://www.meme-arsenal.com/memes/fae5e7084042aa90eb6e86ae3590c9c1.jpg) на ноутбук с кодом
## 1. Таблица аннотированных генов
|Название организма             |Кол-во хромосом|Длина генома|Кол-во генов |Процент генов в геноме |Кол-во участков Z-ДНК|Кол-во участков Z-ДНК* |Общая длина участков Z-ДНК*  |
|:-----------------------------:|:-------------:|:----------:|:-----------:|:---------------------:|:---------------------:|:---------------------:|:---------------------------:|
|Methanosarcina mazei Go1       |1              |4096345     |3417         |74.78                  |4096345                |1848                   |18642                        |
|Methanosarcina thermophila TM-1|1              |3127379     |2741         |74.88                  |3127379                |1191                   |11872                        |
|Methanosarcina vacuolata Z-761 |1              |4505752     |3632         |70.56                  |4563885                |1610                   |16364                        |
|Methanosarcina flavescens      |1              |3283688     |2822         |74.58                  |3283688                |1407                   |14016                        |
|Methanosarcina lacustris Z-7289|1              |4139808     |3339         |71.17                  |4139808                |1544                   |15588                        |
  
*- участков Z-ДНК с zh-score > 500
## 2. Распределение участнов Z-ДНК
Распределение Z-ДНК по промоторам, гену и межгенному пространству:  
![image](https://user-images.githubusercontent.com/55440084/172193249-580876b0-bafd-4e14-b3f3-f6e45ca0e938.png)

 
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
### 4.1 Информация по полученным гомологичным кластерам
Всего кластеров: 3167   
  
![image](https://user-images.githubusercontent.com/55440084/172070713-3ffce547-12ff-4e6d-897d-191519a20e88.png)
  
### 4.2. Таблица с информацией по выбранным кластерам

<table>
    <thead>
        <tr>
            <th>Название кластера</th>
            <th>Кол-во генов</th>
            <th>Гены</th>
            <th>Функции генов</th>
            <th>Расположение Z-ДНК</th>
            <th>Z-Hunt score</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td rowspan=5>Cluster #1</td>
            <td rowspan=5>5</td>
            <td rowspan=1>WP_011032848.1</td>
            <td rowspan=1>Bifunctional phosphoribosylaminoimidazolecarboxamide
            formyltransferase/IMP cyclohydrolase</td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>1201</td>
        </tr>
        <tr>
            <td rowspan=1>WP_048167316.1</td>
            <td rowspan=1>Bifunctional phosphoribosylaminoimidazolecarboxamide
            formyltransferase/IMP cyclohydrolase</td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>2962</td>
        </tr>
        <tr>
            <td rowspan=1>WP_048122363.1</td>
            <td rowspan=1>bifunctional phosphoribosylaminoimidazolecarboxamide
            formyltransferase/IMP cyclohydrolase</td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>2962</td>
        </tr>
        <tr>
            <td rowspan=1>WP_048124614.1</td>
            <td rowspan=1>bifunctional phosphoribosylaminoimidazolecarboxamide
            formyltransferase/IMP cyclohydrolase</td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>2962</td>
        </tr>
        <tr>
            <td rowspan=1>WP_054299839.1</td>
            <td rowspan=1>bifunctional phosphoribosylaminoimidazolecarboxamide
            formyltransferase/IMP cyclohydrolase</td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>1201</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td rowspan=5>Cluster #2</td>
            <td rowspan=5>5</td>
            <td rowspan=1>WP_011033897.1</td>
            <td rowspan=1>PRC-barrel domain-containing protein</td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>908</td>
        </tr>
        <tr>
            <td rowspan=1>WP_048167122.1</td>
            <td rowspan=1>PRC-barrel domain-containing protein</td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>908</td>
        </tr>
        <tr>
            <td rowspan=1>WP_011306735.1</td>
            <td rowspan=1>PRC-barrel domain-containing protein</td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>908</td>
        </tr>
        <tr>
            <td rowspan=1>WP_048127780.1</td>
            <td rowspan=1>PRC-barrel domain-containing protein</td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>908</td>
        </tr>
        <tr>
            <td rowspan=1>WP_054300002.1</td>
            <td rowspan=1>PRC-barrel domain-containing protein</td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>908</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td rowspan=5>Cluster #3</td>
            <td rowspan=5>5</td>
            <td rowspan=1>WP_011032293.1</td>
            <td rowspan=1>LSm family protein</td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>883</td>
        </tr>
        <tr>
            <td rowspan=1>WP_011032293.1</td>
            <td rowspan=1>LSm family protein</td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>2943</td>
        </tr>
        <tr>
            <td rowspan=1>WP_048121098.1</td>
            <td rowspan=1>LSm family protein</td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>2943</td>
        </tr>
        <tr>
            <td rowspan=1>WP_011023130.1</td>
            <td rowspan=1>LSm family protein</td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>2943</td>
        </tr>
        <tr>
            <td rowspan=1>WP_011032293.1</td>
            <td rowspan=1>LSm family protein</td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>883</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td rowspan=5>Cluster #4</td>
            <td rowspan=5>5</td>
            <td rowspan=1>WP_011033697.1</td>
            <td rowspan=1>30S ribosomal protein S9</td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>731, 783</td>
        </tr>
        <tr>
            <td rowspan=1>WP_048167854.1</td>
            <td rowspan=1>30S ribosomal protein S9</td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>731</td>
        </tr>
        <tr>
            <td rowspan=1>WP_048117809.1</td>
            <td rowspan=1>30S ribosomal protein S9</td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>731</td>
        </tr>
        <tr>
            <td rowspan=1>WP_048124440.1</td>
            <td rowspan=1>30S ribosomal protein S9</td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>731</td>
        </tr>
        <tr>
            <td rowspan=1>WP_054297845.1</td>
            <td rowspan=1>30S ribosomal protein S9</td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>731</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td rowspan=5>Cluster #5</td>
            <td rowspan=5>5</td>
            <td rowspan=1>WP_011034015.1</td>
            <td rowspan=1>orotidine-5'-phosphate decarboxylase</td>
            <td rowspan=1>Нет</td>
            <td rowspan=1>-</td>
        </tr>
        <tr>
            <td rowspan=1>WP_048167159.1</td>
            <td rowspan=1>orotidine-5'-phosphate decarboxylase</td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>959</td>
        </tr>
        <tr>
            <td rowspan=1>WP_048118415.1</td>
            <td rowspan=1>orotidine-5'-phosphate decarboxylase</td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>4576</td>
        </tr>
        <tr>
            <td rowspan=1>WP_048127553.1</td>
            <td rowspan=1>orotidine-5'-phosphate decarboxylase</td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>959</td>
        </tr>
        <tr>
            <td rowspan=1>WP_054297609.1</td>
            <td rowspan=1>orotidine-5'-phosphate decarboxylase</td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>1122</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td rowspan=5>Cluster #6</td>
            <td rowspan=5>5</td>
            <td rowspan=1>WP_011032199.1</td>
            <td rowspan=1>riboflavin synthase</td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>883</td>
        </tr>
        <tr>
            <td rowspan=1>WP_048166057.1</td>
            <td rowspan=1>riboflavin synthase</td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>883</td>
        </tr>
        <tr>
            <td rowspan=1>WP_048119173.1</td>
            <td rowspan=1>riboflavin synthase</td>
            <td rowspan=1>Нет</td>
            <td rowspan=1>-</td>
        </tr>
        <tr>
            <td rowspan=1>WP_048126706.1</td>
            <td rowspan=1>riboflavin synthase</td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>883</td>
        </tr>
        <tr>
            <td rowspan=1>WP_054297806.1</td>
            <td rowspan=1>riboflavin synthase</td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>883</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td rowspan=5>Cluster #7</td>
            <td rowspan=5>5</td>
            <td rowspan=1>WP_011032516.1</td>
            <td rowspan=1>CRISPR-associated CARF protein Csa3</td>
            <td rowspan=1>Нет</td>
            <td rowspan=1>-</td>
        </tr>
        <tr>
            <td rowspan=1>WP_231588106.1</td>
            <td rowspan=1>CRISPR-associated CARF protein Csa3</td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>2659</td>
        </tr>
        <tr>
            <td rowspan=1>WP_048117996.1</td>
            <td rowspan=1>CRISPR-associated CARF protein Csa3</td>
            <td rowspan=1>Тело гена</td>
            <td rowspan=1>2779</td>
        </tr>
        <tr>
            <td rowspan=1>WP_048127129.1</td>
            <td rowspan=1>CRISPR-associated CARF protein Csa3</td>
            <td rowspan=1>Тело гена</td>
            <td rowspan=1>8485</td>
        </tr>
        <tr>
            <td rowspan=1>WP_054298565.1</td>
            <td rowspan=1>CRISPR-associated CARF protein Csa3</td>
            <td rowspan=1>Нет</td>
            <td rowspan=1>-</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td rowspan=5>Cluster #8</td>
            <td rowspan=5>5</td>
            <td rowspan=1>WP_011034141.1</td>
            <td rowspan=1>oligosaccharyl transferase, archaeosortase A
            system-associated</td>
            <td rowspan=1>Тело гена</td>
            <td rowspan=1>731</td>
        </tr>
        <tr>
            <td rowspan=1>WP_048168165.1</td>
            <td rowspan=1>oligosaccharyl transferase, archaeosortase A system-associated</td>
            <td rowspan=1>Тело гена</td>
            <td rowspan=1>752, 731</td>
        </tr>
        <tr>
            <td rowspan=1>WP_048124226.1</td>
            <td rowspan=1>oligosaccharyl transferase, archaeosortase A system-associated</td>
            <td rowspan=1>Тело гена</td>
            <td rowspan=1>731</td>
        </tr>
        <tr>
            <td rowspan=1>WP_232308693.1</td>
            <td rowspan=1>oligosaccharyl transferase, archaeosortase A system-associated</td>
            <td rowspan=1>Тело гена</td>
            <td rowspan=1>731, 752</td>
        </tr>
        <tr>
            <td rowspan=1>WP_054298578.1</td>
            <td rowspan=1>oligosaccharyl transferase, archaeosortase A system-associated</td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>731</td>
        </tr>
    </tbody>
</table>

### 4.3. Множественное белковое выравнивание
Результаты выравнивания находятся в директории `alignments`.
<details>
  <summary>Выравнивание для кластера №1</summary>
  
  ```
  >WP_011032848.1_Methanosarcina_mazei_Go1
MVKRALLSVSDKTGIVEFARGLEALGVKIISTGGTAKILRDADIEVTDVSEVTGYPEMMGGRVKTLHPRIHGGLLCLRES
KEQMEEAAKEDISLIDLIAVNLYPFEITVSRENVELEEAIENIDIGGPTLLRSAAKNYRSVTVLSDPSDYGRILKELRSS
GIISDKTRAELAVKAFRHTADYDAAIDTYLSRTLLGEEVLHLKFADGVKLRYGENWHQKAYFYKDSAIKGPSLAKAIQLH
GKELSYNNYVDADNALQTVKELGNASPAVAIVKHNNPCGLATGESLLQALHSAWDGDPISAYGSIICTNEVFDLEAATFL
NGKFVEIILAPDFKPDALEYLKKKSENLRLLKLPDLREGFGAEYTYKYVIGGMLKQSRDIGIYEKWESVTEVPYPENKRA
LSEFCLKACKATKSNAVILAYEYEPGNFMVLGMGAGQPNRVDSIRKLAATKAVENLKVIYEREQPAVPFEEYCQKIMSEC
VMASDAFFPFDDSVVHAAENNIRYIVSPGGSIRDNEVIATANRLGVALVFTGMRHFLH
>WP_048124614.1_Methanosarcina_lacustris_Z-7289
MVKRALLSVSDKTGIAEFARGLEALGVKIISTGGTAKILRDAGIEVTDVAEVTGYPEMMGGRVKTLHPRIHGGLLCLRDS
KEQMAEAAKEDISLLDLVAVNLYPFEVTVSKEGVELEEAIENIDIGGPTLLRSAAKNYRSVTVISDPSDYGHVLTELRSS
GVISDKTRADLAVKAFRHTADYDAAIDTYLSKTLLGEEVLRLKFTDGVKLRYGENWHQKASFFKDPKMEGPTLAKAVQLH
GKELSYNNYVDADNALQTIKELGNTSPAVVIVKHNNPCGLATGDKLLQALQAAWDGDPISAYGSIICTNEIFDLESATFL
NGKFVEIILAPDFKPDALEYLKNKSENLRLLKLSEFRESFGTEYTYKYVIGGMLKQSRDIGIYEKWECVTEFPYPEEKRV
LSEFCLKACKATKSNAVTLAHEYEPGYFMALGMGAGQPNRVDSIRKLAATKAIENLRAIYEREQPAAPFEEYCQKILLEC
VMASDAFFPFDDSVVYAAENNIRYIVSPGGSIRDNEVIATANRLGVSLVFTGMRHFLH
>WP_048167316.1_Methanosarcina_thermophila_TM-1
MVKRALLSVSDKTGITEFARGLQSLGVKIISTGGTAKVLRNAGIEVTDVSEITGFPEMMGGRVKTLHPRIHGGILCLRES
KEQMAEAIKEDISLIDMVAVNLYPFEETVSKEGVKLEEAIENIDIGGPTLLRSAAKNYRSVTVLSDPSDYGHVLEELRST
GVISEATRAALAIKAFRHTANYDAAIDVYLSKTLLGENVLRLNFTEGVKLRYGKNWHQEAFFYKDPKIEGPTLAKAIQLH
GKELSYNNYVDADNALQTVKEIGNVSPAVAIVKHNNPCGLATGSTLLQALQAAWDGDPVSAYGSIICTNEIFDLEAATFL
NGKFVEIILAPDFKPDALEFLKKKSENLRLLKLPELREAFGTDYTYKYIIGGMLKQSRDIGLYEKWESVTDIPYPEEKRP
LSEFCLKACKTTKSNAVILAHEYEPGYFMVLAMGAGQPNRVDSIRKLAATKAVENLRIIYEREKPAISFEEYKQKIISEC
VMASDAFFPFDDSIVYAAQNNIRYIVSPGGSIRDSEVIATANRLGVSMIFTGMRHFLH
>WP_048122363.1_Methanosarcina_vacuolata_Z-761
MVKRALLSVSDKTGIAEFARGLESLGVKIISTGGTAKILRDAGIEVTDVSEVTGCPEMMGGRVKTLHPRIHGGLLCLRES
KEQMAEAEREDISLIDMVAVNLYPFEVTVSKESVELEEAIENIDIGGPTLLRSAAKNYRSVIVLSDPLDYGRVLKELRST
GVVSEATRAALAVKAFRHTADYDAAIDTYLSKTLLEENVLRLNFTGGVKLRYGENWHQKAYFYKDSQIEGPTLAKATQLH
GKELSYNNYVDADNALQTVKELGSAHPGVAIVKHNNPCGLATGSTLLQALQAAWDGDPISAYGSIICTNEIFDLEAATFL
NGKFVEIILAPDFKPDALEYLKKKSENLRLLKLPDLREAFGTDYTYKYVIGGMLKQSRDIGLYEKWESVTDISYPEEKRS
LSEFCLKACKSTKSNSVILAHEYEPGFFMVLAMGAGQPNRVDSIRKLAATKAVENLRIIYERENPETSFEDYCQRVMSEC
VMASDAFFPFDDSIIHAAENDIRYIVSPGGSIRDGEVIAAANRLGVSMVFTGMRHFLH
>WP_054299839.1_Methanosarcina_flavescens
MVKRALLSVSDKTGITEFARGLQSLGVKIISTGGTAKILRDAGIEVTDVSEITGFPEMMGGRVKTLHPRIHGGILCLRES
REQMAEAIKEDISLIDMVAVNLYPFEETVSKEGVKLEEAIENIDIGGPTLLRSAAKNYRSVTVLSDPSDYEHVLEELRST
GVISESTRAALAIKAFRHTADYDAAIDVYLSKTLLGENILRLNFTDGVKLRYGENWHQEAFFYKDPEIEGPTLAKAVQLH
GKELSYNNYVDADNALQTVKEIGNASPAVAIVKHNNPCGLATGSTLLQALQAAWDGDPVSAYGSIICTNEIFDLEAATFL
NGKFVEIILAPDFKPDALEYLKKKSENLRLLKLPELREAFGTDYTYKYIIGGMLKQSRDIGIYEKWESVTDIPYPEEKRP
LSEFCLKACKTTKSNAVILAREYEPGFFMVLAMGAGQPNRVDSIRKLAATKAVENLRIIYEREQPAISFEAYRQEIISEC
VMASDAFFPFDDSIVYAAQNNIRYIVSPGGSIRDSEVIATANRLGVSMIFTGMRHFLH
  ```
</details>

<details>
  <summary>Выравнивание для кластера №2</summary>
  
  ```
  >WP_011033897.1_Methanosarcina_mazei_Go1
MRAELTSLFGLNIYTNNGVYVGKLQDLVIDVEEQKVTGLAVSDINRELFDISSRGIIIPYRWVITAADIIIVRDVIQRYK
KRKED
>WP_054300002.1_Methanosarcina_flavescens
MRAELTSLFGLNIYTNTGVYVGKLQDLVIDIEEQKITGLAISDINRELFDLTSRGVIIPYRWVITAADIIIVRDVIQRYK
KRKED
>WP_011306735.1_Methanosarcina_vacuolata_Z-761
MRAELTSLFGLNVYTNAGVYVGKLQDLVIDIEDQKITGLAISDINRELFDLTTRGVIIPYRWVITAADIIIVRDVIQRYK
KRKED
>WP_048167122.1_Methanosarcina_thermophila_TM-1
MRAELTSLFGLNIYTNTGVYVGKLQDLVIDIEEQKITGLAVSDINRELFDLTSRGVIIPYRWVITAADIIIIRDVIQRYK
KRKED
>WP_048127780.1_Methanosarcina_lacustris_Z-7289
MRAELTSLFGLNIYTNTGVYVGKLQDLVIDVEEQKVTGLAVSDINRELFDLSSRGMIIPYRWVITAADIIIIRDVIQRYK
KRKED
  ```
</details>

<details>
  <summary>Выравнивание для кластера №3</summary>
  
  ```
  >WP_011032293.1_Methanosarcina_flavescens
MANRPLDILNNALDTPVIVRLKGAREFRGELKGYDIHMNLVLDNAEELREGEVVSKFSSVVIRGDNVVYVSP
>WP_011032293.1_Methanosarcina_mazei_Go1
MANRPLDILNNALDTPVIVRLKGAREFRGELKGYDIHMNLVLDNAEELREGEVVSKFSSVVIRGDNVVYVSP
>WP_011032293.1_Methanosarcina_thermophila_TM-1
MANRPLDILNNALDTPVIVRLKGAREFRGELKGYDIHMNLVLDNAEELREGEVVSKFSSVVIRGDNVVYVSP
>WP_048121098.1_Methanosarcina_vacuolata_Z-761
MANRPLDILNNALDTPVIVRLKGAREFRGELKGYDIHMNLVLDNAEELREGEIVSKFSSVVIRGDNVVYVSP
>WP_011023130.1_Methanosarcina_lacustris_Z-7289
MANRPLDILNNALDTPVIVRLKGAREFRGELKGYDIHMNLVLDNAEELRDGEVVSKFSSVVIRGDNVVYVSP
  ```
</details>

<details>
  <summary>Выравнивание для кластера №4</summary>
  
  ```
  >WP_048167854.1_Methanosarcina_thermophila_TM-1
MVKVINSSGKHKTATARATVTKGTGKVRINKIPLELYTPELARIKISEPLLIAGDEVVSGLDIDVDVRGGGIIGQANAVR
TAVARGIVEWTNDTVIRDNFASYDRNLLVNDSRQKESKNFGGPGARAKYQKSYR
>WP_048124440.1_Methanosarcina_lacustris_Z-7289
MVKVVNSSGKHKTATARATVMKGTGKVRINKIPLELYTPELAMMKVSEPLLIAGNEVVSGLDINVDVRGGGIIGQANAVR
TAVARGIVEWTNDTIIRDNFVTYDRSLLVSDSRQKESKNFGGPGARAKYQKSYR
>WP_011033697.1_Methanosarcina_mazei_Go1
MVKVINSSGKHKTATARATVMKGTGKVRINKIPLELYTPELAMMKISEPLLIAGKDVVSGLDINVDVRGGGIVGQANAVR
TAVARGIVEWTNDTTIRDNFAAYDRNLLVSDSRQKEAKNFGGPGARSKYQKSYR
>WP_048117809.1_Methanosarcina_vacuolata_Z-761
MVKVVNSSGKHKTATARATVTKGTGKVRINKIPLELYTPELVMMKISEPLLIAGDEVVSGLDINVDVRGGGIIGQANAVR
TAVARGIVEWTNDTIIRDNFASYDRNLLVSDSRQKESKNFGGPGARAKYQKSYR
>WP_054297845.1_Methanosarcina_flavescens
MVKVINSSGKHKTATARATVTKGTGKVRINKIPLELYAPELVRMKISEPLLIAGDEVVSGLDINVDVRGGGIVGQANAVR
TAVARGIVEWTNDTVIRDNFASYDRNLLVNDSRQKESKNFGGPGARAKYQKSYR
  ```
</details>

<details>
  <summary>Выравнивание для кластера №5</summary>
  
  ```
  >WP_054297609.1_Methanosarcina_flavescens
MERKTRMILALDVSDREEALKIAEDVSEFVDAIKVGYPLVLATGLEIIRELAEFAPIIADFKVADIPNTNRLICKQVFEA
GADAVIVQGFTGRDSLDACIEVASEYRRDVFVVSEMSHPGGAEFLQPVGEAIARMASEAGAFGLVAPATRPERVKKIRKI
IGDKLTIISPGVGAQGGRASDVIAAGADWVIVGRSIYKAELPKEAASEIAAEIEAELRGEG
>WP_011034015.1_Methanosarcina_mazei_Go1
MERNTCMILALDVTEREEALKIAENVREFVDAIKVGYPLILATGLDIIRELARFAPVIADFKVADIPNTNRLICEQVFKA
GADAVIVQGFTGRDSLDACIEVASKYGKDVFVVSEMSHPGGAEFLQSAAEAIAKMAVEAGAFGLVAPATRPERVKEIRKI
IGDRLTIISPGVGAQGGKASDVISAGADWVIVGRSIYKAESPKEAACEIAEEIQAELRG-K
>WP_048167159.1_Methanosarcina_thermophila_TM-1
MERKTRIILALDVSDREEALKIAEDVSEFVDAIKVGYPLVLATGLEIIRELAEFAPIIADFKVADIPNTNRLICEQVFEV
GADAVIVQGFTGRDSLDACIEVASEYRKDVFVVSEMSHPGGAEFLQPVGEAIARMAAEAGASGLVAPATRPERVKKIREI
VGDKLTIISPGVGAQGGRASNAIAAGADWVIVGRSIYKAELPKKAASEIAAEIEAELRREG
>WP_048118415.1_Methanosarcina_vacuolata_Z-761
MEKKSCMILALDVSDREEALKIAEDVSEFVDAIKVGYPLILATGLGIIRELAEFAPIIADFKVADIPNTNRLICEQVFEA
GAEAVIAQGFTGRDSLDACIEVASEYRKDVFVVSEMSHPGGAEFLQPVGEAITRMAAEAGAFGLVAPATRPERVKAIRKI
IGEKLTIISPGVGAQGGKASDVIAAGADWVIVGRAIYKAESPREAARKIATEIEVEIKGEN
>WP_048127553.1_Methanosarcina_lacustris_Z-7289
MERNTCMILALDVTDREEALKIAEDVWEFVDAIKVGYPLILATGLGIIRELAEFAPVIADFKVADIPNTNRLICDQVFEA
GADAVIVQGFTGRDSLDACIDIASEYSRDVFVVSEMSHPGGAEFMQPAAEAIARMALEAGAFGLVAPATRPERVKKIRKI
VGDKLTIISPGVGAQGGRASDVIAAGADWVIVGRSIYRAESPKEAARKIAEEIQAELRGEY
  ```
</details>

<details>
  <summary>Выравнивание для кластера №6</summary>
  
  ```
  >WP_011032199.1_Methanosarcina_mazei_Go1
MPTIGIADTTFARYNMGRAAIDEIQKNVSAQIKRVTVPGIKDLPVAAKKLIEEEGCDIVMALGMPGGKEKDKMCAHEASQ
GLIMAQLMTNTHIIEVFVHEDEGKDEKELAFLMDRRTREHALNVIKLLFKPEKLVREAGTGQRQGFEDAGPLRM
>WP_048119173.1_Methanosarcina_vacuolata_Z-761
MPTIGIADTTFARYNMGRAAIDEIQKNVSVKIKRVTVPGIKDLPVAAKKLIEEEGCDIVMALGMPGAKEQDKICAHEASQ
GIIMAQLMTNTHIIEVFVHENEGKDEKELAFLMDRRTREHALNVIKLLFKPEKLIREAGTGQRQGFEDAGPL--
>WP_048126706.1_Methanosarcina_lacustris_Z-7289
MPTIGIADTTFARYNMGRAAIDEIQKNVSVQIKRVTVPGIKDLPVAAKKLIEAEGCDIVMALGMPGAQQKDKMCAHEASQ
GLIMAQLMTNTHIIEVFVHEDEGKDEKELAFLMDKRTREHALNVIKLLFKPEKLIREAGTGQRQGFEDAGSLRM
>WP_048166057.1_Methanosarcina_thermophila_TM-1
MPTIGIADTTFARYDMGRAAIDEIQKNVSVKIKRVTVPGIKDLPVAAKKLIEEEGCDIVMALGMPGAKEQDKICAHEASQ
GLIMAQLMTNTHIIEVFVHEDEGKDEKELAFLMDRRTREHALNVIKLLFKPEKLIREAGTGQRQGFEDAGPLRM
>WP_054297806.1_Methanosarcina_flavescens
MLTIGIADTTFARYNMGRAAIDEIQKNVSVKIKRVTVPGIKDLPVAAKKLIEEEGCDIVMALGMPGAKEQDKICAHEASQ
GLIMAQLMTNTHIIEVFVHENEGKDEKELAFLMDRRTREHALNVIKLLFKPDKLIQEAGTGQRQGFEDAGPLRM
  ```
</details>

<details>
  <summary>Выравнивание для кластера №7</summary>
  
  ```
  >WP_048127129.1_Methanosarcina_lacustris_Z-7289
MPKLTLISTIYALEPVIICVTRLSPSKIIMLSEEGADEKKLRSEEMIEKTFKNALEVEKRDTALYDTVRVAKDVAELIEK
EHDRGNLVIVNVSGGRKPQAFGALFGAYARNDMVQRVVYVTEEDSMMIDFPVLSFNLSETKKLILEEIQKGVSAVSQIAV
TAGISKGMTYNHLRELKSMGYIADGDNGYIITDAGKIASI
>WP_231588106.1_Methanosarcina_thermophila_TM-1
--------------------------------------------------------------------------------
-----------MSGGRKPQAFGALFGAYARNDMVQRVVYVTEEDSFMIDFPVLSFNLSETKKLILEEIQKGVSSVTKIAA
TAGISKGMTYNHLRKLKAMGYIADGESGYIITDAGRIASI
>WP_011032516.1_Methanosarcina_mazei_Go1
MSKLTLISTIYSLEPVIICVTRLSPSKIILLSEEGANDKKVQSEDIIEKTFKNALEVEKKYTALYDTVRVAKDVAELIEK
EHDRGNQVIVNVSGGRKPQAFGALFGAYARNDMVQRVVYVTEEDSMMIDFPVLSFNLSETKKLILEEIQKGNSSVTKIAA
TAGISKGMTYNHLRELKSMGYIADGDSGYIITDAGRIASI
>WP_048117996.1_Methanosarcina_vacuolata_Z-761
MSKLTLISTIYSLEPVIICVTRLSPSKIILLSEEGAPDKKVQSEEMIEKTFKNALEIEKKYTSVYDTVRVAKDVAELIEQ
EHDRGNQVIVNVSGGRKPQAFGALFGAYARNDMVQRVVYVTEEDSFMIDFPVLSFNLSETKKLILEEIQKGVSSVTQIAV
TAGISKGMTYNHIRELKAMGYITDGENGYIITDAGRIASI
>WP_054298565.1_Methanosarcina_flavescens
MSKLTLISTIYSLEPVIICVTRLSPSKIILLSEEGAPDKKVQSEEMIEKTFKNALVVEKKYTSVYDTVRVAKDVAELIEQ
EHAKGNQVIVNVSGGRKPQAFGALFGAYARNDMVQRVVYVTEEDSFMIDFPVLSFNLSETKKLILEEIQKGVSSVPQIAA
TAGISKGMTYNHLRELKAMGYIADGESGYIITDAGRIASI
  ```
</details>

<details>
  <summary>Выравнивание для кластера №8</summary>
  
  ```
  >WP_048124226.1_Methanosarcina_vacuolata_Z-761
MITTNKGMGCPVAKRPAHRLKFSIISLIAVALVAFLMRMISYSAATANGSINLMGYDSFYHMRRILYTTFNFPHPLNFDT
YINYPAGFEVGWPPFFDFLGALLAKVLGVGNPSLYTTEFAGALLPVLLGVLTIIPLYIAAAAIFDRKTALLGALVFAVIP
AHVYVSRFGAVDHHVAETLLSTSAYACFILALKWAREGSLSLASLKTISSEKKLIKSLAFAGASGLFFALLIYTWIGALV
FVSFILLYAFIQTIIDLKAEKNSDYLLISSTVALLATLIFTIPLSAGSLRPGLEMSAMYLSWFQVFYVFSMLAGTLILWG
FSLYISKKGLDWKYYPAALILISVAGLLSLKILSAESYSFVIEGMSFFLGKGEYISTIAEALPIFLTTDGTLTFSPILGS
LGLCFITALGGLFLLGLEWIGEKSKSEGVFFLLWSVFFAYLTLSQRRFSYLFAVNVAILTSYFLWVLLDSFDFETEVKKL
AKSVPIHGNNAMITSKAEMETKSKRAEKETKSKKAEKETKSKIKSKSKINNLSGSK-QNSQPDYFKIFSSLVLIGLVFIP
CILAGFAFAKDQGLIDPVWKDSLTWLGASSPETSYYLDPAGTPEYGVLSWWDYGNWIVYQAQRPAVSNNFQTGVDDSAHF
FTTDSEEEAKAIIEKLKVKYVMTDNLMAGGKFGSIVKLAGENISKYVNVQTVNVNGGLQTIATAKKEFTETEVYRLHQLD
GSNLGNLRLAHESTASV--DDNDTVSDVKIFEFVPGARLSGTADPGQNITATLELSSNTGRKFTYQNEVMSDKNGSFEIT
VPYSTDNNAGGVSALSTYSLNAGRNTTVSEIQVTEDDVLKGNKIEVKIPDSK
>WP_232308693.1_Methanosarcina_lacustris_Z-7289
-------MRSPAEKGSANSSRIKIISFIAVIVVAFLMRMLSYASLTADGGITFTGYDEFYHMRRILYTVSSFPHILNFDT
YINYPYGFEIGWPPLFDLLGALLAIILGGGHPDMHTVEFAGALLPVLLGVLTLIPVYMVATSVFDRKTGLLGAFIFAVLP
AHVYISRFGAVDHHVAEVLLSTAAYAFFILALKLAGESKLSLNSLKNIASDKKLLNPLVFAAASGLFFSLLVFTWVGAPA
LISFVVLYALVQATLDLKAGKGSDYLFVCSAVTLFATLLFTIPLSAGAARPGLEMSAMYLSWFQVVYVLILLAGLFFLWG
FSAYVSKKGMDWKYYPGVLILVFGSGLLFLRLFSVEYYAFVIEGLRFFSGKGEYIGTISEAVPLFLTSQGKFTLSSVIGS
FGLSFLTALAGFFLFSLELKGEKLKPEGVFFLVWTLFYAYLALSQRRFTYLFAINISILTAYIMWVLMDSLDFGKEIKKL
VKSGKKTENNS------------------ESTFKTGQKTVSRTKSKSKARHVAESRSTDEGSDYFKLVSGVALIGLVFVP
SIWLGAAFSKDAVSIGPEWEDSLKWLEASTPATSYYLEPSETPEYGVLSWWDYGNWIVYVGKRPVVANNFQTGVDDSARF
FITDSEEEAKTIVEKLNVKYVITDTLMAEGKFSAIAEIAGKNIGDYYEVKTTNENTGLTTVATPKQALLQSEIYKLHKLD
GTSLGNFRLIHESTINSTENESSKIDTVKIFEYVPGATLTGTASPNQAVMATLELSSNTGRKFTYQKGEMADENGSFEIT
VPYSTENTGNGVHATSAYSLTAGDNSTIATIQVTENDILDGNIIKVKN---S
>WP_011034141.1_Methanosarcina_mazei_Go1
MIITNNITRISETKKIPKKINLGIISLLIVFMIAFLMRMLSYASLTADGGITFTGYDEFYHMRRILYTTFNFPSFLNFDT
YINYPYGFEVGWPPFFDLLGALLAIILGAGQPDVHTVEFAGAILPVLLGVLTIIPVYVIAASIFNRKTGLVGALVFAVLP
AHVYISRFGTVDHHVAEVFLSTVAYAFFILALKQAGESKLSSGSLKNISSDKKPVKPLVYSAVSGLFFSLLIFTWVGAPA
FVSFIVLYALIQATLDLKTGRKSDYVFICSAVALLATLLFTIPLSAGAVREGLEMSAMYLSWFQVVYLVIMLTGILLLWG
FSSYASKKEMDWKYYPGILILVFGSGLLFLRMFSGEYYAFIIEGMRFFSGKGEYISTIVEAVPLFLTGQGKFTLSGVLGS
FGLTFLTALAGLFLLILELKSEKSRPENIFFLVWTLFYAYLALSQRRFTYLFALNVSILTAYLFWVLMESLDFENEIKKL
IKRGKGERKVS------------------ETALQTEKKSSLKRKSKNRQVTESKS--KTDEPDYFKLVSGTALIALIFVS
SIWIDVTYAKDGVSIDPGWQDSLEWLEASTPETSYYLEPSETPEYGVLSWWDYGNWIVYVGKRPAVSNNFQTGVEDSANF
LLTDSEEEAKTIVEKLKVKYVMTDTLMAEGKFSSITSLAGKEIGEYYEVETVKGDTGLRTVATPKQALLQTQVYKLHKLD
GTSLGHFRLVHESAVNSTDDGNSKENTVKVFEYVKGATLSGTASPNETVMATLELSSNTGRKFTYQKGDVADENGLFEIT
VPYSTESTGDGVHATSAYSLTSGEKPITSGIQVTEDDILNGNRIEVKAPEGA
>WP_048168165.1_Methanosarcina_thermophila_TM-1
MVTTNKGMRCPAVKRPANNLKFSIIALTAVVIVAFLMRMLSYTSVTANGSITFNGYDDFYHMRRILYTASNFPHSLNFDS
YINYPQGFEVGWPPLFDLLGALLAIILGGGQPDLYTIEFAGALLPLLLGILTIIPLYFVTSSVFDRRTALLAAFIFAVLP
AHVYISRFGAVDHHVAETLLSTSAYAFFIFALKRAGEGPLSLTSLKNISSDKKHIKTLASAAASGLFLALLIFTWIGAPV
FVSFIVLYAFIQTTLDLRVGKSSDYLLICTITSLLATLLFTIPLVAGSVRPGLEMSAMYLSWFQVLYVLSLVAGTLILWG
FSSYISKKDLDWKYYPAVLILISGLGLLSLRILSAEYYAFIIEGMRFFLGKGEYISTIVEAVPLFLTAQGKLTFSPVLSS
LGLCFLAALGGFFLLCLEWRGEKSKPEGIFFLLWSIFFAYLAISQRRFTYLFAINVSILTAYFLWVLLESFDFEAELRKL
IKSGPITSKNS------------------TSALKVEKETKSKKKSKQKISNTSGSK-KDQQPDYFKIVSSVALIGLVFVP
CIWAGFAFAKEGGSVDPEWKEALTWLEASSPETSNYLEPSETPEYSVLSWWDYGNWIVYLAKRPVVSNNFQTGIQDSAHF
FTTDSEEEAKAIMEKLNVKYVITDKQMASGKFGAIVELAGKDIEQYFKIETIKGKTGLETVATAKDEFKNTEIYKLHELD
GSNLGNLRLIHESSIPE--EKGGKKNDVKIFEFVPGAKLSGTASPGQNVTATLMLNSNTGREFTYQNTAVSDKNGLFEIT
VPYSTENTAHGVRAVSAYSVSAGGNATVSGIQVTEEDVLNGNQVEVKNLEMN
>WP_054298578.1_Methanosarcina_flavescens
MVTTNKGMRCPAVKRPANNLKLSIIALTAVVIVAFLMRMLSYASVTANGSITFNGYDDFYHMRRILYTASNFPHSLNFDS
YINYPQGFEIGWPPLFDLLGALLAMILGGGQPDLYTIEFAGALLPLLLGILTIIPLYFVTSSVFDRKTALLAAFIFAVLP
AHVYISRFGAVDHHVAETLLSTSAYAFFIFALKWAGEGSLSLTSLKNISSDKKYIKTLASAAASGLFFALLIFTWIGAPV
FVSFIVLYAFIQTTLDLRAGKNSDYLLICTITSLLATLLFTIPLVARSVRPGLEMSAMYLSWFQVLYVLSLVAGTLILWG
FSSYISKKDLNWKYYPAILILVSGLGLLSLRILSAEYYAFVIEGMRFFLGKGEYIGTIAEAVPLFLTAQGKLTFSPVLSS
LGLCFLAALGGFFLLCLEWRGEKSKPEGIFFLLWSIFFAYLAISQRRFSYLFAVNVSILTAYFLWVLLESFDFEAEVRKL
IKSGPITAKNS------------------TSALKEEKETKSKKKSKQKISNTLGSK-KDQQPDYFKIVSSVALIGLVFIP
CIWSGFAFAKEGGSVDPEWKEALTWLEASSPETSNYLEPSETPEYSVLSWWDYGNWIVYLAKRPVVSNNFQTGIQDSAHF
FTTDSEEEAKAIMEKLNVKYVITDKQMASGKFGAIVELAGKDIEQYFKIETVKGKTGLETVATAKNEFKNTEVYKLHELD
GSNLGNLRLVYESSIPE--EKGGKKNDVKIFEFVPGAKLSGTASPGQNVTATLVLNSNTGREFTYQNTAMSDKNSSFEIT
VPYSTENTAHGVRAVSAYSVSTGGNATVSGIQVTEDDVLNGNRIEVKSLETN
  ```
</details>
  
### 4.4. Визуализация расположения участков Z-DNA
Для демонстрации было выбрано 8 кластеров. В некоторых из них во всех гомологичных белках сохраняются участки Z-ДНК, в некоторых - нет (такие кластеры были выбраны специально для иллюстрации). Порядок орагнизмов соответсвует порядку в приведенной ранее таблице (см. п. 1).  
![image](https://user-images.githubusercontent.com/55440084/172192722-7ba256f7-c755-4b08-85ec-cd6026c6aec7.png)
![image](https://user-images.githubusercontent.com/55440084/172192776-78c8ecc9-4f51-48b6-be6b-80350876d888.png)
![image](https://user-images.githubusercontent.com/55440084/172192850-0bc987ab-b3f1-4bb2-875c-b934d7fb5c2c.png)
![image](https://user-images.githubusercontent.com/55440084/172192903-bd73299b-803d-4596-9f7f-6fa788fcf47f.png)
![image](https://user-images.githubusercontent.com/55440084/172192957-568c5e8e-8ae7-4e3e-93b3-fa735c0ef987.png)
![image](https://user-images.githubusercontent.com/55440084/172193003-d1db2ad0-b3b5-419e-ab5f-9eaa364c383d.png)
![image](https://user-images.githubusercontent.com/55440084/172193042-72da5c90-e639-4d61-b17e-8419c0447eac.png)
![image](https://user-images.githubusercontent.com/55440084/172193088-345bd1f7-b43b-4cc5-bbe3-d93f976bade3.png)


## 5. Предсказание G-квадруплексов
