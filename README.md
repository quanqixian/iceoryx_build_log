Here's a log of the terminal output I got from compiling iceoryx.

In this compilation, I executed these commands below, then the `iceoryx_dds/Mempool.hpp: No such file or directory` error occurred

```shell
git clone https://github.com/eclipse-iceoryx/iceoryx.git
gcc -v
cmake -version
cd iceoryx
./tools/iceoryx_build_test.sh build-all
```

Terminal output during compilation:

```shell
[BEGIN] 2022/5/19 23:32:34
git clone https://github.com/eclipse-iceoryx/iceoryx.git
Cloning into 'iceoryx'...
remote: Enumerating objects: 84360, done.
remote: Counting objects:   0% (1/580)
remote: Counting objects:   1% (6/580)
remote: Counting objects:   2% (12/580)
remote: Counting objects:   3% (18/580)
remote: Counting objects:   4% (24/580)
remote: Counting objects:   5% (29/580)
remote: Counting objects:   6% (35/580)
remote: Counting objects:   7% (41/580)
remote: Counting objects:   8% (47/580)
remote: Counting objects:   9% (53/580)
remote: Counting objects:  10% (58/580)
remote: Counting objects:  11% (64/580)
remote: Counting objects:  12% (70/580)
remote: Counting objects:  13% (76/580)
remote: Counting objects:  14% (82/580)
remote: Counting objects:  15% (87/580)
remote: Counting objects:  16% (93/580)
remote: Counting objects:  17% (99/580)
remote: Counting objects:  18% (105/580)
remote: Counting objects:  19% (111/580)
remote: Counting objects:  20% (116/580)
remote: Counting objects:  21% (122/580)
remote: Counting objects:  22% (128/580)
remote: Counting objects:  23% (134/580)
remote: Counting objects:  24% (140/580)
remote: Counting objects:  25% (145/580)
remote: Counting objects:  26% (151/580)
remote: Counting objects:  27% (157/580)
remote: Counting objects:  28% (163/580)
remote: Counting objects:  29% (169/580)
remote: Counting objects:  30% (174/580)
remote: Counting objects:  31% (180/580)
remote: Counting objects:  32% (186/580)
remote: Counting objects:  33% (192/580)
remote: Counting objects:  34% (198/580)
remote: Counting objects:  35% (203/580)
remote: Counting objects:  36% (209/580)
remote: Counting objects:  37% (215/580)
remote: Counting objects:  38% (221/580)
remote: Counting objects:  39% (227/580)
remote: Counting objects:  40% (232/580)
remote: Counting objects:  41% (238/580)
remote: Counting objects:  42% (244/580)
remote: Counting objects:  43% (250/580)
remote: Counting objects:  44% (256/580)
remote: Counting objects:  45% (261/580)
remote: Counting objects:  46% (267/580)
remote: Counting objects:  47% (273/580)
remote: Counting objects:  48% (279/580)
remote: Counting objects:  49% (285/580)
remote: Counting objects:  50% (290/580)
remote: Counting objects:  51% (296/580)
remote: Counting objects:  52% (302/580)
remote: Counting objects:  53% (308/580)
remote: Counting objects:  54% (314/580)
remote: Counting objects:  55% (319/580)
remote: Counting objects:  56% (325/580)
remote: Counting objects:  57% (331/580)
remote: Counting objects:  58% (337/580)
remote: Counting objects:  59% (343/580)
remote: Counting objects:  60% (348/580)
remote: Counting objects:  61% (354/580)
remote: Counting objects:  62% (360/580)
remote: Counting objects:  63% (366/580)
remote: Counting objects:  64% (372/580)
remote: Counting objects:  65% (377/580)
remote: Counting objects:  66% (383/580)
remote: Counting objects:  67% (389/580)
remote: Counting objects:  68% (395/580)
remote: Counting objects:  69% (401/580)
remote: Counting objects:  70% (406/580)
remote: Counting objects:  71% (412/580)
remote: Counting objects:  72% (418/580)
remote: Counting objects:  73% (424/580)
remote: Counting objects:  74% (430/580)
remote: Counting objects:  75% (435/580)
remote: Counting objects:  76% (441/580)
remote: Counting objects:  77% (447/580)
remote: Counting objects:  78% (453/580)
remote: Counting objects:  79% (459/580)
remote: Counting objects:  80% (464/580)
remote: Counting objects:  81% (470/580)
remote: Counting objects:  82% (476/580)
remote: Counting objects:  83% (482/580)
remote: Counting objects:  84% (488/580)
remote: Counting objects:  85% (493/580)
remote: Counting objects:  86% (499/580)
remote: Counting objects:  87% (505/580)
remote: Counting objects:  88% (511/580)
remote: Counting objects:  89% (517/580)
remote: Counting objects:  90% (522/580)
remote: Counting objects:  91% (528/580)
remote: Counting objects:  92% (534/580)
remote: Counting objects:  93% (540/580)
remote: Counting objects:  94% (546/580)
remote: Counting objects:  95% (551/580)
remote: Counting objects:  96% (557/580)
remote: Counting objects:  97% (563/580)
remote: Counting objects:  98% (569/580)
remote: Counting objects:  99% (575/580)
remote: Counting objects: 100% (580/580)
remote: Counting objects: 100% (580/580), done.
remote: Compressing objects:   0% (1/205)
remote: Compressing objects:   1% (3/205)
remote: Compressing objects:   2% (5/205)
remote: Compressing objects:   3% (7/205)
remote: Compressing objects:   4% (9/205)
remote: Compressing objects:   5% (11/205)
remote: Compressing objects:   6% (13/205)
remote: Compressing objects:   7% (15/205)
remote: Compressing objects:   8% (17/205)
remote: Compressing objects:   9% (19/205)
remote: Compressing objects:  10% (21/205)
remote: Compressing objects:  11% (23/205)
remote: Compressing objects:  12% (25/205)
remote: Compressing objects:  13% (27/205)
remote: Compressing objects:  14% (29/205)
remote: Compressing objects:  15% (31/205)
remote: Compressing objects:  16% (33/205)
remote: Compressing objects:  17% (35/205)
remote: Compressing objects:  18% (37/205)
remote: Compressing objects:  19% (39/205)
remote: Compressing objects:  20% (41/205)
remote: Compressing objects:  21% (44/205)
remote: Compressing objects:  22% (46/205)
remote: Compressing objects:  23% (48/205)
remote: Compressing objects:  24% (50/205)
remote: Compressing objects:  25% (52/205)
remote: Compressing objects:  26% (54/205)
remote: Compressing objects:  27% (56/205)
remote: Compressing objects:  28% (58/205)
remote: Compressing objects:  29% (60/205)
remote: Compressing objects:  30% (62/205)
remote: Compressing objects:  31% (64/205)
remote: Compressing objects:  32% (66/205)
remote: Compressing objects:  33% (68/205)
remote: Compressing objects:  34% (70/205)
remote: Compressing objects:  35% (72/205)
remote: Compressing objects:  36% (74/205)
remote: Compressing objects:  37% (76/205)
remote: Compressing objects:  38% (78/205)
remote: Compressing objects:  39% (80/205)
remote: Compressing objects:  40% (82/205)
remote: Compressing objects:  41% (85/205)
remote: Compressing objects:  42% (87/205)
remote: Compressing objects:  43% (89/205)
remote: Compressing objects:  44% (91/205)
remote: Compressing objects:  45% (93/205)
remote: Compressing objects:  46% (95/205)
remote: Compressing objects:  47% (97/205)
remote: Compressing objects:  48% (99/205)
remote: Compressing objects:  49% (101/205)
remote: Compressing objects:  50% (103/205)
remote: Compressing objects:  51% (105/205)
remote: Compressing objects:  52% (107/205)
remote: Compressing objects:  53% (109/205)
remote: Compressing objects:  54% (111/205)
remote: Compressing objects:  55% (113/205)
remote: Compressing objects:  56% (115/205)
remote: Compressing objects:  57% (117/205)
remote: Compressing objects:  58% (119/205)
remote: Compressing objects:  59% (121/205)
remote: Compressing objects:  60% (123/205)
remote: Compressing objects:  61% (126/205)
remote: Compressing objects:  62% (128/205)
remote: Compressing objects:  63% (130/205)
remote: Compressing objects:  64% (132/205)
remote: Compressing objects:  65% (134/205)
remote: Compressing objects:  66% (136/205)
remote: Compressing objects:  67% (138/205)
remote: Compressing objects:  68% (140/205)
remote: Compressing objects:  69% (142/205)
remote: Compressing objects:  70% (144/205)
remote: Compressing objects:  71% (146/205)
remote: Compressing objects:  72% (148/205)
remote: Compressing objects:  73% (150/205)
remote: Compressing objects:  74% (152/205)
remote: Compressing objects:  75% (154/205)
remote: Compressing objects:  76% (156/205)
remote: Compressing objects:  77% (158/205)
remote: Compressing objects:  78% (160/205)
remote: Compressing objects:  79% (162/205)
remote: Compressing objects:  80% (164/205)
remote: Compressing objects:  81% (167/205)
remote: Compressing objects:  82% (169/205)
remote: Compressing objects:  83% (171/205)
remote: Compressing objects:  84% (173/205)
remote: Compressing objects:  85% (175/205)
remote: Compressing objects:  86% (177/205)
remote: Compressing objects:  87% (179/205)
remote: Compressing objects:  88% (181/205)
remote: Compressing objects:  89% (183/205)
remote: Compressing objects:  90% (185/205)
remote: Compressing objects:  91% (187/205)
remote: Compressing objects:  92% (189/205)
remote: Compressing objects:  93% (191/205)
remote: Compressing objects:  94% (193/205)
remote: Compressing objects:  95% (195/205)
remote: Compressing objects:  96% (197/205)
remote: Compressing objects:  97% (199/205)
remote: Compressing objects:  98% (201/205)
remote: Compressing objects:  99% (203/205)
remote: Compressing objects: 100% (205/205)
remote: Compressing objects: 100% (205/205), done.
Receiving objects:   0% (1/84360)   
Receiving objects:   1% (844/84360)   
Receiving objects:   2% (1688/84360)   
Receiving objects:   3% (2531/84360), 540.01 KiB | 810.00 KiB/s   
Receiving objects:   4% (3375/84360), 540.01 KiB | 810.00 KiB/s   
Receiving objects:   5% (4218/84360), 540.01 KiB | 810.00 KiB/s   
Receiving objects:   6% (5062/84360), 540.01 KiB | 810.00 KiB/s   
Receiving objects:   7% (5906/84360), 540.01 KiB | 810.00 KiB/s   
Receiving objects:   7% (6398/84360), 540.01 KiB | 810.00 KiB/s   
Receiving objects:   8% (6749/84360), 540.01 KiB | 810.00 KiB/s   
Receiving objects:   9% (7593/84360), 540.01 KiB | 810.00 KiB/s   
Receiving objects:  10% (8436/84360), 2.34 MiB | 2.01 MiB/s   
Receiving objects:  11% (9280/84360), 2.34 MiB | 2.01 MiB/s   
Receiving objects:  12% (10124/84360), 2.34 MiB | 2.01 MiB/s   
Receiving objects:  13% (10967/84360), 2.34 MiB | 2.01 MiB/s   
Receiving objects:  14% (11811/84360), 4.34 MiB | 2.53 MiB/s   
Receiving objects:  15% (12654/84360), 4.34 MiB | 2.53 MiB/s   
Receiving objects:  16% (13498/84360), 4.34 MiB | 2.53 MiB/s   
Receiving objects:  17% (14342/84360), 4.34 MiB | 2.53 MiB/s   
Receiving objects:  18% (15185/84360), 4.34 MiB | 2.53 MiB/s   
Receiving objects:  19% (16029/84360), 4.34 MiB | 2.53 MiB/s   
Receiving objects:  19% (16324/84360), 4.34 MiB | 2.53 MiB/s   
Receiving objects:  20% (16872/84360), 4.34 MiB | 2.53 MiB/s   
Receiving objects:  21% (17716/84360), 4.34 MiB | 2.53 MiB/s   
Receiving objects:  22% (18560/84360), 4.34 MiB | 2.53 MiB/s   
Receiving objects:  23% (19403/84360), 6.75 MiB | 3.05 MiB/s   
Receiving objects:  24% (20247/84360), 6.75 MiB | 3.05 MiB/s   
Receiving objects:  25% (21090/84360), 6.75 MiB | 3.05 MiB/s   
Receiving objects:  26% (21934/84360), 6.75 MiB | 3.05 MiB/s   
Receiving objects:  27% (22778/84360), 6.75 MiB | 3.05 MiB/s   
Receiving objects:  28% (23621/84360), 6.75 MiB | 3.05 MiB/s   
Receiving objects:  29% (24465/84360), 6.75 MiB | 3.05 MiB/s   
Receiving objects:  30% (25308/84360), 6.75 MiB | 3.05 MiB/s   
Receiving objects:  31% (26152/84360), 6.75 MiB | 3.05 MiB/s   
Receiving objects:  32% (26996/84360), 6.75 MiB | 3.05 MiB/s   
Receiving objects:  33% (27839/84360), 6.75 MiB | 3.05 MiB/s   
Receiving objects:  34% (28683/84360), 6.75 MiB | 3.05 MiB/s   
Receiving objects:  35% (29526/84360), 6.75 MiB | 3.05 MiB/s   
Receiving objects:  36% (30370/84360), 6.75 MiB | 3.05 MiB/s   
Receiving objects:  37% (31214/84360), 6.75 MiB | 3.05 MiB/s   
Receiving objects:  38% (32057/84360), 6.75 MiB | 3.05 MiB/s   
Receiving objects:  39% (32901/84360), 6.75 MiB | 3.05 MiB/s   
Receiving objects:  40% (33744/84360), 6.75 MiB | 3.05 MiB/s   
Receiving objects:  41% (34588/84360), 6.75 MiB | 3.05 MiB/s   
Receiving objects:  42% (35432/84360), 6.75 MiB | 3.05 MiB/s   
Receiving objects:  43% (36275/84360), 6.75 MiB | 3.05 MiB/s   
Receiving objects:  44% (37119/84360), 6.75 MiB | 3.05 MiB/s   
Receiving objects:  45% (37962/84360), 6.75 MiB | 3.05 MiB/s   
Receiving objects:  46% (38806/84360), 6.75 MiB | 3.05 MiB/s   
Receiving objects:  47% (39650/84360), 6.75 MiB | 3.05 MiB/s   
Receiving objects:  48% (40493/84360), 6.75 MiB | 3.05 MiB/s   
Receiving objects:  49% (41337/84360), 6.75 MiB | 3.05 MiB/s   
Receiving objects:  50% (42180/84360), 6.75 MiB | 3.05 MiB/s   
Receiving objects:  51% (43024/84360), 9.70 MiB | 3.54 MiB/s   
Receiving objects:  52% (43868/84360), 9.70 MiB | 3.54 MiB/s   
Receiving objects:  53% (44711/84360), 9.70 MiB | 3.54 MiB/s   
Receiving objects:  54% (45555/84360), 9.70 MiB | 3.54 MiB/s   
Receiving objects:  55% (46398/84360), 9.70 MiB | 3.54 MiB/s   
Receiving objects:  56% (47242/84360), 9.70 MiB | 3.54 MiB/s   
Receiving objects:  57% (48086/84360), 9.70 MiB | 3.54 MiB/s   
Receiving objects:  58% (48929/84360), 9.70 MiB | 3.54 MiB/s   
Receiving objects:  59% (49773/84360), 9.70 MiB | 3.54 MiB/s   
Receiving objects:  60% (50616/84360), 9.70 MiB | 3.54 MiB/s   
Receiving objects:  61% (51460/84360), 9.70 MiB | 3.54 MiB/s   
Receiving objects:  62% (52304/84360), 9.70 MiB | 3.54 MiB/s   
Receiving objects:  63% (53147/84360), 9.70 MiB | 3.54 MiB/s   
Receiving objects:  64% (53991/84360), 9.70 MiB | 3.54 MiB/s   
Receiving objects:  65% (54834/84360), 9.70 MiB | 3.54 MiB/s   
Receiving objects:  66% (55678/84360), 9.70 MiB | 3.54 MiB/s   
Receiving objects:  67% (56522/84360), 9.70 MiB | 3.54 MiB/s   
Receiving objects:  68% (57365/84360), 9.70 MiB | 3.54 MiB/s   
Receiving objects:  68% (57766/84360), 9.70 MiB | 3.54 MiB/s   
Receiving objects:  69% (58209/84360), 9.70 MiB | 3.54 MiB/s   
Receiving objects:  70% (59052/84360), 9.70 MiB | 3.54 MiB/s   
Receiving objects:  71% (59896/84360), 9.70 MiB | 3.54 MiB/s   
Receiving objects:  72% (60740/84360), 9.70 MiB | 3.54 MiB/s   
Receiving objects:  73% (61583/84360), 9.70 MiB | 3.54 MiB/s   
Receiving objects:  74% (62427/84360), 9.70 MiB | 3.54 MiB/s   
Receiving objects:  75% (63270/84360), 9.70 MiB | 3.54 MiB/s   
Receiving objects:  76% (64114/84360), 9.70 MiB | 3.54 MiB/s   
Receiving objects:  77% (64958/84360), 9.70 MiB | 3.54 MiB/s   
Receiving objects:  78% (65801/84360), 9.70 MiB | 3.54 MiB/s   
Receiving objects:  79% (66645/84360), 9.70 MiB | 3.54 MiB/s   
Receiving objects:  80% (67488/84360), 9.70 MiB | 3.54 MiB/s   
Receiving objects:  81% (68332/84360), 9.70 MiB | 3.54 MiB/s   
Receiving objects:  82% (69176/84360), 9.70 MiB | 3.54 MiB/s   
Receiving objects:  83% (70019/84360), 9.70 MiB | 3.54 MiB/s   
Receiving objects:  84% (70863/84360), 9.70 MiB | 3.54 MiB/s   
Receiving objects:  85% (71706/84360), 9.70 MiB | 3.54 MiB/s   
Receiving objects:  86% (72550/84360), 9.70 MiB | 3.54 MiB/s   
Receiving objects:  87% (73394/84360), 9.70 MiB | 3.54 MiB/s   
Receiving objects:  88% (74237/84360), 13.28 MiB | 4.06 MiB/s   
Receiving objects:  89% (75081/84360), 13.28 MiB | 4.06 MiB/s   
Receiving objects:  90% (75924/84360), 13.28 MiB | 4.06 MiB/s   
Receiving objects:  91% (76768/84360), 13.28 MiB | 4.06 MiB/s   
Receiving objects:  92% (77612/84360), 13.28 MiB | 4.06 MiB/s   
Receiving objects:  93% (78455/84360), 13.28 MiB | 4.06 MiB/s   
Receiving objects:  94% (79299/84360), 13.28 MiB | 4.06 MiB/s   
Receiving objects:  95% (80142/84360), 13.28 MiB | 4.06 MiB/s   
Receiving objects:  96% (80986/84360), 13.28 MiB | 4.06 MiB/s   
Receiving objects:  97% (81830/84360), 13.28 MiB | 4.06 MiB/s   
Receiving objects:  98% (82673/84360), 13.28 MiB | 4.06 MiB/s   
Receiving objects:  99% (83517/84360), 13.28 MiB | 4.06 MiB/s   
remote: Total 84360 (delta 406), reused 449 (delta 334), pack-reused 83780
Receiving objects: 100% (84360/84360), 13.28 MiB | 4.06 MiB/s   
Receiving objects: 100% (84360/84360), 14.38 MiB | 4.00 MiB/s, done.
Resolving deltas:   0% (0/65985)   
Resolving deltas:   1% (663/65985)   
Resolving deltas:   2% (1340/65985)   
Resolving deltas:   3% (1990/65985)   
Resolving deltas:   4% (2641/65985)   
Resolving deltas:   5% (3311/65985)   
Resolving deltas:   6% (3975/65985)   
Resolving deltas:   7% (4622/65985)   
Resolving deltas:   8% (5287/65985)   
Resolving deltas:   9% (5967/65985)   
Resolving deltas:  10% (6599/65985)   
Resolving deltas:  11% (7266/65985)   
Resolving deltas:  12% (7998/65985)   
Resolving deltas:  13% (8582/65985)   
Resolving deltas:  14% (9246/65985)   
Resolving deltas:  15% (9914/65985)   
Resolving deltas:  16% (10590/65985)   
Resolving deltas:  17% (11236/65985)   
Resolving deltas:  18% (11891/65985)   
Resolving deltas:  19% (12541/65985)   
Resolving deltas:  20% (13216/65985)   
Resolving deltas:  21% (13860/65985)   
Resolving deltas:  22% (14523/65985)   
Resolving deltas:  23% (15205/65985)   
Resolving deltas:  24% (15855/65985)   
Resolving deltas:  25% (16508/65985)   
Resolving deltas:  26% (17170/65985)   
Resolving deltas:  27% (17862/65985)   
Resolving deltas:  28% (18511/65985)   
Resolving deltas:  29% (19137/65985)   
Resolving deltas:  30% (19855/65985)   
Resolving deltas:  31% (20482/65985)   
Resolving deltas:  32% (21142/65985)   
Resolving deltas:  33% (21791/65985)   
Resolving deltas:  34% (22461/65985)   
Resolving deltas:  35% (23139/65985)   
Resolving deltas:  36% (23767/65985)   
Resolving deltas:  37% (24421/65985)   
Resolving deltas:  38% (25148/65985)   
Resolving deltas:  39% (25738/65985)   
Resolving deltas:  40% (26403/65985)   
Resolving deltas:  41% (27074/65985)   
Resolving deltas:  42% (27741/65985)   
Resolving deltas:  43% (28377/65985)   
Resolving deltas:  44% (29034/65985)   
Resolving deltas:  45% (29712/65985)   
Resolving deltas:  46% (30421/65985)   
Resolving deltas:  46% (30959/65985)   
Resolving deltas:  47% (31014/65985)   
Resolving deltas:  48% (31706/65985)   
Resolving deltas:  49% (32335/65985)   
Resolving deltas:  50% (33025/65985)   
Resolving deltas:  51% (33653/65985)   
Resolving deltas:  52% (34321/65985)   
Resolving deltas:  53% (34982/65985)   
Resolving deltas:  54% (35689/65985)   
Resolving deltas:  55% (36297/65985)   
Resolving deltas:  56% (36955/65985)   
Resolving deltas:  57% (37649/65985)   
Resolving deltas:  58% (38272/65985)   
Resolving deltas:  59% (39046/65985)   
Resolving deltas:  60% (39592/65985)   
Resolving deltas:  61% (40261/65985)   
Resolving deltas:  62% (41054/65985)   
Resolving deltas:  63% (41575/65985)   
Resolving deltas:  64% (42243/65985)   
Resolving deltas:  65% (42945/65985)   
Resolving deltas:  66% (43555/65985)   
Resolving deltas:  67% (44235/65985)   
Resolving deltas:  68% (45118/65985)   
Resolving deltas:  69% (45715/65985)   
Resolving deltas:  70% (46231/65985)   
Resolving deltas:  71% (46861/65985)   
Resolving deltas:  72% (47550/65985)   
Resolving deltas:  73% (48366/65985)   
Resolving deltas:  74% (48882/65985)   
Resolving deltas:  75% (49537/65985)   
Resolving deltas:  76% (50181/65985)   
Resolving deltas:  77% (50919/65985)   
Resolving deltas:  78% (51469/65985)   
Resolving deltas:  79% (52157/65985)   
Resolving deltas:  80% (52871/65985)   
Resolving deltas:  81% (53458/65985)   
Resolving deltas:  82% (54114/65985)   
Resolving deltas:  83% (54804/65985)   
Resolving deltas:  84% (55532/65985)   
Resolving deltas:  85% (56261/65985)   
Resolving deltas:  86% (56938/65985)   
Resolving deltas:  87% (57409/65985)   
Resolving deltas:  88% (58221/65985)   
Resolving deltas:  89% (58729/65985)   
Resolving deltas:  90% (59426/65985)   
Resolving deltas:  91% (60061/65985)   
Resolving deltas:  92% (60945/65985)   
Resolving deltas:  93% (61441/65985)   
Resolving deltas:  94% (62050/65985)   
Resolving deltas:  95% (62924/65985)   
Resolving deltas:  96% (63397/65985)   
Resolving deltas:  97% (64107/65985)   
Resolving deltas:  98% (64736/65985)   
Resolving deltas:  99% (65332/65985)   
Resolving deltas: 100% (65985/65985)   
Resolving deltas: 100% (65985/65985), done.
quan@iZ2zeeq1jai7e6qn7xqrnuZ:~/gitee/OpenSourceSoftware$ gcc -v
Using built-in specs.
COLLECT_GCC=gcc
COLLECT_LTO_WRAPPER=/usr/lib/gcc/x86_64-linux-gnu/7/lto-wrapper
OFFLOAD_TARGET_NAMES=nvptx-none
OFFLOAD_TARGET_DEFAULT=1
Target: x86_64-linux-gnu
Configured with: ../src/configure -v --with-pkgversion='Ubuntu 7.5.0-3ubuntu1~18.04' --with-bugurl=file:///usr/share/doc/gcc-7/README.Bugs --enable-languages=c,ada,c++,go,brig,d,fortran,objc,obj-c++ --prefix=/usr --with-gcc-major-version-only --program-suffix=-7 --program-prefix=x86_64-linux-gnu- --enable-shared --enable-linker-build-id --libexecdir=/usr/lib --without-included-gettext --enable-threads=posix --libdir=/usr/lib --enable-nls --enable-bootstrap --enable-clocale=gnu --enable-libstdcxx-debug --enable-libstdcxx-time=yes --with-default-libstdcxx-abi=new --enable-gnu-unique-object --disable-vtable-verify --enable-libmpx --enable-plugin --enable-default-pie --with-system-zlib --with-target-system-zlib --enable-objc-gc=auto --enable-multiarch --disable-werror --with-arch-32=i686 --with-abi=m64 --with-multilib-list=m32,m64,mx32 --enable-multilib --with-tune=generic --enable-offload-targets=nvptx-none --without-cuda-driver --enable-checking=release --build=x86_64-linux-gnu --host=x86_64-linux-gnu --target=x86_64-linux-gnu
Thread model: posix
gcc version 7.5.0 (Ubuntu 7.5.0-3ubuntu1~18.04) 
quan@iZ2zeeq1jai7e6qn7xqrnuZ:~/gitee/OpenSourceSoftware$ cmake -version
cmake version 3.23.1

CMake suite maintained and supported by Kitware (kitware.com/cmake).
quan@iZ2zeeq1jai7e6qn7xqrnuZ:~/gitee/OpenSourceSoftware$ cd iceoryx
quan@iZ2zeeq1jai7e6qn7xqrnuZ:~/gitee/OpenSourceSoftware/iceoryx$ ./tools/iceoryx_build_test.sh build-all
 [i] Build complete iceoryx with all extensions and all examples
 [i] Building in /home/quan/gitee/OpenSourceSoftware/iceoryx/build
 [i] Building with 1 jobs
 [i] Preparing build directory
 [i] Current working directory: /home/quan/gitee/OpenSourceSoftware/iceoryx/build
>>>>>> Start building iceoryx package <<<<<<
-- The C compiler identification is GNU 7.5.0
-- The CXX compiler identification is GNU 7.5.0
-- Detecting C compiler ABI info
-- Detecting C compiler ABI info - done
-- Check for working C compiler: /usr/bin/cc - skipped
-- Detecting C compile features
-- Detecting C compile features - done
-- Detecting CXX compiler ABI info
-- Detecting CXX compiler ABI info - done
-- Check for working CXX compiler: /usr/bin/c++ - skipped
-- Detecting CXX compile features
-- Detecting CXX compile features - done
-- Configuring done
-- Generating done
-- Build files have been written to: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/googletest/download
[ 11%] Creating directories for 'googletest'
[ 22%] Performing download step (git clone) for 'googletest'
Cloning into 'src'...
HEAD is now at 703bd9ca Googletest export
[ 33%] Performing update step for 'googletest'
[ 44%] No patch step for 'googletest'
[ 55%] No configure step for 'googletest'
[ 66%] No build step for 'googletest'
[ 77%] No install step for 'googletest'
[ 88%] No test step for 'googletest'
[100%] Completed 'googletest'
[100%] Built target googletest
CMake Deprecation Warning at CMakeLists.txt:4 (cmake_minimum_required):
  Compatibility with CMake < 2.8.12 will be removed from a future version of
  CMake.

  Update the VERSION argument <min> value or use a ...<max> suffix to tell
  CMake that the project does not need compatibility with older versions.


-- The C compiler identification is GNU 7.5.0
-- The CXX compiler identification is GNU 7.5.0
-- Detecting C compiler ABI info
-- Detecting C compiler ABI info - done
-- Check for working C compiler: /usr/bin/cc - skipped
-- Detecting C compile features
-- Detecting C compile features - done
-- Detecting CXX compiler ABI info
-- Detecting CXX compiler ABI info - done
-- Check for working CXX compiler: /usr/bin/c++ - skipped
-- Detecting CXX compile features
-- Detecting CXX compile features - done
CMake Deprecation Warning at googlemock/CMakeLists.txt:45 (cmake_minimum_required):
  Compatibility with CMake < 2.8.12 will be removed from a future version of
  CMake.

  Update the VERSION argument <min> value or use a ...<max> suffix to tell
  CMake that the project does not need compatibility with older versions.


CMake Deprecation Warning at googletest/CMakeLists.txt:56 (cmake_minimum_required):
  Compatibility with CMake < 2.8.12 will be removed from a future version of
  CMake.

  Update the VERSION argument <min> value or use a ...<max> suffix to tell
  CMake that the project does not need compatibility with older versions.


-- Found PythonInterp: /usr/bin/python (found version "2.7.17") 
-- Looking for pthread.h
-- Looking for pthread.h - found
-- Performing Test CMAKE_HAVE_LIBC_PTHREAD
-- Performing Test CMAKE_HAVE_LIBC_PTHREAD - Failed
-- Looking for pthread_create in pthreads
-- Looking for pthread_create in pthreads - not found
-- Looking for pthread_create in pthread
-- Looking for pthread_create in pthread - found
-- Found Threads: TRUE  
-- Configuring done
-- Generating done
-- Build files have been written to: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/googletest/build
[ 12%] Building CXX object googletest/CMakeFiles/gtest.dir/src/gtest-all.cc.o
[ 25%] Linking CXX static library ../lib/libgtest.a
[ 25%] Built target gtest
[ 37%] Building CXX object googlemock/CMakeFiles/gmock.dir/src/gmock-all.cc.o
[ 50%] Linking CXX static library ../lib/libgmock.a
[ 50%] Built target gmock
[ 62%] Building CXX object googlemock/CMakeFiles/gmock_main.dir/src/gmock_main.cc.o
[ 75%] Linking CXX static library ../lib/libgmock_main.a
[ 75%] Built target gmock_main
[ 87%] Building CXX object googletest/CMakeFiles/gtest_main.dir/src/gtest_main.cc.o
[100%] Linking CXX static library ../lib/libgtest_main.a
[100%] Built target gtest_main
Install the project...
-- Install configuration: ""
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gmock
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gmock/internal
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gmock/internal/gmock-port.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gmock/internal/gmock-internal-utils.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gmock/internal/custom
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gmock/internal/custom/gmock-generated-actions.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gmock/internal/custom/gmock-port.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gmock/internal/custom/gmock-generated-actions.h.pump
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gmock/internal/custom/gmock-matchers.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gmock/internal/custom/README.md
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gmock/internal/gmock-pp.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gmock/gmock-spec-builders.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gmock/gmock-generated-actions.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gmock/gmock-generated-actions.h.pump
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gmock/gmock-generated-matchers.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gmock/gmock-actions.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gmock/gmock-generated-function-mockers.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gmock/gmock-more-matchers.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gmock/gmock-matchers.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gmock/gmock-more-actions.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gmock/gmock-function-mocker.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gmock/gmock-generated-function-mockers.h.pump
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gmock/gmock-generated-matchers.h.pump
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gmock/gmock.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gmock/gmock-nice-strict.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gmock/gmock-cardinalities.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/lib/libgmock.a
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/lib/libgmock_main.a
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/lib/pkgconfig/gmock.pc
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/lib/pkgconfig/gmock_main.pc
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/lib/cmake/GTest/GTestTargets.cmake
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/lib/cmake/GTest/GTestTargets-noconfig.cmake
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/lib/cmake/GTest/GTestConfigVersion.cmake
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/lib/cmake/GTest/GTestConfig.cmake
-- Up-to-date: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gtest
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gtest/gtest-message.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gtest/internal
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gtest/internal/gtest-port.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gtest/internal/gtest-type-util.h.pump
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gtest/internal/gtest-filepath.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gtest/internal/gtest-param-util.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gtest/internal/gtest-internal.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gtest/internal/gtest-type-util.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gtest/internal/custom
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gtest/internal/custom/gtest-port.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gtest/internal/custom/gtest.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gtest/internal/custom/gtest-printers.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gtest/internal/custom/README.md
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gtest/internal/gtest-death-test-internal.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gtest/internal/gtest-port-arch.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gtest/internal/gtest-string.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gtest/gtest-spi.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gtest/gtest-matchers.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gtest/gtest.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gtest/gtest-printers.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gtest/gtest-param-test.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gtest/gtest-typed-test.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gtest/gtest_pred_impl.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gtest/gtest-test-part.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gtest/gtest_prod.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/gtest/gtest-death-test.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/lib/libgtest.a
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/lib/libgtest_main.a
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/lib/pkgconfig/gtest.pc
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/lib/pkgconfig/gtest_main.pc
-- Looking for pthread.h
-- Looking for pthread.h - found
-- Performing Test CMAKE_HAVE_LIBC_PTHREAD
-- Performing Test CMAKE_HAVE_LIBC_PTHREAD - Failed
-- Looking for pthread_create in pthreads
-- Looking for pthread_create in pthreads - not found
-- Looking for pthread_create in pthread
-- Looking for pthread_create in pthread - found
-- Found Threads: TRUE  
-- GTest was found, building iceoryx_hoofs_testing enabled.
-- The package 'iceoryx_hoofs_testing' is used in source code version.
-- The package 'iceoryx_hoofs' is used in source code version.
-- Configuring done
-- Generating done
-- Build files have been written to: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/cpptoml/download
[ 11%] Creating directories for 'ext_cpptoml'
[ 22%] Performing download step (git clone) for 'ext_cpptoml'
Cloning into 'src'...
HEAD is now at fededad one-char typo
Submodule 'deps/meta-cmake' (https://github.com/meta-toolkit/meta-cmake.git) registered for path 'deps/meta-cmake'
Cloning into '/home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/cpptoml/src/deps/meta-cmake'...
fatal: unable to access 'https://github.com/meta-toolkit/meta-cmake.git/': gnutls_handshake() failed: The TLS connection was non-properly terminated.
fatal: clone of 'https://github.com/meta-toolkit/meta-cmake.git' into submodule path '/home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/cpptoml/src/deps/meta-cmake' failed
Failed to clone 'deps/meta-cmake'. Retry scheduled
Cloning into '/home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/cpptoml/src/deps/meta-cmake'...
Submodule path 'deps/meta-cmake': checked out 'db7ff976c430a6cb6cbd03ae691be04cfaac0a07'
Submodule path 'deps/meta-cmake': checked out 'db7ff976c430a6cb6cbd03ae691be04cfaac0a07'
[ 33%] Performing update step for 'ext_cpptoml'
[ 44%] No patch step for 'ext_cpptoml'
[ 55%] No configure step for 'ext_cpptoml'
[ 66%] No build step for 'ext_cpptoml'
[ 77%] No install step for 'ext_cpptoml'
[ 88%] No test step for 'ext_cpptoml'
[100%] Completed 'ext_cpptoml'
[100%] Built target ext_cpptoml
-- The C compiler identification is GNU 7.5.0
-- The CXX compiler identification is GNU 7.5.0
-- Detecting C compiler ABI info
-- Detecting C compiler ABI info - done
-- Check for working C compiler: /usr/bin/cc - skipped
-- Detecting C compile features
-- Detecting C compile features - done
-- Detecting CXX compiler ABI info
-- Detecting CXX compiler ABI info - done
-- Check for working CXX compiler: /usr/bin/c++ - skipped
-- Detecting CXX compile features
-- Detecting CXX compile features - done
-- Found Doxygen: /usr/bin/doxygen (found version "1.8.13") found components: doxygen missing components: dot
-- Configuring done
-- Generating done
-- Build files have been written to: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/cpptoml/build
Install the project...
-- Install configuration: ""
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/cpptoml.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/lib/cmake/cpptoml/cpptomlTargets.cmake
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/lib/cmake/cpptoml/cpptomlConfigVersion.cmake
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/lib/cmake/cpptoml/cpptomlConfig.cmake
-- [i] <<<<<<<<<<<<< Start iceoryx_posh configuration: >>>>>>>>>>>>>
-- [i] Using m:n communication!
-- [i] IOX_MAX_PUBLISHERS:512
-- [i] IOX_MAX_SUBSCRIBERS:1024
-- [i] IOX_MAX_INTERFACE_NUMBER:4
-- [i] IOX_MAX_SUBSCRIBERS_PER_PUBLISHER:256
-- [i] IOX_MAX_CHUNKS_ALLOCATED_PER_PUBLISHER_SIMULTANEOUSLY:8
-- [i] IOX_MAX_PUBLISHER_HISTORY:16
-- [i] IOX_MAX_CHUNKS_HELD_PER_SUBSCRIBER_SIMULTANEOUSLY:256
-- [i] <<<<<<<<<<<<<< End iceoryx_posh configuration: >>>>>>>>>>>>>>
-- The package 'iceoryx_posh_testing' is used in source code version.
-- The package 'iceoryx_posh' is used in source code version.
-- Found Curses: /usr/lib/x86_64-linux-gnu/libcurses.so  
-- Configuring done
-- Generating done
CMake Warning:
  Manually-specified variables were not used by the project:

    CMAKE_CXX_FLAGS


-- Build files have been written to: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/cyclonedds/download
[ 11%] Creating directories for 'ext_cyclonedds'
[ 22%] Performing download step (git clone) for 'ext_cyclonedds'
Cloning into 'src'...
fatal: unable to access 'https://github.com/eclipse-cyclonedds/cyclonedds.git/': gnutls_handshake() failed: The TLS connection was non-properly terminated.
Cloning into 'src'...
-- Had to git clone more than once: 2 times.
HEAD is now at d63de72f Bump version to 0.8.2
[ 33%] Performing update step for 'ext_cyclonedds'
[ 44%] No patch step for 'ext_cyclonedds'
[ 55%] No configure step for 'ext_cyclonedds'
[ 66%] No build step for 'ext_cyclonedds'
[ 77%] No install step for 'ext_cyclonedds'
[ 88%] No test step for 'ext_cyclonedds'
[100%] Completed 'ext_cyclonedds'
[100%] Built target ext_cyclonedds
-- The C compiler identification is GNU 7.5.0
-- Detecting C compiler ABI info
-- Detecting C compiler ABI info - done
-- Check for working C compiler: /usr/bin/cc - skipped
-- Detecting C compile features
-- Detecting C compile features - done
-- Setting build type to 'RelWithDebInfo' as none was specified.
-- Linux/MacOS system found, trying to find iceoryx...
-- iceoryx not found, falling back to loopback communication.
-- Found OpenSSL: /usr/lib/x86_64-linux-gnu/libcrypto.so (found version "1.1.1")  
-- Building with OpenSSL support
-- Looking for stdint.h
-- Looking for stdint.h - found
-- Looking for inttypes.h
-- Looking for inttypes.h - found
-- Looking for sys/types.h
-- Looking for sys/types.h - found
-- Looking for stdint.h
-- Looking for stdint.h - found
-- Looking for stddef.h
-- Looking for stddef.h - found
-- Check size of intmax_t
-- Check size of intmax_t - done
-- Looking for stpcpy
-- Looking for stpcpy - found
-- Looking for strlcpy
-- Looking for strlcpy - not found
-- Looking for strlcat
-- Looking for strlcat - not found
-- Performing Test COMPILER_HAS_HIDDEN_VISIBILITY
-- Performing Test COMPILER_HAS_HIDDEN_VISIBILITY - Success
-- Performing Test COMPILER_HAS_HIDDEN_INLINE_VISIBILITY
-- Performing Test COMPILER_HAS_HIDDEN_INLINE_VISIBILITY - Failed
-- Performing Test COMPILER_HAS_DEPRECATED_ATTR
-- Performing Test COMPILER_HAS_DEPRECATED_ATTR - Success
-- Looking for getopt.h
-- Looking for getopt.h - found
-- Looking for pthread.h
-- Looking for pthread.h - found
-- Performing Test CMAKE_HAVE_LIBC_PTHREAD
-- Performing Test CMAKE_HAVE_LIBC_PTHREAD - Failed
-- Looking for pthread_create in pthreads
-- Looking for pthread_create in pthreads - not found
-- Looking for pthread_create in pthread
-- Looking for pthread_create in pthread - found
-- Found Threads: TRUE  
-- Looking for clock_gettime in c
-- Looking for clock_gettime in c - found
-- Found BISON: /usr/bin/bison (found suitable version "3.0.4", minimum required is "3.0.4") 
-- Configuring done
-- Generating done
-- Build files have been written to: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/cyclonedds/build
[  1%] Building C object src/tools/ddsconf/CMakeFiles/ddsconf.dir/ddsconf.c.o
[  1%] Building C object src/tools/ddsconf/CMakeFiles/ddsconf.dir/rnc.c.o
[  2%] Building C object src/tools/ddsconf/CMakeFiles/ddsconf.dir/md.c.o
[  2%] Building C object src/tools/ddsconf/CMakeFiles/ddsconf.dir/xsd.c.o
[  2%] Building C object src/tools/ddsconf/CMakeFiles/ddsconf.dir/defconfig.c.o
[  3%] Building C object src/tools/ddsconf/CMakeFiles/ddsconf.dir/__/__/core/ddsi/src/q_config.c.o
[  3%] Building C object src/tools/ddsconf/CMakeFiles/ddsconf.dir/__/__/ddsrt/src/bswap.c.o
[  3%] Building C object src/tools/ddsconf/CMakeFiles/ddsconf.dir/__/__/ddsrt/src/io.c.o
[  4%] Building C object src/tools/ddsconf/CMakeFiles/ddsconf.dir/__/__/ddsrt/src/log.c.o
[  4%] Building C object src/tools/ddsconf/CMakeFiles/ddsconf.dir/__/__/ddsrt/src/retcode.c.o
[  5%] Building C object src/tools/ddsconf/CMakeFiles/ddsconf.dir/__/__/ddsrt/src/strtod.c.o
[  5%] Building C object src/tools/ddsconf/CMakeFiles/ddsconf.dir/__/__/ddsrt/src/strtol.c.o
[  5%] Building C object src/tools/ddsconf/CMakeFiles/ddsconf.dir/__/__/ddsrt/src/mh3.c.o
[  6%] Building C object src/tools/ddsconf/CMakeFiles/ddsconf.dir/__/__/ddsrt/src/avl.c.o
[  6%] Building C object src/tools/ddsconf/CMakeFiles/ddsconf.dir/__/__/ddsrt/src/environ.c.o
[  7%] Building C object src/tools/ddsconf/CMakeFiles/ddsconf.dir/__/__/ddsrt/src/expand_vars.c.o
[  7%] Building C object src/tools/ddsconf/CMakeFiles/ddsconf.dir/__/__/ddsrt/src/fibheap.c.o
[  7%] Building C object src/tools/ddsconf/CMakeFiles/ddsconf.dir/__/__/ddsrt/src/hopscotch.c.o
[  8%] Building C object src/tools/ddsconf/CMakeFiles/ddsconf.dir/__/__/ddsrt/src/xmlparser.c.o
[  8%] Building C object src/tools/ddsconf/CMakeFiles/ddsconf.dir/__/__/ddsrt/src/circlist.c.o
[  9%] Building C object src/tools/ddsconf/CMakeFiles/ddsconf.dir/__/__/ddsrt/src/atomics.c.o
[  9%] Building C object src/tools/ddsconf/CMakeFiles/ddsconf.dir/__/__/ddsrt/src/cdtors.c.o
[  9%] Building C object src/tools/ddsconf/CMakeFiles/ddsconf.dir/__/__/ddsrt/src/environ/posix/environ.c.o
[ 10%] Building C object src/tools/ddsconf/CMakeFiles/ddsconf.dir/__/__/ddsrt/src/heap/posix/heap.c.o
[ 10%] Building C object src/tools/ddsconf/CMakeFiles/ddsconf.dir/__/__/ddsrt/src/ifaddrs.c.o
[ 11%] Building C object src/tools/ddsconf/CMakeFiles/ddsconf.dir/__/__/ddsrt/src/ifaddrs/posix/ifaddrs.c.o
[ 11%] Building C object src/tools/ddsconf/CMakeFiles/ddsconf.dir/__/__/ddsrt/src/random.c.o
[ 11%] Building C object src/tools/ddsconf/CMakeFiles/ddsconf.dir/__/__/ddsrt/src/random/posix/random.c.o
[ 12%] Building C object src/tools/ddsconf/CMakeFiles/ddsconf.dir/__/__/ddsrt/src/rusage/posix/rusage.c.o
[ 12%] Building C object src/tools/ddsconf/CMakeFiles/ddsconf.dir/__/__/ddsrt/src/sockets.c.o
[ 13%] Building C object src/tools/ddsconf/CMakeFiles/ddsconf.dir/__/__/ddsrt/src/sockets/posix/gethostname.c.o
[ 13%] Building C object src/tools/ddsconf/CMakeFiles/ddsconf.dir/__/__/ddsrt/src/sockets/posix/socket.c.o
[ 13%] Building C object src/tools/ddsconf/CMakeFiles/ddsconf.dir/__/__/ddsrt/src/string.c.o
[ 14%] Building C object src/tools/ddsconf/CMakeFiles/ddsconf.dir/__/__/ddsrt/src/string/posix/strerror.c.o
[ 14%] Building C object src/tools/ddsconf/CMakeFiles/ddsconf.dir/__/__/ddsrt/src/sync/posix/sync.c.o
[ 15%] Building C object src/tools/ddsconf/CMakeFiles/ddsconf.dir/__/__/ddsrt/src/threads.c.o
[ 15%] Building C object src/tools/ddsconf/CMakeFiles/ddsconf.dir/__/__/ddsrt/src/threads/posix/threads.c.o
[ 15%] Building C object src/tools/ddsconf/CMakeFiles/ddsconf.dir/__/__/ddsrt/src/time.c.o
[ 16%] Building C object src/tools/ddsconf/CMakeFiles/ddsconf.dir/__/__/ddsrt/src/time/posix/time.c.o
[ 16%] Building C object src/tools/ddsconf/CMakeFiles/ddsconf.dir/__/__/ddsrt/src/md5.c.o
[ 17%] Building C object src/tools/ddsconf/CMakeFiles/ddsconf.dir/__/__/ddsrt/src/process/posix/process.c.o
[ 17%] Building C object src/tools/ddsconf/CMakeFiles/ddsconf.dir/__/__/ddsrt/src/netstat/linux/netstat.c.o
[ 17%] Building C object src/tools/ddsconf/CMakeFiles/ddsconf.dir/__/__/ddsrt/src/dynlib/posix/dynlib.c.o
[ 18%] Building C object src/tools/ddsconf/CMakeFiles/ddsconf.dir/__/__/ddsrt/src/filesystem/posix/filesystem.c.o
[ 18%] Linking C executable ../../../bin/ddsconf
[ 18%] Built target ddsconf
[ 18%] Generating defconfig.c
[ 19%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/ddsi_eth.c.o
[ 19%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/ddsi_ssl.c.o
[ 20%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/ddsi_tcp.c.o
[ 20%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/ddsi_tran.c.o
[ 20%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/ddsi_udp.c.o
[ 21%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/ddsi_raweth.c.o
[ 21%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/ddsi_vnet.c.o
[ 22%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/ddsi_ipaddr.c.o
[ 22%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/ddsi_mcgroup.c.o
[ 22%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/ddsi_security_util.c.o
[ 23%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/ddsi_security_omg.c.o
[ 23%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/ddsi_portmapping.c.o
[ 24%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/ddsi_handshake.c.o
[ 24%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/ddsi_serdata.c.o
[ 24%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/ddsi_serdata_default.c.o
[ 25%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/ddsi_serdata_pserop.c.o
[ 25%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/ddsi_serdata_plist.c.o
[ 26%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/ddsi_sertype.c.o
[ 26%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/ddsi_sertype_default.c.o
[ 26%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/ddsi_sertype_pserop.c.o
[ 27%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/ddsi_sertype_plist.c.o
[ 27%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/ddsi_sertopic.c.o
[ 27%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/ddsi_statistics.c.o
[ 28%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/ddsi_iid.c.o
[ 28%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/ddsi_tkmap.c.o
[ 29%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/ddsi_vendor.c.o
[ 29%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/ddsi_threadmon.c.o
[ 29%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/ddsi_rhc.c.o
[ 30%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/ddsi_pmd.c.o
[ 30%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/ddsi_entity_index.c.o
[ 31%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/ddsi_deadline.c.o
[ 31%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/ddsi_deliver_locally.c.o
[ 31%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/ddsi_plist.c.o
[ 32%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/ddsi_cdrstream.c.o
[ 32%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/ddsi_time.c.o
[ 33%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/ddsi_ownip.c.o
[ 33%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/ddsi_acknack.c.o
[ 33%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/ddsi_list_genptr.c.o
[ 34%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/ddsi_wraddrset.c.o
[ 34%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/q_addrset.c.o
[ 35%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/q_bitset_inlines.c.o
[ 35%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/q_bswap.c.o
[ 35%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/q_config.c.o
[ 36%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/q_ddsi_discovery.c.o
[ 36%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/q_debmon.c.o
[ 37%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/q_entity.c.o
[ 37%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/q_gc.c.o
[ 37%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/q_init.c.o
[ 38%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/q_lat_estim.c.o
[ 38%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/q_lease.c.o
[ 39%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/q_misc.c.o
[ 39%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/q_pcap.c.o
[ 39%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/q_qosmatch.c.o
[ 40%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/q_radmin.c.o
[ 40%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/q_receive.c.o
[ 41%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/q_sockwaitset.c.o
[ 41%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/q_thread.c.o
[ 41%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/q_transmit.c.o
[ 42%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/q_inverse_uint32_set.c.o
[ 42%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/q_whc.c.o
[ 43%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/q_xevent.c.o
[ 43%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/q_xmsg.c.o
[ 43%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/q_freelist.c.o
[ 44%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/sysdeps.c.o
[ 44%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/ddsi_lifespan.c.o
[ 44%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/ddsi_security_msg.c.o
[ 45%] Building C object src/core/CMakeFiles/ddsc.dir/ddsi/src/ddsi_security_exchange.c.o
[ 45%] Building C object src/core/CMakeFiles/ddsc.dir/defconfig.c.o
[ 46%] Building C object src/core/CMakeFiles/ddsc.dir/ddsc/src/dds_alloc.c.o
[ 46%] Building C object src/core/CMakeFiles/ddsc.dir/ddsc/src/dds_builtin.c.o
[ 46%] Building C object src/core/CMakeFiles/ddsc.dir/ddsc/src/dds_coherent.c.o
[ 47%] Building C object src/core/CMakeFiles/ddsc.dir/ddsc/src/dds_participant.c.o
[ 47%] Building C object src/core/CMakeFiles/ddsc.dir/ddsc/src/dds_reader.c.o
[ 48%] Building C object src/core/CMakeFiles/ddsc.dir/ddsc/src/dds_writer.c.o
[ 48%] Building C object src/core/CMakeFiles/ddsc.dir/ddsc/src/dds_init.c.o
[ 48%] Building C object src/core/CMakeFiles/ddsc.dir/ddsc/src/dds_publisher.c.o
[ 49%] Building C object src/core/CMakeFiles/ddsc.dir/ddsc/src/dds_rhc.c.o
[ 49%] Building C object src/core/CMakeFiles/ddsc.dir/ddsc/src/dds_rhc_default.c.o
[ 50%] Building C object src/core/CMakeFiles/ddsc.dir/ddsc/src/dds_domain.c.o
[ 50%] Building C object src/core/CMakeFiles/ddsc.dir/ddsc/src/dds_instance.c.o
[ 50%] Building C object src/core/CMakeFiles/ddsc.dir/ddsc/src/dds_qos.c.o
[ 51%] Building C object src/core/CMakeFiles/ddsc.dir/ddsc/src/dds_handles.c.o
[ 51%] Building C object src/core/CMakeFiles/ddsc.dir/ddsc/src/dds_entity.c.o
[ 52%] Building C object src/core/CMakeFiles/ddsc.dir/ddsc/src/dds_matched.c.o
[ 52%] Building C object src/core/CMakeFiles/ddsc.dir/ddsc/src/dds_querycond.c.o
[ 52%] Building C object src/core/CMakeFiles/ddsc.dir/ddsc/src/dds_topic.c.o
[ 53%] Building C object src/core/CMakeFiles/ddsc.dir/ddsc/src/dds_listener.c.o
[ 53%] Building C object src/core/CMakeFiles/ddsc.dir/ddsc/src/dds_read.c.o
[ 54%] Building C object src/core/CMakeFiles/ddsc.dir/ddsc/src/dds_waitset.c.o
[ 54%] Building C object src/core/CMakeFiles/ddsc.dir/ddsc/src/dds_readcond.c.o
[ 54%] Building C object src/core/CMakeFiles/ddsc.dir/ddsc/src/dds_guardcond.c.o
[ 55%] Building C object src/core/CMakeFiles/ddsc.dir/ddsc/src/dds_statistics.c.o
[ 55%] Building C object src/core/CMakeFiles/ddsc.dir/ddsc/src/dds_subscriber.c.o
[ 56%] Building C object src/core/CMakeFiles/ddsc.dir/ddsc/src/dds_write.c.o
[ 56%] Building C object src/core/CMakeFiles/ddsc.dir/ddsc/src/dds_whc.c.o
[ 56%] Building C object src/core/CMakeFiles/ddsc.dir/ddsc/src/dds_whc_builtintopic.c.o
[ 57%] Building C object src/core/CMakeFiles/ddsc.dir/ddsc/src/dds_serdata_builtintopic.c.o
[ 57%] Building C object src/core/CMakeFiles/ddsc.dir/ddsc/src/dds_sertype_builtintopic.c.o
[ 58%] Building C object src/core/CMakeFiles/ddsc.dir/ddsc/src/dds_data_allocator.c.o
[ 58%] Building C object src/core/CMakeFiles/ddsc.dir/__/security/core/src/dds_security_serialize.c.o
[ 58%] Building C object src/core/CMakeFiles/ddsc.dir/__/security/core/src/dds_security_utils.c.o
[ 59%] Building C object src/core/CMakeFiles/ddsc.dir/__/security/core/src/dds_security_plugins.c.o
[ 59%] Building C object src/core/CMakeFiles/ddsc.dir/__/security/core/src/shared_secret.c.o
[ 60%] Building C object src/core/CMakeFiles/ddsc.dir/__/security/core/src/dds_security_fsm.c.o
[ 60%] Building C object src/core/CMakeFiles/ddsc.dir/__/security/core/src/dds_security_timed_cb.c.o
[ 60%] Building C object src/core/CMakeFiles/ddsc.dir/__/ddsrt/src/bswap.c.o
[ 61%] Building C object src/core/CMakeFiles/ddsc.dir/__/ddsrt/src/io.c.o
[ 61%] Building C object src/core/CMakeFiles/ddsc.dir/__/ddsrt/src/log.c.o
[ 61%] Building C object src/core/CMakeFiles/ddsc.dir/__/ddsrt/src/retcode.c.o
[ 62%] Building C object src/core/CMakeFiles/ddsc.dir/__/ddsrt/src/strtod.c.o
[ 62%] Building C object src/core/CMakeFiles/ddsc.dir/__/ddsrt/src/strtol.c.o
[ 63%] Building C object src/core/CMakeFiles/ddsc.dir/__/ddsrt/src/mh3.c.o
[ 63%] Building C object src/core/CMakeFiles/ddsc.dir/__/ddsrt/src/avl.c.o
[ 63%] Building C object src/core/CMakeFiles/ddsc.dir/__/ddsrt/src/environ.c.o
[ 64%] Building C object src/core/CMakeFiles/ddsc.dir/__/ddsrt/src/expand_vars.c.o
[ 64%] Building C object src/core/CMakeFiles/ddsc.dir/__/ddsrt/src/fibheap.c.o
[ 65%] Building C object src/core/CMakeFiles/ddsc.dir/__/ddsrt/src/hopscotch.c.o
[ 65%] Building C object src/core/CMakeFiles/ddsc.dir/__/ddsrt/src/xmlparser.c.o
[ 65%] Building C object src/core/CMakeFiles/ddsc.dir/__/ddsrt/src/circlist.c.o
[ 66%] Building C object src/core/CMakeFiles/ddsc.dir/__/ddsrt/src/atomics.c.o
[ 66%] Building C object src/core/CMakeFiles/ddsc.dir/__/ddsrt/src/cdtors.c.o
[ 67%] Building C object src/core/CMakeFiles/ddsc.dir/__/ddsrt/src/environ/posix/environ.c.o
[ 67%] Building C object src/core/CMakeFiles/ddsc.dir/__/ddsrt/src/heap/posix/heap.c.o
[ 67%] Building C object src/core/CMakeFiles/ddsc.dir/__/ddsrt/src/ifaddrs.c.o
[ 68%] Building C object src/core/CMakeFiles/ddsc.dir/__/ddsrt/src/ifaddrs/posix/ifaddrs.c.o
[ 68%] Building C object src/core/CMakeFiles/ddsc.dir/__/ddsrt/src/random.c.o
[ 69%] Building C object src/core/CMakeFiles/ddsc.dir/__/ddsrt/src/random/posix/random.c.o
[ 69%] Building C object src/core/CMakeFiles/ddsc.dir/__/ddsrt/src/rusage/posix/rusage.c.o
[ 69%] Building C object src/core/CMakeFiles/ddsc.dir/__/ddsrt/src/sockets.c.o
[ 70%] Building C object src/core/CMakeFiles/ddsc.dir/__/ddsrt/src/sockets/posix/gethostname.c.o
[ 70%] Building C object src/core/CMakeFiles/ddsc.dir/__/ddsrt/src/sockets/posix/socket.c.o
[ 71%] Building C object src/core/CMakeFiles/ddsc.dir/__/ddsrt/src/string.c.o
[ 71%] Building C object src/core/CMakeFiles/ddsc.dir/__/ddsrt/src/string/posix/strerror.c.o
[ 71%] Building C object src/core/CMakeFiles/ddsc.dir/__/ddsrt/src/sync/posix/sync.c.o
[ 72%] Building C object src/core/CMakeFiles/ddsc.dir/__/ddsrt/src/threads.c.o
[ 72%] Building C object src/core/CMakeFiles/ddsc.dir/__/ddsrt/src/threads/posix/threads.c.o
[ 73%] Building C object src/core/CMakeFiles/ddsc.dir/__/ddsrt/src/time.c.o
[ 73%] Building C object src/core/CMakeFiles/ddsc.dir/__/ddsrt/src/time/posix/time.c.o
[ 73%] Building C object src/core/CMakeFiles/ddsc.dir/__/ddsrt/src/md5.c.o
[ 74%] Building C object src/core/CMakeFiles/ddsc.dir/__/ddsrt/src/process/posix/process.c.o
[ 74%] Building C object src/core/CMakeFiles/ddsc.dir/__/ddsrt/src/netstat/linux/netstat.c.o
[ 75%] Building C object src/core/CMakeFiles/ddsc.dir/__/ddsrt/src/dynlib/posix/dynlib.c.o
[ 75%] Building C object src/core/CMakeFiles/ddsc.dir/__/ddsrt/src/filesystem/posix/filesystem.c.o
[ 75%] Linking C shared library ../../lib/libddsc.so
[ 75%] Built target ddsc
[ 76%] Building C object src/tools/pubsub/CMakeFiles/pubsub.dir/pubsub.c.o
[ 76%] Building C object src/tools/pubsub/CMakeFiles/pubsub.dir/common.c.o
[ 76%] Building C object src/tools/pubsub/CMakeFiles/pubsub.dir/testtype.c.o
[ 77%] Building C object src/tools/pubsub/CMakeFiles/pubsub.dir/porting.c.o
[ 77%] Linking C executable ../../../bin/pubsub
[ 77%] Built target pubsub
[ 77%] Building C object src/tools/idlpp/CMakeFiles/idlpp.dir/src/directive.c.o
[ 78%] Building C object src/tools/idlpp/CMakeFiles/idlpp.dir/src/eval.c.o
[ 78%] Building C object src/tools/idlpp/CMakeFiles/idlpp.dir/src/expand.c.o
[ 79%] Building C object src/tools/idlpp/CMakeFiles/idlpp.dir/src/main.c.o
[ 79%] Building C object src/tools/idlpp/CMakeFiles/idlpp.dir/src/mbchar.c.o
[ 79%] Building C object src/tools/idlpp/CMakeFiles/idlpp.dir/src/support.c.o
[ 80%] Building C object src/tools/idlpp/CMakeFiles/idlpp.dir/src/system.c.o
[ 80%] Linking C static library ../../../lib/libidlpp.a
[ 80%] Built target idlpp
[ 80%] [BISON][parser] Building parser with bison 3.0.4
[ 81%] Building C object src/idl/CMakeFiles/idl.dir/src/symbol.c.o
[ 81%] Building C object src/idl/CMakeFiles/idl.dir/src/directive.c.o
[ 81%] Building C object src/idl/CMakeFiles/idl.dir/src/expression.c.o
[ 82%] Building C object src/idl/CMakeFiles/idl.dir/src/file.c.o
[ 82%] Building C object src/idl/CMakeFiles/idl.dir/src/processor.c.o
[ 83%] Building C object src/idl/CMakeFiles/idl.dir/src/scanner.c.o
[ 83%] Building C object src/idl/CMakeFiles/idl.dir/src/string.c.o
[ 83%] Building C object src/idl/CMakeFiles/idl.dir/src/annotation.c.o
[ 84%] Building C object src/idl/CMakeFiles/idl.dir/src/scope.c.o
[ 84%] Building C object src/idl/CMakeFiles/idl.dir/src/tree.c.o
[ 85%] Building C object src/idl/CMakeFiles/idl.dir/src/visit.c.o
[ 85%] Building C object src/idl/CMakeFiles/idl.dir/src/print.c.o
[ 85%] Building C object src/idl/CMakeFiles/idl.dir/hashid.c.o
[ 86%] Building C object src/idl/CMakeFiles/idl.dir/parser.c.o
[ 86%] Linking C shared library ../../lib/libcycloneddsidl.so
[ 86%] Built target idl
[ 87%] Building C object src/tools/idlc/CMakeFiles/idlc.dir/src/idlc.c.o
[ 87%] Building C object src/tools/idlc/CMakeFiles/idlc.dir/src/plugin.c.o
[ 87%] Building C object src/tools/idlc/CMakeFiles/idlc.dir/src/options.c.o
[ 88%] Building C object src/tools/idlc/CMakeFiles/idlc.dir/src/generator.c.o
[ 88%] Building C object src/tools/idlc/CMakeFiles/idlc.dir/src/descriptor.c.o
[ 89%] Building C object src/tools/idlc/CMakeFiles/idlc.dir/src/types.c.o
[ 89%] Linking C executable ../../../bin/idlc
[ 89%] Built target idlc
[ 90%] Generating ddsperf_types.c, ddsperf_types.h
[ 90%] Built target ddsperf_types_generate
[ 90%] Building C object src/tools/ddsperf/CMakeFiles/ddsperf.dir/ddsperf.c.o
[ 90%] Building C object src/tools/ddsperf/CMakeFiles/ddsperf.dir/cputime.c.o
[ 91%] Building C object src/tools/ddsperf/CMakeFiles/ddsperf.dir/netload.c.o
[ 91%] Building C object src/tools/ddsperf/CMakeFiles/ddsperf.dir/ddsperf_types.c.o
[ 91%] Linking C executable ../../../bin/ddsperf
[ 92%] Built target ddsperf
[ 92%] Building C object src/security/builtin_plugins/access_control/CMakeFiles/dds_security_ac.dir/src/access_control_objects.c.o
[ 92%] Building C object src/security/builtin_plugins/access_control/CMakeFiles/dds_security_ac.dir/src/access_control_parser.c.o
[ 93%] Building C object src/security/builtin_plugins/access_control/CMakeFiles/dds_security_ac.dir/src/access_control_utils.c.o
[ 93%] Building C object src/security/builtin_plugins/access_control/CMakeFiles/dds_security_ac.dir/src/access_control.c.o
[ 93%] Building C object src/security/builtin_plugins/access_control/CMakeFiles/dds_security_ac.dir/__/__/openssl/src/openssl_support.c.o
[ 94%] Linking C shared library ../../../../lib/libdds_security_ac.so
[ 94%] Built target dds_security_ac
[ 94%] Building C object src/security/builtin_plugins/authentication/CMakeFiles/dds_security_auth.dir/src/authentication.c.o
[ 95%] Building C object src/security/builtin_plugins/authentication/CMakeFiles/dds_security_auth.dir/src/auth_utils.c.o
[ 95%] Building C object src/security/builtin_plugins/authentication/CMakeFiles/dds_security_auth.dir/__/__/openssl/src/openssl_support.c.o
[ 95%] Linking C shared library ../../../../lib/libdds_security_auth.so
[ 95%] Built target dds_security_auth
[ 96%] Building C object src/security/builtin_plugins/cryptographic/CMakeFiles/dds_security_crypto.dir/src/crypto_cipher.c.o
[ 96%] Building C object src/security/builtin_plugins/cryptographic/CMakeFiles/dds_security_crypto.dir/src/crypto_key_exchange.c.o
[ 97%] Building C object src/security/builtin_plugins/cryptographic/CMakeFiles/dds_security_crypto.dir/src/crypto_key_factory.c.o
[ 97%] Building C object src/security/builtin_plugins/cryptographic/CMakeFiles/dds_security_crypto.dir/src/crypto_objects.c.o
[ 97%] Building C object src/security/builtin_plugins/cryptographic/CMakeFiles/dds_security_crypto.dir/src/crypto_transform.c.o
[ 98%] Building C object src/security/builtin_plugins/cryptographic/CMakeFiles/dds_security_crypto.dir/src/crypto_utils.c.o
[ 98%] Building C object src/security/builtin_plugins/cryptographic/CMakeFiles/dds_security_crypto.dir/src/cryptography.c.o
[ 99%] Building C object src/security/builtin_plugins/cryptographic/CMakeFiles/dds_security_crypto.dir/__/__/openssl/src/openssl_support.c.o
[ 99%] Linking C shared library ../../../../lib/libdds_security_crypto.so
[ 99%] Built target dds_security_crypto
[100%] Generating cyclonedds.rnc, cyclonedds.xsd, manual/options.md
[100%] Built target schema
Install the project...
-- Install configuration: "RelWithDebInfo"
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/lib/cmake/CycloneDDS/CycloneDDSConfig.cmake
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/lib/cmake/CycloneDDS/CycloneDDSConfigVersion.cmake
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/lib/cmake/CycloneDDS/CycloneDDSTargets.cmake
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/lib/cmake/CycloneDDS/CycloneDDSTargets-relwithdebinfo.cmake
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/bin/pubsub
-- Set runtime path of "/home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/bin/pubsub" to "$ORIGIN/../lib"
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/bin/ddsconf
-- Set runtime path of "/home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/bin/ddsconf" to "$ORIGIN/../lib"
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/idlc
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/idlc/options.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/idlc/generator.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/bin/idlc
-- Set runtime path of "/home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/bin/idlc" to "$ORIGIN/../lib"
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/lib/cmake/CycloneDDS/idlc/Generate.cmake
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/bin/ddsperf
-- Set runtime path of "/home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/bin/ddsperf" to "$ORIGIN/../lib"
-- Up-to-date: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/io.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/environ.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/bswap.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/sockets.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/sockets
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/sockets/posix.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/sockets/windows.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/string.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/misc.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/attributes.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/dynlib.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/process.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/atomics.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/types
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/types/posix.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/types/windows.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/types/vxworks.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/strtod.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/filesystem.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/iovec.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/time.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/xmlparser.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/threads.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/filesystem
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/filesystem/posix.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/filesystem/windows.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/threads
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/threads/posix.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/threads/freertos.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/threads/windows.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/rusage.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/endian.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/hopscotch.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/log.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/fibheap.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/circlist.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/sync.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/static_assert.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/sched.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/retcode.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/sync
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/sync/solaris2.6.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/sync/posix.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/sync/freertos.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/sync/windows.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/arch.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/time
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/time/freertos.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/avl.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/atomics
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/atomics/gcc.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/atomics/arm.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/atomics/msvc.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/atomics/sun.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/types.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/mh3.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/cdtors.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/netstat.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/random.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/strtol.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/heap.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/countargs.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/md5.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/ifaddrs.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsrt/expand_vars.h
-- Up-to-date: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include
-- Up-to-date: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/version.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/idl
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/idl/string.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/idl/attributes.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/idl/print.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/idl/symbol.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/idl/file.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/idl/visit.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/idl/stream.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/idl/retcode.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/idl/tree.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/idl/processor.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/idl/scope.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/idl/expression.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/idl/export.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/idl/version.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/lib/libcycloneddsidl.so.0.8.2
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/lib/libcycloneddsidl.so.0
-- Set runtime path of "/home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/lib/libcycloneddsidl.so.0.8.2" to "$ORIGIN/../lib"
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/lib/libcycloneddsidl.so
-- Up-to-date: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include
-- Up-to-date: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/security
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/security/dds_security_api_authentication.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/security/dds_security_api_types.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/security/dds_security_api.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/security/dds_security_api_access_control.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/security/dds_security_api_cryptography.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/security/dds_security_api_err.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/security/dds_security_api_defs.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/security/core/
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/security/core//dds_security_serialize.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/security/core//dds_security_utils.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/security/core//dds_security_timed_cb.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/security/core//shared_secret.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/security/core//dds_security_types.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/security/core//dds_security_fsm.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/security/core//dds_security_plugins.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/lib/libdds_security_ac.so
-- Set runtime path of "/home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/lib/libdds_security_ac.so" to "$ORIGIN/../lib"
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/lib/libdds_security_auth.so
-- Set runtime path of "/home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/lib/libdds_security_auth.so" to "$ORIGIN/../lib"
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/lib/libdds_security_crypto.so
-- Set runtime path of "/home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/lib/libdds_security_crypto.so" to "$ORIGIN/../lib"
-- Up-to-date: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include
-- Up-to-date: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_builtin_topic_if.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_serdata_plist.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/q_freelist.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_iid.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_acknack.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/q_receive.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/q_xmsg.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_ssl.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_cdrstream.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_statistics.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/q_qosmatch.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_sertopic.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_deadline.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/q_bitset.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/q_config.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/q_protocol.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_ipaddr.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/q_init.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_portmapping.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_domaingv.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/q_inverse_uint32_set.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_security_msg.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_vendor.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_keyhash.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_pmd.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/q_gc.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_security_omg.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/q_transmit.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/q_thread.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/q_log.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_config.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/q_radmin.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/q_rtps.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/shm_sync.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_ownip.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_tcp.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/q_whc.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_mcgroup.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/q_lease.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/q_bswap.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/q_ddsi_discovery.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/q_pcap.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/q_sockwaitset.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_security_util.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_xqos.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_vnet.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_udp.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_serdata_pserop.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_serdata_default.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_lifespan.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_entity_index.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/q_addrset.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_plist.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/q_lat_estim.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_cfgunits.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/q_feature_check.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_typeid.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_guid.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_tran.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_handshake.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_rhc.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_cfgelems.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/q_debmon.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_deliver_locally.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_list_genptr.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_time.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/q_xevent.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_list_tmpl.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/shm_init.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_plist_generic.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/q_hbcontrol.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_security_exchange.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_threadmon.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_serdata.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/q_entity.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/q_unused.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_sertype.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_wraddrset.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/q_misc.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_locator.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_raweth.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/sysdeps.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_tkmap.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsi/ddsi_typelookup.h
-- Up-to-date: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddsc
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddsc/dds.h
-- Up-to-date: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsc
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsc/dds_rhc.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsc/dds_public_qos.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsc/dds_public_qosdefs.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsc/dds_public_listener.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsc/dds_opcodes.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsc/dds_public_impl.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsc/dds_public_alloc.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsc/dds_public_error.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsc/dds_internal_api.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsc/dds_public_status.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsc/dds_statistics.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/ddsc/dds_data_allocator.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/dds.h
-- Up-to-date: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include
-- Up-to-date: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/export.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/dds/features.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/lib/libddsc.so.0.8.2
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/lib/libddsc.so.0
-- Set runtime path of "/home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/lib/libddsc.so.0.8.2" to "$ORIGIN/../lib"
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/lib/libddsc.so
-- Configuring done
-- Generating done
CMake Warning:
  Manually-specified variables were not used by the project:

    CMAKE_CXX_FLAGS


-- Build files have been written to: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/cyclonedds-cxx/download
[ 11%] Creating directories for 'ext_cyclonedds_cxx'
[ 22%] Performing download step (git clone) for 'ext_cyclonedds_cxx'
Cloning into 'src'...
HEAD is now at e466345 Bump version number to 0.8.2
[ 33%] Performing update step for 'ext_cyclonedds_cxx'
[ 44%] No patch step for 'ext_cyclonedds_cxx'
[ 55%] No configure step for 'ext_cyclonedds_cxx'
[ 66%] No build step for 'ext_cyclonedds_cxx'
[ 77%] No install step for 'ext_cyclonedds_cxx'
[ 88%] No test step for 'ext_cyclonedds_cxx'
[100%] Completed 'ext_cyclonedds_cxx'
[100%] Built target ext_cyclonedds_cxx
-- The C compiler identification is GNU 7.5.0
-- The CXX compiler identification is GNU 7.5.0
-- Detecting C compiler ABI info
-- Detecting C compiler ABI info - done
-- Check for working C compiler: /usr/bin/cc - skipped
-- Detecting C compile features
-- Detecting C compile features - done
-- Detecting CXX compiler ABI info
-- Detecting CXX compiler ABI info - done
-- Check for working CXX compiler: /usr/bin/c++ - skipped
-- Detecting CXX compile features
-- Detecting CXX compile features - done
-- Performing Test COMPILER_HAS_HIDDEN_VISIBILITY
-- Performing Test COMPILER_HAS_HIDDEN_VISIBILITY - Success
-- Performing Test COMPILER_HAS_HIDDEN_INLINE_VISIBILITY
-- Performing Test COMPILER_HAS_HIDDEN_INLINE_VISIBILITY - Success
-- Performing Test COMPILER_HAS_DEPRECATED_ATTR
-- Performing Test COMPILER_HAS_DEPRECATED_ATTR - Success
-- Configuring done
-- Generating done
-- Build files have been written to: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/cyclonedds-cxx/build
[  1%] Building C object src/idlcxx/CMakeFiles/idlcxx.dir/src/types.c.o
[  3%] Building C object src/idlcxx/CMakeFiles/idlcxx.dir/src/traits.c.o
[  5%] Building C object src/idlcxx/CMakeFiles/idlcxx.dir/src/streamers.c.o
[  7%] Building C object src/idlcxx/CMakeFiles/idlcxx.dir/src/generator.c.o
[  8%] Linking C shared library ../../lib/libcycloneddsidlcxx.so
[  8%] Built target idlcxx
[ 10%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/dds/core/Duration.cpp.o
[ 12%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/dds/core/Exception.cpp.o
[ 14%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/dds/core/Reference.cpp.o
[ 15%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/dds/core/Time.cpp.o
[ 17%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/dds/core/policy/CorePolicy.cpp.o
[ 19%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/dds/core/status/State.cpp.o
[ 21%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/dds/domain/discovery.cpp.o
[ 22%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/dds/domain/find.cpp.o
[ 24%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/dds/pub/pubdiscovery.cpp.o
[ 26%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/dds/sub/subdiscovery.cpp.o
[ 28%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/dds/sub/subfind.cpp.o
[ 29%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/dds/sub/status/DataState.cpp.o
[ 31%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/org/eclipse/cyclonedds/core/Mutex.cpp.o
[ 33%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/org/eclipse/cyclonedds/core/ObjectDelegate.cpp.o
[ 35%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/org/eclipse/cyclonedds/core/DDScObjectDelegate.cpp.o
[ 36%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/org/eclipse/cyclonedds/core/ObjectSet.cpp.o
[ 38%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/org/eclipse/cyclonedds/core/EntityDelegate.cpp.o
[ 40%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/org/eclipse/cyclonedds/core/ReportUtils.cpp.o
[ 42%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/org/eclipse/cyclonedds/core/ListenerDispatcher.cpp.o
[ 43%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/org/eclipse/cyclonedds/core/InstanceHandleDelegate.cpp.o
[ 45%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/org/eclipse/cyclonedds/core/EntitySet.cpp.o
[ 47%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/org/eclipse/cyclonedds/core/MiscUtils.cpp.o
[ 49%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/org/eclipse/cyclonedds/core/cdr/cdr_stream.cpp.o
[ 50%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/org/eclipse/cyclonedds/core/cond/ConditionDelegate.cpp.o
[ 52%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/org/eclipse/cyclonedds/core/cond/GuardConditionDelegate.cpp.o
[ 54%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/org/eclipse/cyclonedds/core/cond/StatusConditionDelegate.cpp.o
[ 56%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/org/eclipse/cyclonedds/core/cond/WaitSetDelegate.cpp.o
[ 57%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/org/eclipse/cyclonedds/core/policy/PolicyDelegate.cpp.o
[ 59%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/org/eclipse/cyclonedds/domain/Domain.cpp.o
[ 61%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/org/eclipse/cyclonedds/domain/DomainWrap.cpp.o
[ 63%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/org/eclipse/cyclonedds/domain/DomainParticipantDelegate.cpp.o
[ 64%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/org/eclipse/cyclonedds/domain/DomainParticipantRegistry.cpp.o
[ 66%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/org/eclipse/cyclonedds/domain/qos/DomainParticipantQosDelegate.cpp.o
[ 68%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/org/eclipse/cyclonedds/pub/AnyDataWriterDelegate.cpp.o
[ 70%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/org/eclipse/cyclonedds/pub/PublisherDelegate.cpp.o
[ 71%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/org/eclipse/cyclonedds/pub/qos/DataWriterQosDelegate.cpp.o
[ 73%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/org/eclipse/cyclonedds/pub/qos/PublisherQosDelegate.cpp.o
[ 75%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/org/eclipse/cyclonedds/sub/qos/DataReaderQosDelegate.cpp.o
[ 77%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/org/eclipse/cyclonedds/sub/AnyDataReaderDelegate.cpp.o
[ 78%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/org/eclipse/cyclonedds/sub/SubscriberDelegate.cpp.o
[ 80%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/org/eclipse/cyclonedds/sub/BuiltinSubscriberDelegate.cpp.o
[ 82%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/org/eclipse/cyclonedds/sub/QueryDelegate.cpp.o
[ 84%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/org/eclipse/cyclonedds/sub/cond/ReadConditionDelegate.cpp.o
[ 85%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/org/eclipse/cyclonedds/sub/cond/QueryConditionDelegate.cpp.o
[ 87%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/org/eclipse/cyclonedds/sub/qos/SubscriberQosDelegate.cpp.o
[ 89%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/org/eclipse/cyclonedds/topic/find.cpp.o
[ 91%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/org/eclipse/cyclonedds/topic/hash.cpp.o
[ 92%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/org/eclipse/cyclonedds/topic/AnyTopicDelegate.cpp.o
[ 94%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/org/eclipse/cyclonedds/topic/FilterDelegate.cpp.o
[ 96%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/org/eclipse/cyclonedds/topic/TopicDescriptionDelegate.cpp.o
[ 98%] Building CXX object src/ddscxx/CMakeFiles/ddscxx.dir/src/org/eclipse/cyclonedds/topic/qos/TopicQosDelegate.cpp.o
[100%] Linking CXX shared library ../../lib/libddscxx.so
[100%] Built target ddscxx
Install the project...
-- Install configuration: ""
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/lib/cmake/CycloneDDS-CXX/CycloneDDS-CXXConfig.cmake
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/lib/cmake/CycloneDDS-CXX/CycloneDDS-CXXVersion.cmake
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/lib/cmake/CycloneDDS-CXX/CycloneDDS-CXXTargets.cmake
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/lib/cmake/CycloneDDS-CXX/CycloneDDS-CXXTargets-noconfig.cmake
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/lib/libcycloneddsidlcxx.so.0.8.2
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/lib/libcycloneddsidlcxx.so.0
-- Set runtime path of "/home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/lib/libcycloneddsidlcxx.so.0.8.2" to ""
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/lib/libcycloneddsidlcxx.so
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/lib/cmake/CycloneDDS-CXX/idlcxx/Generate.cmake
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/lib/libddscxx.so.0.8.2
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/lib/libddscxx.so.0
-- Set runtime path of "/home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/lib/libddscxx.so.0.8.2" to ""
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/lib/libddscxx.so
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/LICENSE
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/dds.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/SubscriberListener.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/AnyDataReader.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/GenerationCount.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/TDataReader.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/cond
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/cond/ReadCondition.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/cond/TReadCondition.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/cond/TQueryCondition.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/cond/QueryCondition.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/cond/detail
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/cond/detail/TReadConditionImpl.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/cond/detail/ReadCondition.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/cond/detail/TQueryConditionImpl.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/cond/detail/QueryCondition.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/TQuery.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/LoanedSamples.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/Rank.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/TSample.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/TRank.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/discovery.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/qos
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/qos/SubscriberQos.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/qos/detail
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/qos/detail/SubscriberQos.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/qos/detail/DataReaderQos.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/qos/DataReaderQos.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/SharedSamples.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/TCoherentAccess.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/Sample.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/Query.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/Subscriber.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/find.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/SampleRef.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/SampleInfo.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/TSampleRef.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/TSampleInfo.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/AnyDataReaderListener.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/DataReader.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/DataReaderListener.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/CoherentAccess.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/ddssub.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/TSubscriber.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/status
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/status/DataState.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/status/detail
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/status/detail/DataStateImpl.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/TAnyDataReader.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/TGenerationCount.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/detail
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/detail/TRankImpl.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/detail/TDataReaderImpl.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/detail/AnyDataReader.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/detail/TQueryImpl.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/detail/Manipulators.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/detail/TCoherentAccessImpl.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/detail/GenerationCount.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/detail/LoanedSamples.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/detail/TAnyDataReaderImpl.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/detail/SamplesHolder.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/detail/Rank.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/detail/TSampleRefImpl.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/detail/discovery.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/detail/SharedSamples.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/detail/Sample.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/detail/SharedSamplesImpl.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/detail/Query.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/detail/Subscriber.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/detail/find.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/detail/SampleRef.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/detail/SampleInfo.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/detail/LoanedSamplesImpl.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/detail/DataReader.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/detail/TSampleImpl.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/detail/CoherentAccess.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/detail/ddssub.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/detail/TGenerationCountImpl.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/detail/TSampleInfoImpl.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/sub/detail/TSubscriberImpl.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/topic
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/topic/AnyTopic.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/topic/BuiltinTopicKey.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/topic/MultiTopic.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/topic/TopicDescription.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/topic/TBuiltinTopic.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/topic/TBuiltinTopicKey.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/topic/TFilter.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/topic/ddstopic.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/topic/discovery.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/topic/qos
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/topic/qos/TopicQos.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/topic/qos/detail
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/topic/qos/detail/TopicQos.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/topic/TAnyTopic.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/topic/TopicListener.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/topic/Filter.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/topic/find.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/topic/TContentFilteredTopic.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/topic/TTopicDescription.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/topic/TopicInstance.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/topic/Topic.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/topic/BuiltinTopic.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/topic/AnyTopicListener.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/topic/TTopic.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/topic/ContentFilteredTopic.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/topic/TMultiTopic.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/topic/detail
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/topic/detail/AnyTopic.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/topic/detail/BuiltinTopicKey.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/topic/detail/MultiTopic.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/topic/detail/TopicDescription.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/topic/detail/TopicInstanceImpl.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/topic/detail/TAnyTopicImpl.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/topic/detail/ddstopic.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/topic/detail/discovery.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/topic/detail/TBuiltinTopicImpl.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/topic/detail/TContentFilteredTopicImpl.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/topic/detail/TFilterImpl.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/topic/detail/Filter.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/topic/detail/find.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/topic/detail/TTopicImpl.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/topic/detail/Topic.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/topic/detail/BuiltinTopic.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/topic/detail/TTopicDescriptionImpl.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/topic/detail/ContentFilteredTopic.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/topic/detail/TBuiltinTopicKeyImpl.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/topic/TopicTraits.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/domain
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/domain/discovery.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/domain/qos
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/domain/qos/DomainParticipantQos.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/domain/qos/detail
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/domain/qos/detail/DomainParticipantQos.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/domain/find.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/domain/DomainParticipant.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/domain/DomainParticipantListener.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/domain/TDomainParticipant.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/domain/ddsdomain.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/domain/detail
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/domain/detail/TDomainParticipantImpl.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/domain/detail/DomainParticipant.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/domain/detail/ddsdomain.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/TQosProvider.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/conformance.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/InstanceHandle.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/cond
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/cond/GuardCondition.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/cond/TCondition.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/cond/TStatusCondition.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/cond/Condition.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/cond/TGuardCondition.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/cond/TWaitSet.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/cond/StatusCondition.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/cond/WaitSet.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/cond/detail
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/cond/detail/GuardCondition.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/cond/detail/TConditionImpl.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/cond/detail/Condition.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/cond/detail/TGuardConditionImpl.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/cond/detail/StatusCondition.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/cond/detail/WaitSet.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/cond/detail/TStatusConditionImpl.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/cond/detail/TWaitSetImpl.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/xtypes
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/xtypes/TypeProvider.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/xtypes/TDynamicData.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/xtypes/TStructType.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/xtypes/PrimitiveTypes.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/xtypes/UnionCase.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/xtypes/DynamicType.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/xtypes/TDynamicType.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/xtypes/TMemberType.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/xtypes/CollectionTypes.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/xtypes/Annotations.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/xtypes/TAnnotation.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/xtypes/TypeKind.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/xtypes/DynamicData.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/xtypes/StructType.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/xtypes/UnionType.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/xtypes/TCollectionTypes.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/xtypes/TTypeProvider.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/xtypes/MemberType.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/xtypes/detail
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/xtypes/detail/TypeProvider.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/xtypes/detail/Annotation.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/xtypes/detail/PrimitiveTypes.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/xtypes/detail/UnionCase.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/xtypes/detail/DynamicType.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/xtypes/detail/CollectionTypes.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/xtypes/detail/DynamicData.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/xtypes/detail/StructType.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/xtypes/detail/UnionType.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/xtypes/detail/MemberType.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/TEntityQos.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/SafeEnumeration.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/Value.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/Duration.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/Exception.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/array.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/TEntity.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/policy
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/policy/PolicyKind.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/policy/TQosPolicyCount.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/policy/QosPolicyCount.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/policy/CorePolicy.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/policy/TCorePolicy.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/policy/detail
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/policy/detail/TQosPolicyCountImpl.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/policy/detail/TCorePolicyImpl.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/policy/detail/QosPolicyCount.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/policy/detail/CorePolicy.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/TBuiltinTopicTypes.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/Entity.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/WeakReference.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/BuiltinTopicTypes.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/QosProvider.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/Time.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/Reference.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/refmacros.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/macros.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/status
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/status/Status.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/status/State.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/status/TStatus.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/status/detail
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/status/detail/Status.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/status/detail/TStatusImpl.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/ref_traits.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/Optional.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/TInstanceHandle.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/detail
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/detail/TEntityQosImpl.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/detail/conformance.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/detail/InstanceHandle.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/detail/TEntityImpl.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/detail/Value.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/detail/WeakReferenceImpl.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/detail/TInstanceHandleImpl.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/detail/array.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/detail/module_docs.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/detail/Entity.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/detail/BuiltinTopicTypes.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/detail/QosProvider.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/detail/TQosProviderImpl.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/detail/macros.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/detail/ReferenceImpl.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/detail/inttypes.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/detail/ref_traits.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/detail/old_win_stdint.h
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/detail/ddscore.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/ddscore.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/LengthUnlimited.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/types.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/pub
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/pub/PublisherListener.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/pub/Publisher.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/pub/CoherentSet.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/pub/TPublisher.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/pub/AnyDataWriter.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/pub/discovery.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/pub/qos
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/pub/qos/PublisherQos.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/pub/qos/DataWriterQos.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/pub/qos/detail
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/pub/qos/detail/PublisherQos.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/pub/qos/detail/DataWriterQos.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/pub/ddspub.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/pub/find.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/pub/DataWriterListener.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/pub/TCoherentSet.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/pub/DataWriter.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/pub/TSuspendedPublication.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/pub/SuspendedPublication.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/pub/AnyDataWriterListener.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/pub/detail
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/pub/detail/TAnyDataWriterImpl.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/pub/detail/Publisher.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/pub/detail/CoherentSet.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/pub/detail/AnyDataWriter.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/pub/detail/discovery.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/pub/detail/ddspub.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/pub/detail/find.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/pub/detail/TPublisherImpl.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/pub/detail/DataWriter.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/pub/detail/SuspendedPublication.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/pub/detail/DataWriterImpl.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/pub/detail/TCoherentSetImpl.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/pub/detail/TSuspendedPublicationImpl.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/pub/TAnyDataWriter.hpp
-- Up-to-date: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/features.hpp
-- Up-to-date: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core
-- Up-to-date: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/detail
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/dds/core/detail/export.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/sub
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/sub/CoherentAccessDelegate.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/sub/cond
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/sub/cond/QueryConditionDelegate.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/sub/cond/ReadConditionDelegate.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/sub/GenerationCountImpl.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/sub/QueryDelegate.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/sub/AnyDataReaderDelegate.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/sub/RankImpl.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/sub/qos
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/sub/qos/SubscriberQosDelegate.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/sub/qos/DataReaderQosDelegate.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/sub/SampleInfoImpl.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/sub/BuiltinSubscriberDelegate.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/sub/SubscriberDelegate.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/ForwardDeclarations.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/topic
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/topic/BuiltinTopicCopy.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/topic/AnyTopicDelegate.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/topic/TBuiltinTopic.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/topic/FilterDelegate.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/topic/CDRBlob.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/topic/DataRepresentation.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/topic/discovery.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/topic/qos
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/topic/qos/TopicQosDelegate.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/topic/TopicDescriptionDelegate.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/topic/hash.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/topic/BuiltinTopicKeyDelegate.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/topic/TopicListener.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/topic/find.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/topic/datatopic.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/topic/BuiltinTopic.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/topic/BuiltinTopicTraits.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/topic/AnyTopicListener.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/topic/BuiltinTopicDelegate.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/topic/TopicTraits.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/domain
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/domain/DomainWrap.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/domain/qos
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/domain/qos/DomainParticipantQosDelegate.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/domain/DomainParticipantDelegate.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/domain/DomainParticipantRegistry.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/domain/DomainParticipantListener.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/domain/Domain.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/core
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/core/ListenerDispatcher.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/core/ReportUtils.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/core/config.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/core/EntitySet.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/core/ScopedLock.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/core/MiscUtils.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/core/cond
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/core/cond/ShadowParticipant.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/core/cond/GuardConditionDelegate.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/core/cond/WaitSetDelegate.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/core/cond/FunctorHolder.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/core/cond/StatusConditionDelegate.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/core/cond/ConditionDelegate.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/core/TimeHelper.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/core/type_helpers.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/core/ObjectSet.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/core/QosProviderDelegate.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/core/ObjectDelegate.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/core/Missing.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/core/Mutex.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/core/EntityDelegate.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/core/policy
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/core/policy/ProprietaryPolicyKind.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/core/policy/TPolicy.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/core/policy/Policy.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/core/policy/QosPolicyCountDelegate.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/core/policy/PolicyDelegate.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/core/DDScObjectDelegate.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/core/WeakReferenceSet.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/core/status
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/core/status/StatusDelegate.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/core/EntityRegistry.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/core/cdr
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/core/cdr/cdr_stream.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/core/cdr/basic_cdr_ser.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/core/InstanceHandleDelegate.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/pub
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/pub/PublisherDelegate.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/pub/SuspendedPublicationDelegate.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/pub/qos
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/pub/qos/DataWriterQosDelegate.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/pub/qos/PublisherQosDelegate.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/pub/CoherentSetDelegate.hpp
-- Installing: /home/quan/gitee/OpenSourceSoftware/iceoryx/build/dependencies/install/include/ddscxx/org/eclipse/cyclonedds/pub/AnyDataWriterDelegate.hpp
INFO Using CycloneDDS stack
-- [i] <<<<<<<<<<<<< Start iceoryx_posh configuration: >>>>>>>>>>>>>
-- [i] Using m:n communication!
-- [i] IOX_MAX_PUBLISHERS:512
-- [i] IOX_MAX_SUBSCRIBERS:1024
-- [i] IOX_MAX_INTERFACE_NUMBER:4
-- [i] IOX_MAX_SUBSCRIBERS_PER_PUBLISHER:256
-- [i] IOX_MAX_CHUNKS_ALLOCATED_PER_PUBLISHER_SIMULTANEOUSLY:8
-- [i] IOX_MAX_PUBLISHER_HISTORY:16
-- [i] IOX_MAX_CHUNKS_HELD_PER_SUBSCRIBER_SIMULTANEOUSLY:256
-- [i] <<<<<<<<<<<<<< End iceoryx_posh configuration: >>>>>>>>>>>>>>
-- The package 'iceoryx_binding_c' is used in source code version.

       CMake Options
          CMAKE_BUILD_TYPE.....................: Release
          CMAKE_TOOLCHAIN_FILE.................: 
          CMAKE_EXPORT_COMPILE_COMMANDS........: ON

       iceoryx Options
          BINDING_C............................: ON
          BUILD_ALL............................: ON
          BUILD_DOC............................: OFF
          BUILD_SHARED_LIBS....................: OFF
          BUILD_STRICT.........................: OFF
          BUILD_TEST...........................: ON
          CCACHE...............................: ON (ccache not found)
          CLANG_TIDY...........................: OFF
          COVERAGE.............................: OFF
          DDS_GATEWAY..........................: ON
          DOWNLOAD_TOML_LIB....................: ON
          EXAMPLES.............................: ON
          INTROSPECTION........................: ON
          ONE_TO_MANY_ONLY ....................: OFF
          ROUDI_ENVIRONMENT....................: ON (activated by BUILD_TEST=ON)
          SANITIZE.............................: OFF
          TEST_WITH_ADDITIONAL_USER ...........: OFF
          TOML_CONFIG..........................: ON

       Build Properties
          project name..............: iceoryx_package
          c compiler................: /usr/bin/cc
          c++ compiler..............: /usr/bin/c++
          cmake.....................: 3.23.1

-- Configuring done
-- Generating done
-- Build files have been written to: /home/quan/gitee/OpenSourceSoftware/iceoryx/build
[  0%] Building CXX object hoofs/platform/CMakeFiles/iceoryx_platform.dir/linux/source/file.cpp.o
[  0%] Building CXX object hoofs/platform/CMakeFiles/iceoryx_platform.dir/linux/source/fnctl.cpp.o
[  0%] Building CXX object hoofs/platform/CMakeFiles/iceoryx_platform.dir/linux/source/grp.cpp.o
[  0%] Building CXX object hoofs/platform/CMakeFiles/iceoryx_platform.dir/linux/source/mman.cpp.o
[  0%] Building CXX object hoofs/platform/CMakeFiles/iceoryx_platform.dir/linux/source/mqueue.cpp.o
[  1%] Building CXX object hoofs/platform/CMakeFiles/iceoryx_platform.dir/linux/source/socket.cpp.o
[  1%] Building CXX object hoofs/platform/CMakeFiles/iceoryx_platform.dir/linux/source/unistd.cpp.o
[  1%] Linking CXX static library libiceoryx_platform.a
[  1%] Built target iceoryx_platform
[  1%] Building CXX object hoofs/CMakeFiles/iceoryx_hoofs.dir/source/concurrent/active_object.cpp.o
[  1%] Building CXX object hoofs/CMakeFiles/iceoryx_hoofs.dir/source/concurrent/loffli.cpp.o
[  1%] Building CXX object hoofs/CMakeFiles/iceoryx_hoofs.dir/source/cxx/adaptive_wait.cpp.o
[  1%] Building CXX object hoofs/CMakeFiles/iceoryx_hoofs.dir/source/cxx/deadline_timer.cpp.o
[  2%] Building CXX object hoofs/CMakeFiles/iceoryx_hoofs.dir/source/cxx/filesystem.cpp.o
[  2%] Building CXX object hoofs/CMakeFiles/iceoryx_hoofs.dir/source/cxx/generic_raii.cpp.o
[  2%] Building CXX object hoofs/CMakeFiles/iceoryx_hoofs.dir/source/cxx/helplets.cpp.o
[  2%] Building CXX object hoofs/CMakeFiles/iceoryx_hoofs.dir/source/cxx/requires.cpp.o
[  2%] Building CXX object hoofs/CMakeFiles/iceoryx_hoofs.dir/source/cxx/unique_id.cpp.o
[  3%] Building CXX object hoofs/CMakeFiles/iceoryx_hoofs.dir/source/error_handling/error_handler.cpp.o
[  3%] Building CXX object hoofs/CMakeFiles/iceoryx_hoofs.dir/source/error_handling/error_handling.cpp.o
[  3%] Building CXX object hoofs/CMakeFiles/iceoryx_hoofs.dir/source/file_reader/file_reader.cpp.o
[  3%] Building CXX object hoofs/CMakeFiles/iceoryx_hoofs.dir/source/log/hoofs_logging.cpp.o
[  3%] Building CXX object hoofs/CMakeFiles/iceoryx_hoofs.dir/source/log/logcommon.cpp.o
[  3%] Building CXX object hoofs/CMakeFiles/iceoryx_hoofs.dir/source/log/logger.cpp.o
[  4%] Building CXX object hoofs/CMakeFiles/iceoryx_hoofs.dir/source/log/logging_internal.cpp.o
[  4%] Building CXX object hoofs/CMakeFiles/iceoryx_hoofs.dir/source/log/logging.cpp.o
[  4%] Building CXX object hoofs/CMakeFiles/iceoryx_hoofs.dir/source/log/logmanager.cpp.o
[  4%] Building CXX object hoofs/CMakeFiles/iceoryx_hoofs.dir/source/log/logstream.cpp.o
[  4%] Building CXX object hoofs/CMakeFiles/iceoryx_hoofs.dir/source/posix_wrapper/access_control.cpp.o
[  5%] Building CXX object hoofs/CMakeFiles/iceoryx_hoofs.dir/source/posix_wrapper/file_lock.cpp.o
[  5%] Building CXX object hoofs/CMakeFiles/iceoryx_hoofs.dir/source/posix_wrapper/message_queue.cpp.o
[  5%] Building CXX object hoofs/CMakeFiles/iceoryx_hoofs.dir/source/posix_wrapper/mutex.cpp.o
[  5%] Building CXX object hoofs/CMakeFiles/iceoryx_hoofs.dir/source/posix_wrapper/named_pipe.cpp.o
[  5%] Building CXX object hoofs/CMakeFiles/iceoryx_hoofs.dir/source/posix_wrapper/posix_access_rights.cpp.o
[  5%] Building CXX object hoofs/CMakeFiles/iceoryx_hoofs.dir/source/posix_wrapper/semaphore.cpp.o
[  6%] Building CXX object hoofs/CMakeFiles/iceoryx_hoofs.dir/source/posix_wrapper/shared_memory_object.cpp.o
[  6%] Building CXX object hoofs/CMakeFiles/iceoryx_hoofs.dir/source/posix_wrapper/shared_memory_object/allocator.cpp.o
[  6%] Building CXX object hoofs/CMakeFiles/iceoryx_hoofs.dir/source/posix_wrapper/shared_memory_object/memory_map.cpp.o
[  6%] Building CXX object hoofs/CMakeFiles/iceoryx_hoofs.dir/source/posix_wrapper/shared_memory_object/shared_memory.cpp.o
[  6%] Building CXX object hoofs/CMakeFiles/iceoryx_hoofs.dir/source/posix_wrapper/signal_handler.cpp.o
[  7%] Building CXX object hoofs/CMakeFiles/iceoryx_hoofs.dir/source/posix_wrapper/signal_watcher.cpp.o
[  7%] Building CXX object hoofs/CMakeFiles/iceoryx_hoofs.dir/source/posix_wrapper/system_configuration.cpp.o
[  7%] Building CXX object hoofs/CMakeFiles/iceoryx_hoofs.dir/source/posix_wrapper/thread.cpp.o
[  7%] Building CXX object hoofs/CMakeFiles/iceoryx_hoofs.dir/source/posix_wrapper/timer.cpp.o
[  7%] Building CXX object hoofs/CMakeFiles/iceoryx_hoofs.dir/source/posix_wrapper/unix_domain_socket.cpp.o
[  7%] Building CXX object hoofs/CMakeFiles/iceoryx_hoofs.dir/source/relocatable_pointer/base_relative_pointer.cpp.o
[  8%] Building CXX object hoofs/CMakeFiles/iceoryx_hoofs.dir/source/relocatable_pointer/relative_pointer_data.cpp.o
[  8%] Building CXX object hoofs/CMakeFiles/iceoryx_hoofs.dir/source/units/duration.cpp.o
[  8%] Linking CXX static library libiceoryx_hoofs.a
[  8%] Built target iceoryx_hoofs
[  8%] Building CXX object hoofs/testing/CMakeFiles/iceoryx_hoofs_testing.dir/mocks/time_mock.cpp.o
[  8%] Building CXX object hoofs/testing/CMakeFiles/iceoryx_hoofs_testing.dir/mocks/error_handler_mock.cpp.o
[  9%] Building CXX object hoofs/testing/CMakeFiles/iceoryx_hoofs_testing.dir/timing_test.cpp.o
[  9%] Building CXX object hoofs/testing/CMakeFiles/iceoryx_hoofs_testing.dir/compile_test.cpp.o
[  9%] Linking CXX static library libiceoryx_hoofs_testing.a
[  9%] Built target iceoryx_hoofs_testing
[  9%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_access_control.cpp.o
[  9%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_allocator.cpp.o
[  9%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_atomic_relocatable_ptr.cpp.o
[  9%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_concurrent_fifo.cpp.o
[ 10%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_concurrent_loffli.cpp.o
[ 10%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_concurrent_periodic_task.cpp.o
[ 10%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_concurrent_smart_lock.cpp.o
[ 10%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_concurrent_sofi.cpp.o
[ 10%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_concurrent_taco.cpp.o
[ 11%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_concurrent_trigger_queue.cpp.o
[ 11%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_cxx_adaptive_wait.cpp.o
[ 11%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_cxx_algorithm.cpp.o
[ 11%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_cxx_convert.cpp.o
[ 11%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_cxx_deadline_timer.cpp.o
[ 12%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_cxx_expected.cpp.o
[ 12%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_cxx_filesystem.cpp.o
[ 12%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_cxx_forward_list.cpp.o
[ 12%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_cxx_function.cpp.o
[ 12%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_cxx_function_ref.cpp.o
[ 12%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_cxx_functional_interface_and_then.cpp.o
[ 13%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_cxx_functional_interface_common.cpp.o
[ 13%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_cxx_functional_interface_concat_multiple_calls.cpp.o
[ 13%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_cxx_functional_interface_expect.cpp.o
[ 13%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_cxx_functional_interface_or_else.cpp.o
[ 13%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_cxx_functional_interface_types.cpp.o
[ 14%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_cxx_functional_interface_value_or.cpp.o
[ 14%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_cxx_generic_raii.cpp.o
[ 14%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_cxx_helplets.cpp.o
[ 14%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_cxx_list.cpp.o
[ 14%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_cxx_method_callback.cpp.o
[ 14%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_cxx_newtype.cpp.o
[ 15%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_cxx_optional.cpp.o
[ 15%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_cxx_poor_mans_heap.cpp.o
[ 15%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_cxx_reference_counter.cpp.o
[ 15%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_cxx_serialization.cpp.o
[ 15%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_cxx_set.cpp.o
[ 16%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_cxx_stack.cpp.o
[ 16%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_cxx_string.cpp.o
[ 16%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_cxx_type_traits.cpp.o
[ 16%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_cxx_unique_id.cpp.o
[ 16%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_cxx_unique_ptr.cpp.o
[ 16%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_cxx_variant.cpp.o
[ 17%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_cxx_variant_queue.cpp.o
[ 17%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_cxx_vector.cpp.o
[ 17%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_directed_graph.cpp.o
[ 17%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_file_reader.cpp.o
[ 17%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_hoofs_modules.cpp.o
[ 18%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_index_queue.cpp.o
[ 18%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_ipc_channel.cpp.o
[ 18%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_lockfree_queue.cpp.o
[ 18%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_lockfree_queue_buffer.cpp.o
[ 18%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_lockfree_queue_cyclic_index.cpp.o
[ 18%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_logger.cpp.o
[ 19%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_logstream.cpp.o
[ 19%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_objectpool.cpp.o
[ 19%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_posix_access_rights.cpp.o
[ 19%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_posix_file_lock.cpp.o
[ 19%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_posix_mutex.cpp.o
[ 20%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_posix_posix_call.cpp.o
[ 20%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_posix_signal_handler.cpp.o
[ 20%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_posix_signal_watcher.cpp.o
[ 20%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_posix_thread.cpp.o
[ 20%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_posix_timer.cpp.o
[ 21%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_relative_pointer.cpp.o
[ 21%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_relative_pointer_data.cpp.o
[ 21%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_relocatable_ptr.cpp.o
[ 21%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_resizeable_lockfree_queue.cpp.o
[ 21%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_semaphore_module.cpp.o
[ 21%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_shared_memory.cpp.o
[ 22%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_shared_memory_object.cpp.o
[ 22%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_static_storage.cpp.o
[ 22%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_unit_duration.cpp.o
[ 22%] Building CXX object hoofs/test/CMakeFiles/hoofs_moduletests.dir/moduletests/test_unix_domain_sockets.cpp.o
[ 22%] Linking CXX executable hoofs_moduletests
[ 22%] Built target hoofs_moduletests
[ 22%] Building CXX object hoofs/test/CMakeFiles/hoofs_mocktests.dir/mocktests/test_error_handler_mock.cpp.o
[ 23%] Building CXX object hoofs/test/CMakeFiles/hoofs_mocktests.dir/mocktests/test_hoofs_mock.cpp.o
[ 23%] Linking CXX executable hoofs_mocktests
[ 23%] Built target hoofs_mocktests
[ 24%] Building CXX object hoofs/test/CMakeFiles/hoofs_integrationtests.dir/integrationtests/test_hoofs_integration.cpp.o
[ 24%] Building CXX object hoofs/test/CMakeFiles/hoofs_integrationtests.dir/integrationtests/test_lockfree_queue_stresstest.cpp.o
[ 24%] Building CXX object hoofs/test/CMakeFiles/hoofs_integrationtests.dir/integrationtests/test_resizeable_lockfree_queue_stresstest.cpp.o
[ 24%] Linking CXX executable hoofs_integrationtests
[ 24%] Built target hoofs_integrationtests
[ 24%] Building CXX object hoofs/test/CMakeFiles/test_stress_sofi.dir/stresstests/test_stress_sofi.cpp.o
[ 25%] Linking CXX executable test_stress_sofi
[ 25%] Built target test_stress_sofi
[ 25%] Building CXX object hoofs/test/stresstests/benchmark_optional_and_expected/CMakeFiles/iox-bm-optional-and-expected.dir/benchmark_optional_and_expected.cpp.o
[ 25%] Linking CXX executable ../../iox-bm-optional-and-expected
[ 25%] Built target iox-bm-optional-and-expected
[ 25%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/log/posh_logging.cpp.o
[ 25%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/capro/capro_message.cpp.o
[ 26%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/capro/service_description.cpp.o
[ 26%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/error_handling/error_handling.cpp.o
[ 26%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/mepoo/chunk_header.cpp.o
[ 26%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/mepoo/chunk_management.cpp.o
[ 26%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/mepoo/chunk_settings.cpp.o
[ 26%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/mepoo/mepoo_config.cpp.o
[ 27%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/mepoo/segment_config.cpp.o
[ 27%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/mepoo/memory_manager.cpp.o
[ 27%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/mepoo/mem_pool.cpp.o
[ 27%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/mepoo/shared_chunk.cpp.o
[ 27%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/mepoo/shm_safe_unmanaged_chunk.cpp.o
[ 28%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/mepoo/segment_manager.cpp.o
[ 28%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/mepoo/mepoo_segment.cpp.o
[ 28%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/mepoo/memory_info.cpp.o
[ 28%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/popo/ports/interface_port.cpp.o
[ 28%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/popo/ports/interface_port_data.cpp.o
[ 28%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/popo/ports/base_port_data.cpp.o
[ 29%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/popo/ports/base_port.cpp.o
[ 29%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/popo/ports/publisher_port_data.cpp.o
[ 29%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/popo/ports/publisher_port_user.cpp.o
[ 29%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/popo/ports/publisher_port_roudi.cpp.o
[ 29%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/popo/ports/subscriber_port_user.cpp.o
[ 30%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/popo/ports/subscriber_port_roudi.cpp.o
[ 30%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/popo/ports/subscriber_port_single_producer.cpp.o
[ 30%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/popo/ports/subscriber_port_multi_producer.cpp.o
[ 30%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/popo/ports/subscriber_port_data.cpp.o
[ 30%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/popo/ports/client_port_data.cpp.o
[ 30%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/popo/ports/client_port_roudi.cpp.o
[ 31%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/popo/ports/client_port_user.cpp.o
[ 31%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/popo/ports/server_port_data.cpp.o
[ 31%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/popo/ports/server_port_roudi.cpp.o
[ 31%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/popo/ports/server_port_user.cpp.o
[ 31%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/popo/building_blocks/condition_listener.cpp.o
[ 32%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/popo/building_blocks/condition_notifier.cpp.o
[ 32%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/popo/building_blocks/condition_variable_data.cpp.o
[ 32%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/popo/building_blocks/locking_policy.cpp.o
[ 32%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/popo/building_blocks/unique_port_id.cpp.o
[ 32%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/popo/client_options.cpp.o
[ 33%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/popo/listener.cpp.o
[ 33%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/popo/notification_info.cpp.o
[ 33%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/popo/rpc_header.cpp.o
[ 33%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/popo/publisher_options.cpp.o
[ 33%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/popo/server_options.cpp.o
[ 33%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/popo/subscriber_options.cpp.o
[ 34%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/popo/trigger.cpp.o
[ 34%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/popo/trigger_handle.cpp.o
[ 34%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/popo/user_trigger.cpp.o
[ 34%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/version/version_info.cpp.o
[ 34%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/runtime/ipc_interface_base.cpp.o
[ 35%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/runtime/ipc_interface_user.cpp.o
[ 35%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/runtime/ipc_interface_creator.cpp.o
[ 35%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/runtime/ipc_runtime_interface.cpp.o
[ 35%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/runtime/ipc_message.cpp.o
[ 35%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/runtime/port_config_info.cpp.o
[ 35%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/runtime/posh_runtime.cpp.o
[ 36%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/runtime/posh_runtime_impl.cpp.o
[ 36%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/runtime/posh_runtime_single_process.cpp.o
[ 36%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/runtime/service_discovery.cpp.o
[ 36%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/runtime/node.cpp.o
[ 36%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/runtime/node_data.cpp.o
[ 37%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/runtime/node_property.cpp.o
[ 37%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/runtime/shared_memory_user.cpp.o
[ 37%] Building CXX object posh/CMakeFiles/iceoryx_posh.dir/source/roudi/service_registry.cpp.o
[ 37%] Linking CXX static library libiceoryx_posh.a
[ 37%] Built target iceoryx_posh
[ 37%] Building CXX object posh/CMakeFiles/iceoryx_posh_gateway.dir/source/gateway/gateway_base.cpp.o
[ 37%] Linking CXX static library libiceoryx_posh_gateway.a
[ 37%] Built target iceoryx_posh_gateway
[ 38%] Building CXX object posh/CMakeFiles/iceoryx_posh_roudi.dir/source/roudi/application/iceoryx_roudi_app.cpp.o
[ 38%] Building CXX object posh/CMakeFiles/iceoryx_posh_roudi.dir/source/roudi/application/roudi_app.cpp.o
[ 38%] Building CXX object posh/CMakeFiles/iceoryx_posh_roudi.dir/source/roudi/memory/memory_block.cpp.o
[ 38%] Building CXX object posh/CMakeFiles/iceoryx_posh_roudi.dir/source/roudi/memory/memory_provider.cpp.o
[ 38%] Building CXX object posh/CMakeFiles/iceoryx_posh_roudi.dir/source/roudi/memory/mempool_collection_memory_block.cpp.o
[ 39%] Building CXX object posh/CMakeFiles/iceoryx_posh_roudi.dir/source/roudi/memory/mempool_segment_manager_memory_block.cpp.o
[ 39%] Building CXX object posh/CMakeFiles/iceoryx_posh_roudi.dir/source/roudi/memory/port_pool_memory_block.cpp.o
[ 39%] Building CXX object posh/CMakeFiles/iceoryx_posh_roudi.dir/source/roudi/memory/posix_shm_memory_provider.cpp.o
[ 39%] Building CXX object posh/CMakeFiles/iceoryx_posh_roudi.dir/source/roudi/memory/default_roudi_memory.cpp.o
[ 39%] Building CXX object posh/CMakeFiles/iceoryx_posh_roudi.dir/source/roudi/memory/roudi_memory_manager.cpp.o
[ 39%] Building CXX object posh/CMakeFiles/iceoryx_posh_roudi.dir/source/roudi/memory/iceoryx_roudi_memory_manager.cpp.o
[ 40%] Building CXX object posh/CMakeFiles/iceoryx_posh_roudi.dir/source/roudi/port_manager.cpp.o
[ 40%] Building CXX object posh/CMakeFiles/iceoryx_posh_roudi.dir/source/roudi/port_pool.cpp.o
[ 40%] Building CXX object posh/CMakeFiles/iceoryx_posh_roudi.dir/source/roudi/roudi.cpp.o
[ 40%] Building CXX object posh/CMakeFiles/iceoryx_posh_roudi.dir/source/roudi/process.cpp.o
[ 40%] Building CXX object posh/CMakeFiles/iceoryx_posh_roudi.dir/source/roudi/process_manager.cpp.o
[ 41%] Building CXX object posh/CMakeFiles/iceoryx_posh_roudi.dir/source/roudi/iceoryx_roudi_components.cpp.o
[ 41%] Building CXX object posh/CMakeFiles/iceoryx_posh_roudi.dir/source/roudi/roudi_cmd_line_parser.cpp.o
[ 41%] Building CXX object posh/CMakeFiles/iceoryx_posh_roudi.dir/source/roudi/roudi_cmd_line_parser_config_file_option.cpp.o
[ 41%] Building CXX object posh/CMakeFiles/iceoryx_posh_roudi.dir/source/roudi/roudi_config.cpp.o
[ 41%] Linking CXX static library libiceoryx_posh_roudi.a
[ 41%] Built target iceoryx_posh_roudi
[ 41%] Building CXX object posh/CMakeFiles/iceoryx_posh_config.dir/source/log/posh_config_logging.cpp.o
[ 41%] Building CXX object posh/CMakeFiles/iceoryx_posh_config.dir/source/gateway/gateway_config.cpp.o
[ 42%] Building CXX object posh/CMakeFiles/iceoryx_posh_config.dir/source/gateway/toml_gateway_config_parser.cpp.o
[ 42%] Building CXX object posh/CMakeFiles/iceoryx_posh_config.dir/source/roudi/roudi_config_toml_file_provider.cpp.o
[ 42%] Linking CXX static library libiceoryx_posh_config.a
[ 42%] Built target iceoryx_posh_config
[ 42%] Building CXX object posh/CMakeFiles/iox-roudi.dir/source/roudi/application/roudi_main.cpp.o
[ 42%] Linking CXX executable ../iox-roudi
[ 42%] Built target iox-roudi
[ 42%] Building CXX object posh/CMakeFiles/iceoryx_posh_testing.dir/testing/roudi_environment/runtime_test_interface.cpp.o
[ 43%] Building CXX object posh/CMakeFiles/iceoryx_posh_testing.dir/testing/roudi_environment/roudi_environment.cpp.o
[ 43%] Linking CXX static library libiceoryx_posh_testing.a
[ 43%] Built target iceoryx_posh_testing
[ 43%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_base_port.cpp.o
[ 43%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_capro_message.cpp.o
[ 43%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_capro_service.cpp.o
[ 44%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_compatibility_check_level.cpp.o
[ 44%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_fixed_size_container.cpp.o
[ 44%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_gw_channel.cpp.o
[ 44%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_gw_gateway_discovery.cpp.o
[ 44%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_gw_gateway_generic.cpp.o
[ 45%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_mepoo_chunk_header.cpp.o
[ 45%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_mepoo_chunk_settings.cpp.o
[ 45%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_mepoo_config.cpp.o
[ 45%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_mepoo_memory_info.cpp.o
[ 45%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_mepoo_memory_manager.cpp.o
[ 45%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_mepoo_mempool.cpp.o
[ 46%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_mepoo_segment.cpp.o
[ 46%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_mepoo_segment_management.cpp.o
[ 46%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_mepoo_shared_chunk.cpp.o
[ 46%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_mepoo_shared_pointer.cpp.o
[ 46%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_mepoo_shm_safe_unmanaged_chunk.cpp.o
[ 47%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_mepoo_typed_mempool.cpp.o
[ 47%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_monitoringmode_logstream.cpp.o
[ 47%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_mq_message.cpp.o
[ 47%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_popo_base_client.cpp.o
[ 47%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_popo_base_publisher.cpp.o
[ 47%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_popo_base_server.cpp.o
[ 48%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_popo_base_subscriber.cpp.o
[ 48%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_popo_chunk_distributor.cpp.o
[ 48%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_popo_chunk_queue.cpp.o
[ 48%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_popo_chunk_receiver.cpp.o
[ 48%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_popo_chunk_sender.cpp.o
[ 49%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_popo_client.cpp.o
[ 49%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_popo_client_options.cpp.o
[ 49%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_popo_client_port.cpp.o
[ 49%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_popo_condition_variable.cpp.o
[ 49%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_popo_interface_port.cpp.o
[ 49%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_popo_listener.cpp.o
[ 50%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_popo_listener_waitset_attachments.cpp.o
[ 50%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_popo_notification_info.cpp.o
[ 50%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_popo_publisher.cpp.o
[ 50%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_popo_publisher_options.cpp.o
[ 50%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_popo_publisher_port.cpp.o
[ 51%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_popo_request.cpp.o
[ 51%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_popo_response.cpp.o
[ 51%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_popo_rpc_header.cpp.o
[ 51%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_popo_sample.cpp.o
[ 51%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_popo_server.cpp.o
[ 51%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_popo_server_options.cpp.o
[ 52%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_popo_server_port_roudi.cpp.o
[ 52%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_popo_server_port_user.cpp.o
[ 52%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_popo_smart_chunk.cpp.o
[ 52%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_popo_subscriber.cpp.o
[ 52%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_popo_subscriber_options.cpp.o
[ 53%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_popo_subscriber_port.cpp.o
[ 53%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_popo_toml_gateway_config_parser.cpp.o
[ 53%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_popo_trigger.cpp.o
[ 53%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_popo_trigger_handle.cpp.o
[ 53%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_popo_unique_port_id.cpp.o
[ 54%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_popo_untyped_client.cpp.o
[ 54%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_popo_untyped_publisher.cpp.o
[ 54%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_popo_untyped_server.cpp.o
[ 54%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_popo_untyped_subscriber.cpp.o
[ 54%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_popo_used_chunk_list.cpp.o
[ 54%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_popo_user_trigger.cpp.o
[ 55%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_popo_waitset.cpp.o
[ 55%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_posh_modules.cpp.o
[ 55%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_posh_runtime.cpp.o
[ 55%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_posh_runtime_node.cpp.o
[ 55%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_posh_runtime_node_property.cpp.o
[ 56%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_posh_runtime_single_process.cpp.o
[ 56%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_roudi_cmd_line_parser.cpp.o
[ 56%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_roudi_cmd_line_parser_config_file_option.cpp.o
[ 56%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_roudi_config_toml_file_provider.cpp.o
[ 56%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_roudi_generic_memory_block.cpp.o
[ 56%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_roudi_iceoryx_roudi_app.cpp.o
[ 57%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_roudi_iceoyx_roudi_memory_manager.cpp.o
[ 57%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_roudi_memory_block.cpp.o
[ 57%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_roudi_memory_manager.cpp.o
[ 57%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_roudi_memory_provider.cpp.o
[ 57%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_roudi_mempool_introspection.cpp.o
[ 58%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_roudi_port_introspection.cpp.o
[ 58%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_roudi_portmanager.cpp.o
[ 58%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_roudi_portmanager_client_server.cpp.o
[ 58%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_roudi_portpool.cpp.o
[ 58%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_roudi_posix_shm_memory_provider.cpp.o
[ 58%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_roudi_process.cpp.o
[ 59%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_roudi_process_introspection.cpp.o
[ 59%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_roudi_process_manager.cpp.o
[ 59%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_roudi_service_registry.cpp.o
[ 59%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_runtime_ipc_interface_creator.cpp.o
[ 59%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_runtime_port_config_info.cpp.o
[ 60%] Building CXX object posh/test/CMakeFiles/posh_moduletests.dir/moduletests/test_version_info.cpp.o
[ 60%] Linking CXX executable posh_moduletests
[ 60%] Built target posh_moduletests
[ 61%] Building CXX object posh/test/CMakeFiles/posh_integrationtests.dir/integrationtests/test_client_server.cpp.o
[ 61%] Building CXX object posh/test/CMakeFiles/posh_integrationtests.dir/integrationtests/test_interface_port_stack_blowup.cpp.o
[ 61%] Building CXX object posh/test/CMakeFiles/posh_integrationtests.dir/integrationtests/test_mq_interface_startup_race.cpp.o
[ 61%] Building CXX object posh/test/CMakeFiles/posh_integrationtests.dir/integrationtests/test_popo_chunk_building_blocks.cpp.o
[ 61%] Building CXX object posh/test/CMakeFiles/posh_integrationtests.dir/integrationtests/test_popo_port_user_building_blocks.cpp.o
[ 62%] Building CXX object posh/test/CMakeFiles/posh_integrationtests.dir/integrationtests/test_popo_pub_sub_listener.cpp.o
[ 62%] Building CXX object posh/test/CMakeFiles/posh_integrationtests.dir/integrationtests/test_posh_integration.cpp.o
[ 62%] Building CXX object posh/test/CMakeFiles/posh_integrationtests.dir/integrationtests/test_posh_mepoo.cpp.o
[ 62%] Building CXX object posh/test/CMakeFiles/posh_integrationtests.dir/integrationtests/test_publisher_subscriber_communication.cpp.o
[ 62%] Building CXX object posh/test/CMakeFiles/posh_integrationtests.dir/integrationtests/test_roudi_roudi_environment.cpp.o
[ 62%] Building CXX object posh/test/CMakeFiles/posh_integrationtests.dir/integrationtests/test_service_discovery.cpp.o
[ 63%] Building CXX object posh/test/CMakeFiles/posh_integrationtests.dir/integrationtests/test_shm_sigbus_handler.cpp.o
[ 63%] Linking CXX executable posh_integrationtests
[ 63%] Built target posh_integrationtests
[ 63%] Building CXX object iceoryx_introspection/CMakeFiles/iceoryx_introspection.dir/source/iceoryx_introspection_app.cpp.o
[ 63%] Building CXX object iceoryx_introspection/CMakeFiles/iceoryx_introspection.dir/source/introspection_app.cpp.o
[ 64%] Linking CXX static library libiceoryx_introspection.a
[ 64%] Built target iceoryx_introspection
[ 64%] Building CXX object iceoryx_introspection/CMakeFiles/iox-introspection-client.dir/source/introspection_main.cpp.o
[ 64%] Linking CXX executable ../iox-introspection-client
[ 64%] Built target iox-introspection-client
[ 64%] Building CXX object iceoryx_dds/CMakeFiles/iceoryx_dds.dir/source/iceoryx_dds/log/logging.cpp.o
[ 64%] Building CXX object iceoryx_dds/CMakeFiles/iceoryx_dds.dir/source/iceoryx_dds/dds/cyclone_context.cpp.o
[ 64%] Building CXX object iceoryx_dds/CMakeFiles/iceoryx_dds.dir/source/iceoryx_dds/dds/cyclone_data_reader.cpp.o
In file included from /home/quan/gitee/OpenSourceSoftware/iceoryx/iceoryx_dds/source/iceoryx_dds/dds/cyclone_data_reader.cpp:18:0:
/home/quan/gitee/OpenSourceSoftware/iceoryx/iceoryx_dds/include/iceoryx_dds/dds/cyclone_data_reader.hpp:21:10: fatal error: iceoryx_dds/Mempool.hpp: No such file or directory
 #include "iceoryx_dds/Mempool.hpp"
          ^~~~~~~~~~~~~~~~~~~~~~~~~
compilation terminated.
iceoryx_dds/CMakeFiles/iceoryx_dds.dir/build.make:103: recipe for target 'iceoryx_dds/CMakeFiles/iceoryx_dds.dir/source/iceoryx_dds/dds/cyclone_data_reader.cpp.o' failed
make[2]: *** [iceoryx_dds/CMakeFiles/iceoryx_dds.dir/source/iceoryx_dds/dds/cyclone_data_reader.cpp.o] Error 1
CMakeFiles/Makefile2:1444: recipe for target 'iceoryx_dds/CMakeFiles/iceoryx_dds.dir/all' failed
make[1]: *** [iceoryx_dds/CMakeFiles/iceoryx_dds.dir/all] Error 2
Makefile:155: recipe for target 'all' failed
make: *** [all] Error 2
quan@iZ2zeeq1jai7e6qn7xqrnuZ:~/gitee/OpenSourceSoftware/iceoryx$ 
quan@iZ2zeeq1jai7e6qn7xqrnuZ:~/gitee/OpenSourceSoftware/iceoryx$ find ./ -name Mempool.hpp
quan@iZ2zeeq1jai7e6qn7xqrnuZ:~/gitee/OpenSourceSoftware/iceoryx$ 
[END] 2022/5/20 0:01:51

```

However, the Mempool.hpp file was not generated, causing this error
