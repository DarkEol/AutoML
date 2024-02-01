# Comparision of AutoSklearn Runs under different conditions

| N | Dataset | AutoML library | Limit | Num. DS | Data characteristic | Selected algorithm | Accuracy | Precision | Recall | F-measure | AUC | Time elapsed |
|---|---------|----------------|-------|---------|---------------------|--------------------|----------|-----------|--------|-----------|-----|--------------|
| 0 | adult | Auto-Sklearn | No limits |  | No characteristics | gradient_boosting | 0,869996929 | 0,770165209 | 0,665407221 | 0,713963964 | 0,800687907 | 894,4867167
| 1 | adult | Auto-Sklearn | cost <= 0.15 |  | No characteristics | random_forest | 0,853823319 | 0,731104651 | 0,633501259 | 0,678812416 | 0,779184635 | 45,91373444
| 2 | adult | Auto-Sklearn | cost <= 0.15 | 35 | BinaryClass, BinaryAttributes, MissingValues | random_forest | 0,853823319 | 0,731104651 | 0,633501259 | 0,678812416 | 0,779184635 | 44,42252398
| 3 | adult | Auto-Sklearn | cost <= 0.15 | 35 | BinaryClass, BinaryAttributes, MissingValues | random_forest | 0,853823319 | 0,731104651 | 0,633501259 | 0,678812416 | 0,779184635 | 44,66560555
| 4 | adult | Auto-Sklearn | cost <= 0.15 | 35 | BinaryClass, BinaryAttributes, MissingValues | random_forest | 0,853823319 | 0,731104651 | 0,633501259 | 0,678812416 | 0,779184635 | 43,61937571
5 | adult | Auto-Sklearn | cost <= 0.15 | 50 | MissingValues, NoUnaryAttibutes, NumericAttributes | random_forest | 0,853823319 | 0,731104651 | 0,633501259 | 0,678812416 | 0,779184635 | 44,83941889
6 | adult | Auto-Sklearn | cost <= 0.15 | 50 | MissingValues, NoUnaryAttibutes, NumericAttributes | random_forest | 0,853823319 | 0,731104651 | 0,633501259 | 0,678812416 | 0,779184635 | 43,5070169
7 | adult | Auto-Sklearn | cost <= 0.15 | 50 | MissingValues, NoUnaryAttibutes, NumericAttributes | random_forest | 0,853823319 | 0,731104651 | 0,633501259 | 0,678812416 | 0,779184635 | 44,4016664
8 | bank-<br>marketing | Auto-Sklearn | No limits |  | No characteristics | gradient_boosting | 0,907110472 | 0,624113475 | 0,502857143 | 0,556962025 | 0,731536166 | 895,0670404
9 | bank-<br>marketing | Auto-Sklearn | cost <= 0.1 |  | No characteristics | random_forest | 0,906778724 | 0,658499234 | 0,40952381 | 0,504991192 | 0,690812199 | 41,00574136
10 | bank-<br>marketing | Auto-Sklearn | cost <= 0.1 | 35 | BinaryClass, BinaryAttributes, NoMissingValues | random_forest | 0,906778724 | 0,658499234 | 0,40952381 | 0,504991192 | 0,690812199 | 40,01231694
11 | bank-<br>marketing | Auto-Sklearn | cost <= 0.1 | 35 | BinaryClass, BinaryAttributes, NoMissingValues | random_forest | 0,906778724 | 0,658499234 | 0,40952381 | 0,504991192 | 0,690812199 | 41,3057251
12 | bank-<br>marketing | Auto-Sklearn | cost <= 0.1 | 35 | BinaryClass, BinaryAttributes, NoMissingValues | random_forest | 0,906778724 | 0,658499234 | 0,40952381 | 0,504991192 | 0,690812199 | 38,50998688
13 | bank-<br>marketing | Auto-Sklearn | cost <= 0.1 | 50 | NoMissingValues, BinaryClass, BinaryAttributes | random_forest | 0,906778724 | 0,658499234 | 0,40952381 | 0,504991192 | 0,690812199 | 38,52636075
14 | bank-<br>marketing | Auto-Sklearn | cost <= 0.1 | 50 | NoMissingValues, BinaryClass, BinaryAttributes | random_forest | 0,906778724 | 0,658499234 | 0,40952381 | 0,504991192 | 0,690812199 | 39,8407867
15 | bank-<br>marketing | Auto-Sklearn | cost <= 0.1 | 50 | NoMissingValues, BinaryClass, BinaryAttributes | random_forest | 0,906778724 | 0,658499234 | 0,40952381 | 0,504991192 | 0,690812199 | 38,58718872
16 | car | Auto-Sklearn | No limits |  | No characteristics | mlp | 0,98265896 | 0,960927961 | 0,957163811 | 0,958476463 | 0,999396974 | 894,2744396
17 | car | Auto-Sklearn | cost <= 0.23 |  | No characteristics | random_forest | 0,947976879 | 0,922487322 | 0,850474949 | 0,877187469 | 0,993176298 | 9,639993668
18 | car | Auto-Sklearn | cost <= 0.23 | 35 | NoBinaryClass, NoNumericClass, NoManyInstances | liblinear_svc | 0,901734104 | 0,787135973 | 0,660628143 | 0,695724108 | 0,986666176 | 8,161915302
19 | car | Auto-Sklearn | cost <= 0.23 | 35 | NoBinaryClass, NoNumericClass, NoManyInstances | liblinear_svc | 0,901734104 | 0,787135973 | 0,660628143 | 0,695724108 | 0,986666176 | 9,637272835
20 | car | Auto-Sklearn | cost <= 0.23 | 35 | NoBinaryClass, NoNumericClass, NoManyInstances | liblinear_svc | 0,901734104 | 0,787135973 | 0,660628143 | 0,695724108 | 0,986666176 | 8,252195835
21 | car | Auto-Sklearn | cost <= 0.23 | 50 | NoMissingValues, NoBinaryClass, FewInstances | libsvm_svc | 0,921965318 | 0,83742991 | 0,708558391 | 0,727175331 | 0,977447997 | 8,797470331
22 | car | Auto-Sklearn | cost <= 0.23 | 50 | NoMissingValues, NoBinaryClass, FewInstances | libsvm_svc | 0,921965318 | 0,83742991 | 0,708558391 | 0,727175331 | 0,977447997 | 8,641489029
23 | car | Auto-Sklearn | cost <= 0.23 | 50 | NoMissingValues, NoBinaryClass, FewInstances | libsvm_svc | 0,921965318 | 0,83742991 | 0,708558391 | 0,727175331 | 0,977447997 | 9,175410271
24 | Amazon_<br>employee_<br>access | Auto-Sklearn | No limits |  | No characteristics | extra_trees | 0,949649069 | 0,952939361 | 0,995968392 | 0,973978868 | 0,565972865 | 895,6172721
25 | Amazon_<br>employee_<br>access | Auto-Sklearn | cost <= 0.05 |  | No characteristics | extra_trees | 0,949649069 | 0,952939361 | 0,995968392 | 0,973978868 | 0,565972865 | 894,9856737
26 | Amazon_<br>employee_<br>access | Auto-Sklearn | cost <= 0.05 | 35 | BinaryClass, NoBinaryAttributes, NoMissingValues | gradient_boosting | 0,946444919 | 0,960484887 | 0,983873569 | 0,972038557 | 0,636412705 | 898,5355978
27 | Amazon_<br>employee_<br>access | Auto-Sklearn | cost <= 0.05 | 35 | BinaryClass, NoBinaryAttributes, NoMissingValues | gradient_boosting | 0,946444919 | 0,960484887 | 0,983873569 | 0,972038557 | 0,636412705 | 898,3310034
28 | Amazon_<br>employee_<br>access | Auto-Sklearn | cost <= 0.05 | 35 | BinaryClass, NoBinaryAttributes, NoMissingValues | gradient_boosting | 0,946444919 | 0,960484887 | 0,983873569 | 0,972038557 | 0,636412705 | 897,68645
29 | Amazon_<br>employee_<br>access | Auto-Sklearn | cost <= 0.05 | 50 | NoMissingValues, BinaryClass, NoBinaryAttributes | gradient_boosting | 0,946444919 | 0,960484887 | 0,983873569 | 0,972038557 | 0,636412705 | 898,0547452
30 | Amazon_<br>employee_<br>access | Auto-Sklearn | cost <= 0.05 | 50 | NoMissingValues, BinaryClass, NoBinaryAttributes | gradient_boosting | 0,946444919 | 0,960484887 | 0,983873569 | 0,972038557 | 0,636412705 | 898,5678468
31 | Amazon_<br>employee_<br>access | Auto-Sklearn | cost <= 0.05 | 50 | NoMissingValues, BinaryClass, NoBinaryAttributes | gradient_boosting | 0,946444919 | 0,960484887 | 0,983873569 | 0,972038557 | 0,636412705 | 898,3010352
32 | Australian | Auto-Sklearn | No limits |  | No characteristics | random_forest | 0,876811594 | 0,898305085 | 0,828125 | 0,861788618 | 0,873521959 | 894,385251
33 | Australian | Auto-Sklearn | cost <= 0.15 |  | No characteristics | random_forest | 0,876811594 | 0,898305085 | 0,828125 | 0,861788618 | 0,873521959 | 219,3451445
34 | Australian | Auto-Sklearn | cost <= 0.15 | 35 | BinaryClass, BinaryAttributes, NoMissingValues | adaboost | 0,905797101 | 0,93220339 | 0,859375 | 0,894308943 | 0,902660473 | 410,2056222
35 | Australian | Auto-Sklearn | cost <= 0.15 | 35 | BinaryClass, BinaryAttributes, NoMissingValues | adaboost | 0,905797101 | 0,93220339 | 0,859375 | 0,894308943 | 0,902660473 | 410,3763468
36 | Australian | Auto-Sklearn | cost <= 0.15 | 35 | BinaryClass, BinaryAttributes, NoMissingValues | adaboost | 0,905797101 | 0,93220339 | 0,859375 | 0,894308943 | 0,902660473 | 408,2810776
37 | Australian | Auto-Sklearn | cost <= 0.15 | 50 | NoMissingValues, BinaryClass, BinaryAttributes | adaboost | 0,905797101 | 0,93220339 | 0,859375 | 0,894308943 | 0,902660473 | 404,9099786
38 | Australian | Auto-Sklearn | cost <= 0.15 | 50 | NoMissingValues, BinaryClass, BinaryAttributes | adaboost | 0,905797101 | 0,93220339 | 0,859375 | 0,894308943 | 0,902660473 | 412,0376239
39 | Australian | Auto-Sklearn | cost <= 0.15 | 50 | NoMissingValues, BinaryClass, BinaryAttributes | adaboost | 0,905797101 | 0,93220339 | 0,859375 | 0,894308943 | 0,902660473 | 403,4875278
0 | blood-transfusion-service-center | Auto-Sklearn | No limits |  | No characteristics | k_nearest_neighbors | 0,793333333 | 0,727272727 | 0,390243902 | 0,507936508 | 0,667599015 | 896,8546588
1 | blood-transfusion-service-center | Auto-Sklearn | cost <= 0.2 |  | No characteristics | mlp | 0,8 | 0,739130435 | 0,414634146 | 0,53125 | 0,679794137 | 120,4862733
2 | blood-transfusion-service-center | Auto-Sklearn | cost <= 0.2 | 35 | BinaryClass, NoBinaryAttributes, NoMissingValues | libsvm_svc | 0,74 | 1 | 0,048780488 | 0,093023256 | 0,524390244 | 897,9957101
3 | blood-transfusion-service-center | Auto-Sklearn | cost <= 0.2 | 35 | BinaryClass, NoBinaryAttributes, NoMissingValues | libsvm_svc | 0,74 | 1 | 0,048780488 | 0,093023256 | 0,524390244 | 897,3492231
4 | blood-transfusion-service-center | Auto-Sklearn | cost <= 0.2 | 35 | BinaryClass, NoBinaryAttributes, NoMissingValues | libsvm_svc | 0,74 | 1 | 0,048780488 | 0,093023256 | 0,524390244 | 898,7075582
5 | blood-transfusion-service-center | Auto-Sklearn | cost <= 0.2 | 50 | NoMissingValues, BinaryClass, NoBinaryAttributes | libsvm_svc | 0,74 | 1 | 0,048780488 | 0,093023256 | 0,524390244 | 898,8073261
6 | blood-transfusion-service-center | Auto-Sklearn | cost <= 0.2 | 50 | NoMissingValues, BinaryClass, NoBinaryAttributes | libsvm_svc | 0,74 | 1 | 0,048780488 | 0,093023256 | 0,524390244 | 893,8631072
7 | blood-transfusion-service-center | Auto-Sklearn | cost <= 0.2 | 50 | NoMissingValues, BinaryClass, NoBinaryAttributes | libsvm_svc | 0,74 | 1 | 0,048780488 | 0,093023256 | 0,524390244 | 898,2039552
8 | christine | Auto-Sklearn | No limits |  | No characteristics | random_forest | 0,742619926 | 0,732692308 | 0,731285988 | 0,731988473 | 0,742197168 | 894,956002
9 | christine | Auto-Sklearn | cost <= 0.27 |  | No characteristics | random_forest | 0,749077491 | 0,74459725 | 0,727447217 | 0,73592233 | 0,748270678 | 61,68036699
10 | christine | Auto-Sklearn | cost <= 0.27 | 35 | BinaryClass, BinaryAttributes, NoMissingValues | random_forest | 0,749077491 | 0,74459725 | 0,727447217 | 0,73592233 | 0,748270678 | 59,73452139
11 | christine | Auto-Sklearn | cost <= 0.27 | 35 | BinaryClass, BinaryAttributes, NoMissingValues | random_forest | 0,749077491 | 0,74459725 | 0,727447217 | 0,73592233 | 0,748270678 | 60,23166728
12 | christine | Auto-Sklearn | cost <= 0.27 | 35 | BinaryClass, BinaryAttributes, NoMissingValues | random_forest | 0,749077491 | 0,74459725 | 0,727447217 | 0,73592233 | 0,748270678 | 59,30829453
13 | christine | Auto-Sklearn | cost <= 0.27 | 50 | NoMissingValues, BinaryClass, BinaryAttributes | random_forest | 0,749077491 | 0,74459725 | 0,727447217 | 0,73592233 | 0,748270678 | 59,71233368
14 | christine | Auto-Sklearn | cost <= 0.27 | 50 | NoMissingValues, BinaryClass, BinaryAttributes | random_forest | 0,749077491 | 0,74459725 | 0,727447217 | 0,73592233 | 0,748270678 | 60,35318613
15 | christine | Auto-Sklearn | cost <= 0.27 | 50 | NoMissingValues, BinaryClass, BinaryAttributes | random_forest | 0,749077491 | 0,74459725 | 0,727447217 | 0,73592233 | 0,748270678 | 58,99270129
16 | cnae-9 | Auto-Sklearn | No limits |  | No characteristics | liblinear_svc | 0,921296296 | 0,922953261 | 0,918742369 | 0,918576405 | 0,996502658 | 900,406086
17 | cnae-9 | Auto-Sklearn | cost <= 0.05 |  | No characteristics | liblinear_svc | 0,921296296 | 0,922953261 | 0,918742369 | 0,918576405 | 0,996502658 | 899,916831
18 | cnae-9 | Auto-Sklearn | cost <= 0.05 | 35 | NoBinaryClass, NumericClass, NoStringAttributes | libsvm_svc | 0,898148148 | 0,90172099 | 0,895816036 | 0,896835879 | 0,982296222 | 895,2986424
19 | cnae-9 | Auto-Sklearn | cost <= 0.05 | 35 | NoBinaryClass, NumericClass, NoStringAttributes | libsvm_svc | 0,898148148 | 0,90172099 | 0,895816036 | 0,896835879 | 0,982296222 | 898,5182335
20 | cnae-9 | Auto-Sklearn | cost <= 0.05 | 35 | NoBinaryClass, NumericClass, NoStringAttributes | libsvm_svc | 0,898148148 | 0,90172099 | 0,895816036 | 0,896835879 | 0,982296222 | 895,9231391
21 | cnae-9 | Auto-Sklearn | cost <= 0.05 | 50 | NoMissingValues, NoBinaryClass, FewInstances | libsvm_svc | 0,898148148 | 0,90172099 | 0,895816036 | 0,896835879 | 0,982296222 | 899,2042248
22 | cnae-9 | Auto-Sklearn | cost <= 0.05 | 50 | NoMissingValues, NoBinaryClass, FewInstances | libsvm_svc | 0,898148148 | 0,90172099 | 0,895816036 | 0,896835879 | 0,982296222 | 896,3343844
23 | cnae-9 | Auto-Sklearn | cost <= 0.05 | 50 | NoMissingValues, NoBinaryClass, FewInstances | libsvm_svc | 0,898148148 | 0,90172099 | 0,895816036 | 0,896835879 | 0,982296222 | 895,8699269
0 | jannis | Auto-Sklearn | No limits |  | No characteristics | gradient_boosting | 0,711828984 | 0,637715628 | 0,542917286 | 0,559196226 | 0,871582637 | 894,3398745
1 | jannis | Auto-Sklearn | cost <= 0.3 |  | No characteristics | gradient_boosting | 0,711828984 | 0,637715628 | 0,542917286 | 0,559196226 | 0,871582637 | 218,8223712
2 | jannis | Auto-Sklearn | cost <= 0.3 | 35 | NoBinaryClass, NumericClass, NoStringAttributes | gradient_boosting | 0,711828984 | 0,637715628 | 0,542917286 | 0,559196226 | 0,871582637 | 217,144552
3 | jannis | Auto-Sklearn | cost <= 0.3 | 35 | NoBinaryClass, NumericClass, NoStringAttributes | gradient_boosting | 0,711828984 | 0,637715628 | 0,542917286 | 0,559196226 | 0,871582637 | 213,8408523
4 | jannis | Auto-Sklearn | cost <= 0.3 | 35 | NoBinaryClass, NumericClass, NoStringAttributes | gradient_boosting | 0,711828984 | 0,637715628 | 0,542917286 | 0,559196226 | 0,871582637 | 218,9195278
5 | jannis | Auto-Sklearn | cost <= 0.3 | 50 | NoMissingValues, NoBinaryClass, NoFewInstances | gradient_boosting | 0,711828984 | 0,637715628 | 0,542917286 | 0,559196226 | 0,871582637 | 212,5533025
6 | jannis | Auto-Sklearn | cost <= 0.3 | 50 | NoMissingValues, NoBinaryClass, NoFewInstances | gradient_boosting | 0,711828984 | 0,637715628 | 0,542917286 | 0,559196226 | 0,871582637 | 220,5655499
7 | jannis | Auto-Sklearn | cost <= 0.3 | 50 | NoMissingValues, NoBinaryClass, NoFewInstances | gradient_boosting | 0,711828984 | 0,637715628 | 0,542917286 | 0,559196226 | 0,871582637 | 223,5436571
8 | jasmine | Auto-Sklearn | No limits |  | No characteristics | random_forest | 0,809045226 | 0,752688172 | 0,927152318 | 0,830860534 | 0,807643956 | 896,1934564
9 | jasmine | Auto-Sklearn | cost <= 0.18 |  | No characteristics | random_forest | 0,809045226 | 0,752688172 | 0,927152318 | 0,830860534 | 0,807643956 | 899,5594747
10 | jasmine | Auto-Sklearn | cost <= 0.18 | 35 | BinaryClass, BinaryAttributes, NoMissingValues | random_forest | 0,814070352 | 0,75331565 | 0,940397351 | 0,8365243 | 0,812571557 | 61,51595783
11 | jasmine | Auto-Sklearn | cost <= 0.18 | 35 | BinaryClass, BinaryAttributes, NoMissingValues | random_forest | 0,814070352 | 0,75331565 | 0,940397351 | 0,8365243 | 0,812571557 | 61,54915595
12 | jasmine | Auto-Sklearn | cost <= 0.18 | 35 | BinaryClass, BinaryAttributes, NoMissingValues | random_forest | 0,814070352 | 0,75331565 | 0,940397351 | 0,8365243 | 0,812571557 | 65,64574313
13 | jasmine | Auto-Sklearn | cost <= 0.18 | 50 | NoMissingValues, BinaryClass, BinaryAttributes | random_forest | 0,814070352 | 0,75331565 | 0,940397351 | 0,8365243 | 0,812571557 | 62,71027446
14 | jasmine | Auto-Sklearn | cost <= 0.18 | 50 | NoMissingValues, BinaryClass, BinaryAttributes | random_forest | 0,814070352 | 0,75331565 | 0,940397351 | 0,8365243 | 0,812571557 | 62,3464849
15 | jasmine | Auto-Sklearn | cost <= 0.18 | 50 | NoMissingValues, BinaryClass, BinaryAttributes | random_forest | 0,814070352 | 0,75331565 | 0,940397351 | 0,8365243 | 0,812571557 | 63,88123822
16 | kc1 | Auto-Sklearn | No limits |  | No characteristics | lda | 0,869668246 | 0,538461538 | 0,362068966 | 0,432989691 | 0,656309208 | 894,6906374
17 | kc1 | Auto-Sklearn | cost <= 0.15 |  | No characteristics | gradient_boosting | 0,857819905 | 0,480769231 | 0,431034483 | 0,454545455 | 0,678429329 | 184,5235698
18 | kc1 | Auto-Sklearn | cost <= 0.15 | 35 | BinaryClass, NoBinaryAttributes, NoMissingValues | gradient_boosting | 0,857819905 | 0,480769231 | 0,431034483 | 0,454545455 | 0,678429329 | 108,0116971
19 | kc1 | Auto-Sklearn | cost <= 0.15 | 35 | BinaryClass, NoBinaryAttributes, NoMissingValues | gradient_boosting | 0,857819905 | 0,480769231 | 0,431034483 | 0,454545455 | 0,678429329 | 108,199254
20 | kc1 | Auto-Sklearn | cost <= 0.15 | 35 | BinaryClass, NoBinaryAttributes, NoMissingValues | gradient_boosting | 0,857819905 | 0,480769231 | 0,431034483 | 0,454545455 | 0,678429329 | 106,815268
21 | kc1 | Auto-Sklearn | cost <= 0.15 | 50 | NoMissingValues, BinaryClass, NoBinaryAttributes | gradient_boosting | 0,857819905 | 0,480769231 | 0,431034483 | 0,454545455 | 0,678429329 | 106,7479448
22 | kc1 | Auto-Sklearn | cost <= 0.15 | 50 | NoMissingValues, BinaryClass, NoBinaryAttributes | gradient_boosting | 0,857819905 | 0,480769231 | 0,431034483 | 0,454545455 | 0,678429329 | 107,6775546
23 | kc1 | Auto-Sklearn | cost <= 0.15 | 50 | NoMissingValues, BinaryClass, NoBinaryAttributes | gradient_boosting | 0,857819905 | 0,480769231 | 0,431034483 | 0,454545455 | 0,678429329 | 107,4750412
24 | kr-vs-kp | Auto-Sklearn | No limits |  | No characteristics | gradient_boosting | 0,996875 | 1 | 0,994065282 | 0,99702381 | 0,997032641 | 898,9814894
25 | kr-vs-kp | Auto-Sklearn | cost <= 0.01 |  | No characteristics | gradient_boosting | 0,9921875 | 0,994047619 | 0,991097923 | 0,992570579 | 0,992248631 | 228,5266671
26 | kr-vs-kp | Auto-Sklearn | cost <= 0.01 | 35 | BinaryClass, BinaryAttributes, NoMissingValues | libsvm_svc | 0,9921875 | 0,994047619 | 0,991097923 | 0,992570579 | 0,992248631 | 207,1461427
27 | kr-vs-kp | Auto-Sklearn | cost <= 0.01 | 35 | BinaryClass, BinaryAttributes, NoMissingValues | libsvm_svc | 0,9921875 | 0,994047619 | 0,991097923 | 0,992570579 | 0,992248631 | 206,5177133
28 | kr-vs-kp | Auto-Sklearn | cost <= 0.01 | 35 | BinaryClass, BinaryAttributes, NoMissingValues | libsvm_svc | 0,9921875 | 0,994047619 | 0,991097923 | 0,992570579 | 0,992248631 | 205,8431094
29 | kr-vs-kp | Auto-Sklearn | cost <= 0.01 | 50 | NoMissingValues, BinaryClass, BinaryAttributes | libsvm_svc | 0,9921875 | 0,994047619 | 0,991097923 | 0,992570579 | 0,992248631 | 205,193819
30 | kr-vs-kp | Auto-Sklearn | cost <= 0.01 | 50 | NoMissingValues, BinaryClass, BinaryAttributes | libsvm_svc | 0,9921875 | 0,994047619 | 0,991097923 | 0,992570579 | 0,992248631 | 206,5407479
31 | kr-vs-kp | Auto-Sklearn | cost <= 0.01 | 50 | NoMissingValues, BinaryClass, BinaryAttributes | libsvm_svc | 0,9921875 | 0,994047619 | 0,991097923 | 0,992570579 | 0,992248631 | 205,3180377
32 | mfeat-factors | Auto-Sklearn | No limits |  | No characteristics | libsvm_svc | 0,9575 | 0,960733321 | 0,957875383 | 0,958464288 | 0,992229084 | 900,0420675
33 | mfeat-factors | Auto-Sklearn | cost <= 0.03 |  | No characteristics | passive_aggressive | 0,9675 | 0,969433317 | 0,967478558 | 0,968060295 | 0,998683491 | 74,0985992
34 | mfeat-factors | Auto-Sklearn | cost <= 0.03 | 35 | NoBinaryClass, NumericClass, NoStringAttributes | libsvm_svc | 0,9575 | 0,960733321 | 0,957875383 | 0,958464288 | 0,992229084 | 35,93908882
35 | mfeat-factors | Auto-Sklearn | cost <= 0.03 | 35 | NoBinaryClass, NumericClass, NoStringAttributes | libsvm_svc | 0,9575 | 0,960733321 | 0,957875383 | 0,958464288 | 0,992229084 | 36,6635778
36 | mfeat-factors | Auto-Sklearn | cost <= 0.03 | 35 | NoBinaryClass, NumericClass, NoStringAttributes | libsvm_svc | 0,9575 | 0,960733321 | 0,957875383 | 0,958464288 | 0,992229084 | 38,56824875
37 | mfeat-factors | Auto-Sklearn | cost <= 0.03 | 50 | NoMissingValues, NoBinaryClass, FewInstances | libsvm_svc | 0,9575 | 0,960733321 | 0,957875383 | 0,958464288 | 0,992229084 | 37,10251141
38 | mfeat-factors | Auto-Sklearn | cost <= 0.03 | 50 | NoMissingValues, NoBinaryClass, FewInstances | libsvm_svc | 0,9575 | 0,960733321 | 0,957875383 | 0,958464288 | 0,992229084 | 35,94508052
39 | mfeat-factors | Auto-Sklearn | cost <= 0.03 | 50 | NoMissingValues, NoBinaryClass, FewInstances | libsvm_svc | 0,9575 | 0,960733321 | 0,957875383 | 0,958464288 | 0,992229084 | 35,82411599
0 | MiniBooNE | Auto-Sklearn | No limits |  | No characteristics | gradient_boosting | 0,944297082 | 0,897951038 | 0,908222312 | 0,90305747 | 0,933472904 | 894,5549371
1 | MiniBooNE | Auto-Sklearn | cost <= 0.06 |  | No characteristics | gradient_boosting | 0,944297082 | 0,897951038 | 0,908222312 | 0,90305747 | 0,933472904 | 155,2574642
2 | MiniBooNE | Auto-Sklearn | cost <= 0.06 | 35 | BinaryClass, NoBinaryAttributes, NoMissingValues | gradient_boosting | 0,944297082 | 0,897951038 | 0,908222312 | 0,90305747 | 0,933472904 | 100,3745794
3 | MiniBooNE | Auto-Sklearn | cost <= 0.06 | 35 | BinaryClass, NoBinaryAttributes, NoMissingValues | gradient_boosting | 0,944297082 | 0,897951038 | 0,908222312 | 0,90305747 | 0,933472904 | 100,1637616
4 | MiniBooNE | Auto-Sklearn | cost <= 0.06 | 35 | BinaryClass, NoBinaryAttributes, NoMissingValues | gradient_boosting | 0,944297082 | 0,897951038 | 0,908222312 | 0,90305747 | 0,933472904 | 99,70038247
5 | MiniBooNE | Auto-Sklearn | cost <= 0.06 | 50 | NoMissingValues, BinaryClass, NoBinaryAttributes | gradient_boosting | 0,944297082 | 0,897951038 | 0,908222312 | 0,90305747 | 0,933472904 | 103,6750548
6 | MiniBooNE | Auto-Sklearn | cost <= 0.06 | 50 | NoMissingValues, BinaryClass, NoBinaryAttributes | gradient_boosting | 0,944297082 | 0,897951038 | 0,908222312 | 0,90305747 | 0,933472904 | 98,29999852
7 | MiniBooNE | Auto-Sklearn | cost <= 0.06 | 50 | NoMissingValues, BinaryClass, NoBinaryAttributes | gradient_boosting | 0,944297082 | 0,897951038 | 0,908222312 | 0,90305747 | 0,933472904 | 99,27196836
8 | nomao | Auto-Sklearn | No limits |  | No characteristics | gradient_boosting | 0,972871029 | 0,980277722 | 0,982056452 | 0,981166281 | 0,965679028 | 898,7522647
9 | nomao | Auto-Sklearn | cost <= 0.03 |  | No characteristics | gradient_boosting | 0,972871029 | 0,980277722 | 0,982056452 | 0,981166281 | 0,965679028 | 727,325871
10 | nomao | Auto-Sklearn | cost <= 0.03 | 35 | BinaryClass, BinaryAttributes, NoMissingValues | random_forest | 0,963876396 | 0,973277075 | 0,976612903 | 0,974942135 | 0,953903968 | 895,8232579
11 | nomao | Auto-Sklearn | cost <= 0.03 | 35 | BinaryClass, BinaryAttributes, NoMissingValues | random_forest | 0,963876396 | 0,973277075 | 0,976612903 | 0,974942135 | 0,953903968 | 895,8915684
12 | nomao | Auto-Sklearn | cost <= 0.03 | 35 | BinaryClass, BinaryAttributes, NoMissingValues | random_forest | 0,963876396 | 0,973277075 | 0,976612903 | 0,974942135 | 0,953903968 | 895,1908221
13 | nomao | Auto-Sklearn | cost <= 0.03 | 50 | NoMissingValues, BinaryClass, BinaryAttributes | random_forest | 0,963876396 | 0,973277075 | 0,976612903 | 0,974942135 | 0,953903968 | 894,9358537
14 | nomao | Auto-Sklearn | cost <= 0.03 | 50 | NoMissingValues, BinaryClass, BinaryAttributes | random_forest | 0,963876396 | 0,973277075 | 0,976612903 | 0,974942135 | 0,953903968 | 895,5358505
15 | nomao | Auto-Sklearn | cost <= 0.03 | 50 | NoMissingValues, BinaryClass, BinaryAttributes | random_forest | 0,963876396 | 0,973277075 | 0,976612903 | 0,974942135 | 0,953903968 | 895,1017079
16 | credit-g | Auto-Sklearn | No limits |  | No characteristics | random_forest | 0,755 | 0,791139241 | 0,886524823 | 0,836120401 | 0,663601394 | 902,5536523
17 | credit-g | Auto-Sklearn | cost <= 0.25 |  | No characteristics | gradient_boosting | 0,78 | 0,790419162 | 0,936170213 | 0,857142857 | 0,671474937 | 73,17601871
18 | credit-g | Auto-Sklearn | cost <= 0.25 | 35 | BinaryClass, BinaryAttributes, NoMissingValues | random_forest | 0,77 | 0,787878788 | 0,921985816 | 0,849673203 | 0,664382738 | 19,12191582
19 | credit-g | Auto-Sklearn | cost <= 0.25 | 35 | BinaryClass, BinaryAttributes, NoMissingValues | random_forest | 0,77 | 0,787878788 | 0,921985816 | 0,849673203 | 0,664382738 | 19,87905002
20 | credit-g | Auto-Sklearn | cost <= 0.25 | 35 | BinaryClass, BinaryAttributes, NoMissingValues | random_forest | 0,77 | 0,787878788 | 0,921985816 | 0,849673203 | 0,664382738 | 18,1295836
21 | credit-g | Auto-Sklearn | cost <= 0.25 | 50 | NoMissingValues, BinaryClass, BinaryAttributes | random_forest | 0,77 | 0,787878788 | 0,921985816 | 0,849673203 | 0,664382738 | 18,08147264
22 | credit-g | Auto-Sklearn | cost <= 0.25 | 50 | NoMissingValues, BinaryClass, BinaryAttributes | random_forest | 0,77 | 0,787878788 | 0,921985816 | 0,849673203 | 0,664382738 | 19,15249014
23 | credit-g | Auto-Sklearn | cost <= 0.25 | 50 | NoMissingValues, BinaryClass, BinaryAttributes | random_forest | 0,77 | 0,787878788 | 0,921985816 | 0,849673203 | 0,664382738 | 19,16044092
24 | segment | Auto-Sklearn | No limits |  | No characteristics | gradient_boosting | 0,974025974 | 0,973297217 | 0,972027946 | 0,972529715 | 0,998655031 | 902,0215812
25 | segment | Auto-Sklearn | cost <= 0.02 |  | No characteristics | gradient_boosting | 0,974025974 | 0,973297217 | 0,972027946 | 0,972529715 | 0,998655031 | 900,3991137
26 | segment | Auto-Sklearn | cost <= 0.02 | 35 | NoBinaryClass, NoNumericClass, NoManyInstances | gradient_boosting | 0,984848485 | 0,984969056 | 0,984221502 | 0,984560834 | 0,999148492 | 895,3420923
27 | segment | Auto-Sklearn | cost <= 0.02 | 35 | NoBinaryClass, NoNumericClass, NoManyInstances | gradient_boosting | 0,984848485 | 0,984969056 | 0,984221502 | 0,984560834 | 0,999148492 | 895,1076479
28 | segment | Auto-Sklearn | cost <= 0.02 | 35 | NoBinaryClass, NoNumericClass, NoManyInstances | gradient_boosting | 0,984848485 | 0,984969056 | 0,984221502 | 0,984560834 | 0,999148492 | 898,8535852
29 | segment | Auto-Sklearn | cost <= 0.02 | 50 | NoMissingValues, NoBinaryClass, FewInstances | gradient_boosting | 0,984848485 | 0,984969056 | 0,984221502 | 0,984560834 | 0,999292885 | 750,610301
30 | segment | Auto-Sklearn | cost <= 0.02 | 50 | NoMissingValues, NoBinaryClass, FewInstances | gradient_boosting | 0,984848485 | 0,984969056 | 0,984221502 | 0,984560834 | 0,999292885 | 760,6900783
31 | segment | Auto-Sklearn | cost <= 0.02 | 50 | NoMissingValues, NoBinaryClass, FewInstances | gradient_boosting | 0,984848485 | 0,984969056 | 0,984221502 | 0,984560834 | 0,999292885 | 762,7497201
