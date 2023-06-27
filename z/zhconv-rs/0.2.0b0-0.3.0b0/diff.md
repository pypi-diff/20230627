# Comparing `tmp/zhconv_rs-0.2.0b0.tar.gz` & `tmp/zhconv_rs-0.3.0b0.tar.gz`

## Comparing `zhconv_rs-0.2.0b0.tar` & `zhconv_rs-0.3.0b0.tar`

### file list

```diff
@@ -1,474 +1,477 @@
--rw-r--r--   0        0        0     1728 1970-01-01 00:00:00.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/Cargo.toml
--rw-r--r--   0     1001      123      426 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/.gitattributes
--rw-r--r--   0     1001      123     1775 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/.github/workflows/main.yml
--rw-r--r--   0     1001      123     2445 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/.github/workflows/npm.yml
--rw-r--r--   0     1001      123     1973 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/.github/workflows/pyo3.yml
--rw-r--r--   0     1001      123     2703 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/.github/workflows/release.yml
--rw-r--r--   0     1001      123       20 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/.gitignore
--rw-r--r--   0     1001      123    35149 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/LICENSE
--rw-r--r--   0     1001      123    10364 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/README.md
--rw-r--r--   0     1001      123   284864 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/benches/25328-0.txt
--rw-r--r--   0     1001      123      198 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/benches/LICENSE.md
--rw-r--r--   0     1001      123  3261912 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/benches/data3185k.txt
--rw-r--r--   0     1001      123    55192 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/benches/data54k.txt
--rw-r--r--   0     1001      123   705845 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/benches/data689k.txt
--rw-r--r--   0     1001      123     4638 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/benches/zhconv_benchmark.rs
--rw-r--r--   0     1001      123    14233 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/build.rs
--rw-r--r--   0     1001      123      532 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/HKVariants.txt
--rw-r--r--   0     1001      123     2709 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/HKVariantsRevPhrases.txt
--rw-r--r--   0     1001      123      870 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/README.md
--rw-r--r--   0     1001      123    34353 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/STCharacters.txt
--rw-r--r--   0     1001      123  1004153 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/STPhrases.txt
--rw-r--r--   0     1001      123    34627 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/TSCharacters.txt
--rw-r--r--   0     1001      123     5161 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/TSPhrases.txt
--rw-r--r--   0     1001      123     7611 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/TWPhrasesIT.txt
--rw-r--r--   0     1001      123     2121 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/TWPhrasesName.txt
--rw-r--r--   0     1001      123      571 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/TWPhrasesOther.txt
--rw-r--r--   0     1001      123      312 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/TWVariants.txt
--rw-r--r--   0     1001      123     1075 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/TWVariantsRevPhrases.txt
--rw-r--r--   0     1001      123   447718 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/ZhConversion.php
--rw-r--r--   0     1001      123     7470 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/1D.json
--rw-r--r--   0     1001      123     4660 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/2016年太平洋颱風季.json
--rw-r--r--   0     1001      123     4462 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/2017年太平洋颱風季.json
--rw-r--r--   0     1001      123     4953 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/2018年太平洋颱風季.json
--rw-r--r--   0     1001      123     4967 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/2019年太平洋颱風季.json
--rw-r--r--   0     1001      123     4150 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/2020年太平洋颱風季.json
--rw-r--r--   0     1001      123     3977 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/2021年太平洋颱風季.json
--rw-r--r--   0     1001      123     4396 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/2022年太平洋颱風季.json
--rw-r--r--   0     1001      123      311 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/2023年太平洋颱風季.json
--rw-r--r--   0     1001      123    18639 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/24.json
--rw-r--r--   0     1001      123     1347 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/A Pink.json
--rw-r--r--   0     1001      123     1436 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/A Song of Ice and Fire.json
--rw-r--r--   0     1001      123     4784 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/ACmilan.json
--rw-r--r--   0     1001      123     4078 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/ALeague.json
--rw-r--r--   0     1001      123    12349 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/AT Places.json
--rw-r--r--   0     1001      123    12270 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/AU Places.json
--rw-r--r--   0     1001      123     2618 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Adventure Time.json
--rw-r--r--   0     1001      123    24747 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Aero.json
--rw-r--r--   0     1001      123     4785 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Aikatsu.json
--rw-r--r--   0     1001      123    44770 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Anime.json
--rw-r--r--   0     1001      123    11339 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Apple.json
--rw-r--r--   0     1001      123     6426 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Aquatics.json
--rw-r--r--   0     1001      123     3127 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Ariana Grande.json
--rw-r--r--   0     1001      123      682 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Artist.json
--rw-r--r--   0     1001      123    11447 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Astronomy.json
--rw-r--r--   0     1001      123     4837 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Avatar.json
--rw-r--r--   0     1001      123     3325 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Avril Lavigne.json
--rw-r--r--   0     1001      123    46163 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/BE Places.json
--rw-r--r--   0     1001      123    11395 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/BUDDYCOMPLEX.json
--rw-r--r--   0     1001      123    10696 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Badminton.json
--rw-r--r--   0     1001      123     2277 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Bakuman.json
--rw-r--r--   0     1001      123     1911 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Battle Spirits.json
--rw-r--r--   0     1001      123   108138 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Bird.json
--rw-r--r--   0     1001      123   891099 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/BirdG.json
--rw-r--r--   0     1001      123   528555 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/BirdP.json
--rw-r--r--   0     1001      123     3893 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Black Mirror.json
--rw-r--r--   0     1001      123     3895 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Bridge.json
--rw-r--r--   0     1001      123     7962 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Britney Spears.json
--rw-r--r--   0     1001      123     7729 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Bundesliga.json
--rw-r--r--   0     1001      123    66546 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Butterfly.json
--rw-r--r--   0     1001      123     3715 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/C&C.json
--rw-r--r--   0     1001      123    17645 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/CA Places.json
--rw-r--r--   0     1001      123     2454 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/CANAAN.json
--rw-r--r--   0     1001      123    33866 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/CH Places.json
--rw-r--r--   0     1001      123    13534 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/COD.json
--rw-r--r--   0     1001      123     9143 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/CWBTyphoonOld.json
--rw-r--r--   0     1001      123     6467 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Canada.json
--rw-r--r--   0     1001      123     4462 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Carnivorous Plant.json
--rw-r--r--   0     1001      123    10024 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Cartoon.json
--rw-r--r--   0     1001      123      883 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Chanel.json
--rw-r--r--   0     1001      123    18060 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Chemistry.json
--rw-r--r--   0     1001      123     5155 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Code Black.json
--rw-r--r--   0     1001      123     7909 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Code Geass.json
--rw-r--r--   0     1001      123     2053 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/CodeLyoko.json
--rw-r--r--   0     1001      123     3078 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Coldplay.json
--rw-r--r--   0     1001      123    11955 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Communication.json
--rw-r--r--   0     1001      123     5620 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Composer.json
--rw-r--r--   0     1001      123     4654 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Copyright.json
--rw-r--r--   0     1001      123    92366 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Counter-Strike.json
--rw-r--r--   0     1001      123      294 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/County.json
--rw-r--r--   0     1001      123    17698 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Crazyracing Kartrider.json
--rw-r--r--   0     1001      123     3200 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Cyber Formula.json
--rw-r--r--   0     1001      123     6089 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Cyclone.json
--rw-r--r--   0     1001      123     1381 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/DCComics.json
--rw-r--r--   0     1001      123   103362 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/DE Places.json
--rw-r--r--   0     1001      123    10853 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Danball Senki.json
--rw-r--r--   0     1001      123     1129 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Dance.json
--rw-r--r--   0     1001      123     1629 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Death Note.json
--rw-r--r--   0     1001      123     6663 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Diablo.json
--rw-r--r--   0     1001      123      783 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Die Weiße Rose.json
--rw-r--r--   0     1001      123    17587 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Digimon.json
--rw-r--r--   0     1001      123    33790 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Disney.json
--rw-r--r--   0     1001      123     3249 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Doctor Who.json
--rw-r--r--   0     1001      123     7180 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Doraemon.json
--rw-r--r--   0     1001      123    15722 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/DragonBall.json
--rw-r--r--   0     1001      123    28035 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/DreamWorks.json
--rw-r--r--   0     1001      123     5595 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/ED.json
--rw-r--r--   0     1001      123    23292 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/EPL.json
--rw-r--r--   0     1001      123     6196 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/EU.json
--rw-r--r--   0     1001      123    10152 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Earthquake.json
--rw-r--r--   0     1001      123    34462 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Ecology.json
--rw-r--r--   0     1001      123    25054 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Economics.json
--rw-r--r--   0     1001      123    16745 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Electronics.json
--rw-r--r--   0     1001      123     1949 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Esports.json
--rw-r--r--   0     1001      123     5832 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Eyeshield21.json
--rw-r--r--   0     1001      123    16682 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/F1.json
--rw-r--r--   0     1001      123    12291 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/FAcup.json
--rw-r--r--   0     1001      123   112357 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/FR Places.json
--rw-r--r--   0     1001      123     5415 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Family Guy.json
--rw-r--r--   0     1001      123    38198 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Firearms.json
--rw-r--r--   0     1001      123    26299 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Food.json
--rw-r--r--   0     1001      123    23933 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Football.json
--rw-r--r--   0     1001      123     1431 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Friends.json
--rw-r--r--   0     1001      123     2301 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Fringe.json
--rw-r--r--   0     1001      123     5440 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Frozen.json
--rw-r--r--   0     1001      123    16568 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/FullmetalAlchemist.json
--rw-r--r--   0     1001      123     3114 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Futurama.json
--rw-r--r--   0     1001      123    30810 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/GBF.json
--rw-r--r--   0     1001      123     6024 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/GGundam.json
--rw-r--r--   0     1001      123     5068 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/GOSICK.json
--rw-r--r--   0     1001      123     5201 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/GZFC.json
--rw-r--r--   0     1001      123     6847 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Games-zh.json
--rw-r--r--   0     1001      123    75060 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Games.json
--rw-r--r--   0     1001      123     2196 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/GaoGaiGar.json
--rw-r--r--   0     1001      123     1586 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Geography.json
--rw-r--r--   0     1001      123     2860 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Getter Robo.json
--rw-r--r--   0     1001      123     6273 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Ghibli.json
--rw-r--r--   0     1001      123     7545 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Glee.json
--rw-r--r--   0     1001      123     5456 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/GossipGirl.json
--rw-r--r--   0     1001      123     5846 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Guardians of Ga'Hoole.json
--rw-r--r--   0     1001      123    28072 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Gundam00.json
--rw-r--r--   0     1001      123    21085 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/GundamAGE.json
--rw-r--r--   0     1001      123    32810 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/GundamIBO.json
--rw-r--r--   0     1001      123    37988 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/GundamSeed.json
--rw-r--r--   0     1001      123    12889 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/GundamTWFM.json
--rw-r--r--   0     1001      123    72213 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/GundamUC.json
--rw-r--r--   0     1001      123     7502 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/GundamW.json
--rw-r--r--   0     1001      123     7651 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/HTGAWM.json
--rw-r--r--   0     1001      123    14605 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/HUNTER.json
--rw-r--r--   0     1001      123     6381 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Half-Life.json
--rw-r--r--   0     1001      123     1213 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Hannibal Lecter.json
--rw-r--r--   0     1001      123    69432 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/HarryPotter.json
--rw-r--r--   0     1001      123      771 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Hawaii Five-0.json
--rw-r--r--   0     1001      123     4149 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Hayate the Combat Butler.json
--rw-r--r--   0     1001      123    10198 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Heroes of the Storm.json
--rw-r--r--   0     1001      123    12525 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/House.json
--rw-r--r--   0     1001      123     1670 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/IMF.json
--rw-r--r--   0     1001      123   186279 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/IT.json
--rw-r--r--   0     1001      123     2734 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/JLeague.json
--rw-r--r--   0     1001      123   214806 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/JP Show.json
--rw-r--r--   0     1001      123    12353 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/James Bond.json
--rw-r--r--   0     1001      123    14545 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Jewelpet.json
--rw-r--r--   0     1001      123     1814 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Justin Bieber.json
--rw-r--r--   0     1001      123     6140 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/KLeague.json
--rw-r--r--   0     1001      123    71612 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/KO Movie.json
--rw-r--r--   0     1001      123    31224 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/KO Show.json
--rw-r--r--   0     1001      123   124806 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/KO TV Show.json
--rw-r--r--   0     1001      123    30116 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/KamenRider.json
--rw-r--r--   0     1001      123     3400 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Kao.json
--rw-r--r--   0     1001      123     1214 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Katy Perry.json
--rw-r--r--   0     1001      123     1403 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Korea Comparison.json
--rw-r--r--   0     1001      123    27780 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Korea.json
--rw-r--r--   0     1001      123      563 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Korean.json
--rw-r--r--   0     1001      123     1494 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/LEGO.json
--rw-r--r--   0     1001      123    20622 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/LOL.json
--rw-r--r--   0     1001      123     5749 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/LR.json
--rw-r--r--   0     1001      123     7789 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/La casa de papel.json
--rw-r--r--   0     1001      123     2998 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Lady Gaga.json
--rw-r--r--   0     1001      123     5497 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Lana Del Rey.json
--rw-r--r--   0     1001      123     2009 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Laos.json
--rw-r--r--   0     1001      123     1545 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Legend of the Guardians.json
--rw-r--r--   0     1001      123     2412 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Les Misérables.json
--rw-r--r--   0     1001      123    64760 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Lifesciences.json
--rw-r--r--   0     1001      123      200 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Linguistics.json
--rw-r--r--   0     1001      123     3038 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Linkin.json
--rw-r--r--   0     1001      123     2381 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Lorde.json
--rw-r--r--   0     1001      123    96457 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/LuaIT.json
--rw-r--r--   0     1001      123   242697 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/LuaMovie.json
--rw-r--r--   0     1001      123   113609 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/LuaShow.json
--rw-r--r--   0     1001      123    14349 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/MA.json
--rw-r--r--   0     1001      123     5674 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/MCD.json
--rw-r--r--   0     1001      123     7228 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/MCFC.json
--rw-r--r--   0     1001      123     3350 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/MLS.json
--rw-r--r--   0     1001      123    14999 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/MUFC.json
--rw-r--r--   0     1001      123    14862 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/MY.json
--rw-r--r--   0     1001      123    17706 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Mabinogi.json
--rw-r--r--   0     1001      123    14833 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/MapleStory.json
--rw-r--r--   0     1001      123      946 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Mariah Carey.json
--rw-r--r--   0     1001      123      215 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/MarvelNetflix.json
--rw-r--r--   0     1001      123    34592 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Math.json
--rw-r--r--   0     1001      123    11580 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Mazinger.json
--rw-r--r--   0     1001      123     5877 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/McDonald's.json
--rw-r--r--   0     1001      123    16322 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/MediaWiki special.json
--rw-r--r--   0     1001      123    11410 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/MediaWiki.json
--rw-r--r--   0     1001      123    19988 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Medicine.json
--rw-r--r--   0     1001      123     1285 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Michael Jackson.json
--rw-r--r--   0     1001      123      183 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/MigTest.json
--rw-r--r--   0     1001      123     3043 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Might&Magic.json
--rw-r--r--   0     1001      123    44509 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Military.json
--rw-r--r--   0     1001      123     7029 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Minecraft.json
--rw-r--r--   0     1001      123   442700 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Movie.json
--rw-r--r--   0     1001      123    28123 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Music.json
--rw-r--r--   0     1001      123    44930 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/My Little Pony.json
--rw-r--r--   0     1001      123     8118 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/MyHeroAcademia.json
--rw-r--r--   0     1001      123    14670 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/NARUTO.json
--rw-r--r--   0     1001      123    77638 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/NBA.json
--rw-r--r--   0     1001      123     5860 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/NFL.json
--rw-r--r--   0     1001      123     1095 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/NHL.json
--rw-r--r--   0     1001      123    12730 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Nintendo.json
--rw-r--r--   0     1001      123     7719 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Nobel Prize.json
--rw-r--r--   0     1001      123    37371 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/OnePiece.json
--rw-r--r--   0     1001      123    10030 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Organization.json
--rw-r--r--   0     1001      123     4166 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Overwatch.json
--rw-r--r--   0     1001      123     3308 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/P&G.json
--rw-r--r--   0     1001      123     2081 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/PHL Places.json
--rw-r--r--   0     1001      123    94006 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/People.json
--rw-r--r--   0     1001      123     3404 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/PeppaPig.json
--rw-r--r--   0     1001      123     2479 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Percy Jackson.json
--rw-r--r--   0     1001      123     3168 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/PerryClass.json
--rw-r--r--   0     1001      123     6642 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Pesticide.json
--rw-r--r--   0     1001      123     2918 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Photography.json
--rw-r--r--   0     1001      123    28389 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Physics.json
--rw-r--r--   0     1001      123     4149 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Pichi Pichi Pitch.json
--rw-r--r--   0     1001      123      966 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Pinnacle Islands.json
--rw-r--r--   0     1001      123    34697 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Pixar.json
--rw-r--r--   0     1001      123    20027 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Pokemon-old.json
--rw-r--r--   0     1001      123    20296 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Pokemon.json
--rw-r--r--   0     1001      123    67585 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/PoliticiansUK.json
--rw-r--r--   0     1001      123     8551 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Popes.json
--rw-r--r--   0     1001      123     3495 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Power Rangers.json
--rw-r--r--   0     1001      123    31357 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/PresidentsUS.json
--rw-r--r--   0     1001      123    11576 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Pretty Rhythm.json
--rw-r--r--   0     1001      123     5719 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/PrisonBreak.json
--rw-r--r--   0     1001      123    17999 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Psychology.json
--rw-r--r--   0     1001      123    49490 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Racing.json
--rw-r--r--   0     1001      123    37973 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Railway.json
--rw-r--r--   0     1001      123     2496 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/RainbowSixSiege.json
--rw-r--r--   0     1001      123    11105 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Reborn.json
--rw-r--r--   0     1001      123     6151 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/ResidentEvil.json
--rw-r--r--   0     1001      123     3555 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Rihanna.json
--rw-r--r--   0     1001      123    35731 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/SAO.json
--rw-r--r--   0     1001      123     1842 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/SARS-CoV-2 variant.json
--rw-r--r--   0     1001      123     5934 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/SEGA.json
--rw-r--r--   0     1001      123     4084 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/SNSD.json
--rw-r--r--   0     1001      123     2282 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/SPL.json
--rw-r--r--   0     1001      123     1598 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/SPY×FAMILY.json
--rw-r--r--   0     1001      123     3803 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Sailor Moon.json
--rw-r--r--   0     1001      123     9438 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/SaintSeiyaOmega.json
--rw-r--r--   0     1001      123    74396 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Sandbox.json
--rw-r--r--   0     1001      123     1837 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Selena Gomez.json
--rw-r--r--   0     1001      123    24202 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Shinkalion.json
--rw-r--r--   0     1001      123     8677 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Shipname.json
--rw-r--r--   0     1001      123   270643 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Show.json
--rw-r--r--   0     1001      123     3132 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Shugo Chara!.json
--rw-r--r--   0     1001      123     2253 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Sia.json
--rw-r--r--   0     1001      123     2266 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Signals and Systems.json
--rw-r--r--   0     1001      123      372 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Signpost.json
--rw-r--r--   0     1001      123    11351 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Sim.json
--rw-r--r--   0     1001      123    20778 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Simpsons.json
--rw-r--r--   0     1001      123    10767 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Snooker.json
--rw-r--r--   0     1001      123     2588 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/SouthPark.json
--rw-r--r--   0     1001      123     9718 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/SpongeBob SquarePants.json
--rw-r--r--   0     1001      123    10794 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Sports.json
--rw-r--r--   0     1001      123    17092 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Square Enix.json
--rw-r--r--   0     1001      123     7526 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/StarCraft.json
--rw-r--r--   0     1001      123    11391 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/StarCraft2.json
--rw-r--r--   0     1001      123    27435 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/StarTrek.json
--rw-r--r--   0     1001      123    12653 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/StarWars.json
--rw-r--r--   0     1001      123     6942 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/StephenKing.json
--rw-r--r--   0     1001      123      549 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Summon Night.json
--rw-r--r--   0     1001      123     1674 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/TCM.json
--rw-r--r--   0     1001      123      275 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/TLeague.json
--rw-r--r--   0     1001      123   105974 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/TV.json
--rw-r--r--   0     1001      123     5543 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Table Tennis.json
--rw-r--r--   0     1001      123     3650 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Tales.json
--rw-r--r--   0     1001      123     5286 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Tamagotchi.json
--rw-r--r--   0     1001      123    11981 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Taylor Swift.json
--rw-r--r--   0     1001      123     2419 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Telcom.json
--rw-r--r--   0     1001      123    71368 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Tennis.json
--rw-r--r--   0     1001      123      115 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/TfL.json
--rw-r--r--   0     1001      123      521 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/The Chainsmokers.json
--rw-r--r--   0     1001      123    12593 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/The Witcher.json
--rw-r--r--   0     1001      123     4828 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/The World God Only Knows.json
--rw-r--r--   0     1001      123     3120 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/TheBeatles.json
--rw-r--r--   0     1001      123     2346 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/ThePeanuts.json
--rw-r--r--   0     1001      123     3570 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Toaru.json
--rw-r--r--   0     1001      123    24126 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Transformers.json
--rw-r--r--   0     1001      123     4352 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Transport for London.json
--rw-r--r--   0     1001      123    44492 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Transport.json
--rw-r--r--   0     1001      123    35103 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/TropicalCycloneName.json
--rw-r--r--   0     1001      123     3253 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Twilight.json
--rw-r--r--   0     1001      123     6974 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/TyphoonNew.json
--rw-r--r--   0     1001      123    25610 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/TyphoonOld.json
--rw-r--r--   0     1001      123     4728 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/UA toponyms.json
--rw-r--r--   0     1001      123    42557 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/UK Places.json
--rw-r--r--   0     1001      123     3707 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/US CA Cities.json
--rw-r--r--   0     1001      123     5434 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/US Government.json
--rw-r--r--   0     1001      123      584 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/US Senators.json
--rw-r--r--   0     1001      123    27748 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/USState.json
--rw-r--r--   0     1001      123    22229 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Ultraman.json
--rw-r--r--   0     1001      123     1791 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Unilever.json
--rw-r--r--   0     1001      123     7171 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Unit.json
--rw-r--r--   0     1001      123     6267 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Urban.json
--rw-r--r--   0     1001      123      802 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/VLeague.json
--rw-r--r--   0     1001      123     2372 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Valkyria.json
--rw-r--r--   0     1001      123     1272 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/WORKING!!.json
--rw-r--r--   0     1001      123    18912 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Warcraft.json
--rw-r--r--   0     1001      123     1024 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Warhammer.json
--rw-r--r--   0     1001      123    11262 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Warriors.json
--rw-r--r--   0     1001      123     1547 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Watch.json
--rw-r--r--   0     1001      123     5103 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Weather.json
--rw-r--r--   0     1001      123    14791 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Windows.json
--rw-r--r--   0     1001      123    26033 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Wow.json
--rw-r--r--   0     1001      123     8357 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Yes! 光之美少女5.json
--rw-r--r--   0     1001      123    63286 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/ZH Show.json
--rw-r--r--   0     1001      123     9963 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/arsenal.json
--rwxr-xr-x   0     1001      123     1629 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/check1.py
--rw-r--r--   0     1001      123    14239 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/chelsea.json
--rw-r--r--   0     1001      123     8008 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/fcbarcelona.json
--rw-r--r--   0     1001      123    34236 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/fcbayern.json
--rw-r--r--   0     1001      123     4414 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/free license.json
--rw-r--r--   0     1001      123     1071 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/inter.json
--rw-r--r--   0     1001      123    25910 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/laliga.json
--rw-r--r--   0     1001      123     4300 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/leek.json
--rw-r--r--   0     1001      123     4246 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/ligue.json
--rw-r--r--   0     1001      123    24883 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/liverpoolfc.json
--rw-r--r--   0     1001      123     8135 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/loghorizon.json
--rw-r--r--   0     1001      123    17062 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/magi.json
--rwxr-xr-x   0     1001      123     1497 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/merge_for_web.py
--rw-r--r--   0     1001      123    27273 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/neo-noir.json
--rw-r--r--   0     1001      123     4240 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/regalia.json
--rw-r--r--   0     1001      123     3967 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/specialpages.json
--rw-r--r--   0     1001      123    39998 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/uefa.json
--rw-r--r--   0     1001      123     8235 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/vital.json
--rw-r--r--   0     1001      123    13742 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/一拳超人.json
--rw-r--r--   0     1001      123     1103 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/伊拉克足球.json
--rw-r--r--   0     1001      123     2735 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/伊斯蘭.json
--rw-r--r--   0     1001      123     2399 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/伊朗足球.json
--rw-r--r--   0     1001      123     1615 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/佛教.json
--rw-r--r--   0     1001      123     3677 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/俄超.json
--rw-r--r--   0     1001      123    13456 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/俱乐部足球联赛.json
--rw-r--r--   0     1001      123    26449 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/列斯聯.json
--rw-r--r--   0     1001      123     2010 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/加超聯.json
--rw-r--r--   0     1001      123    11913 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/南美球會.json
--rw-r--r--   0     1001      123     1870 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/博弈论.json
--rw-r--r--   0     1001      123     2466 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/卡塔尔星级足球联赛.json
--rw-r--r--   0     1001      123     2990 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/叙利亚职业足球联赛.json
--rw-r--r--   0     1001      123     4356 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/名偵探柯南.json
--rw-r--r--   0     1001      123     7683 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/咕嚕咕嚕魔法陣.json
--rw-r--r--   0     1001      123     3368 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/咲-Saki-.json
--rw-r--r--   0     1001      123      413 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/單雙書名號轉換.json
--rw-r--r--   0     1001      123     8161 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/四驅兄弟.json
--rw-r--r--   0     1001      123     1765 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/圍棋.json
--rw-r--r--   0     1001      123    91171 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/地名.json
--rw-r--r--   0     1001      123    11946 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/声临其境.json
--rw-r--r--   0     1001      123    16032 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/妖怪手錶.json
--rw-r--r--   0     1001      123     4612 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/姓氏.json
--rw-r--r--   0     1001      123     1706 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/娛樂.json
--rw-r--r--   0     1001      123     6143 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/小魔女DoReMi.json
--rw-r--r--   0     1001      123     1049 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/巴勒斯坦职业足球联赛.json
--rw-r--r--   0     1001      123     3401 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/巴林职业足球联赛.json
--rw-r--r--   0     1001      123     7552 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/幸福爆發！光之美少女.json
--rw-r--r--   0     1001      123    18532 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/意甲.json
--rw-r--r--   0     1001      123     5596 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/愛天使傳說.json
--rw-r--r--   0     1001      123     8810 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/戰鬥陀螺 鋼鐵奇兵.json
--rw-r--r--   0     1001      123     5374 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/打工吧！魔王大人.json
--rw-r--r--   0     1001      123    12531 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/政治人物.json
--rw-r--r--   0     1001      123    24277 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/文學.json
--rw-r--r--   0     1001      123    21774 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/星光樂園.json
--rw-r--r--   0     1001      123     2086 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/暗影诗章 (动画).json
--rw-r--r--   0     1001      123     1937 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/村上春樹.json
--rw-r--r--   0     1001      123     2512 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/核能.json
--rw-r--r--   0     1001      123     7040 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/機獸系列.json
--rw-r--r--   0     1001      123      672 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/民族.json
--rw-r--r--   0     1001      123     7491 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/沙特职业足球联赛.json
--rw-r--r--   0     1001      123     2691 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/泰國人名.json
--rw-r--r--   0     1001      123     1917 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/涼宮春日的憂鬱.json
--rw-r--r--   0     1001      123     4807 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/潘朵拉之心.json
--rw-r--r--   0     1001      123     3560 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/烏茲別克足球會.json
--rw-r--r--   0     1001      123     7746 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/爆丸.json
--rw-r--r--   0     1001      123     1968 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/畜牧.json
--rw-r--r--   0     1001      123      476 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/當個創世神.json
--rw-r--r--   0     1001      123     4081 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/百變小櫻.json
--rw-r--r--   0     1001      123     1690 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/科威特职业足球联赛.json
--rw-r--r--   0     1001      123     4326 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/童話槍手小紅帽.json
--rw-r--r--   0     1001      123     1287 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/约旦职业足球联赛.json
--rw-r--r--   0     1001      123    50765 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/美国漫画.json
--rw-r--r--   0     1001      123      358 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/艾维里奥斯.json
--rw-r--r--   0     1001      123     4284 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/荷蘭足球聯賽.json
--rw-r--r--   0     1001      123     5889 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/菁英殺機.json
--rw-r--r--   0     1001      123     2402 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/葡超.json
--rw-r--r--   0     1001      123     4186 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/蠟筆小新.json
--rw-r--r--   0     1001      123      332 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/语言与语音.json
--rw-r--r--   0     1001      123     4180 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/通靈王.json
--rw-r--r--   0     1001      123    12331 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/進擊的巨人.json
--rw-r--r--   0     1001      123      964 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/釣魚臺列嶼.json
--rw-r--r--   0     1001      123    29385 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/閃電十一人.json
--rw-r--r--   0     1001      123     2453 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/闇.json
--rw-r--r--   0     1001      123      919 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/阿曼职业足球联赛.json
--rw-r--r--   0     1001      123     4315 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/阿联酋职业足球联赛.json
--rw-r--r--   0     1001      123     2845 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/降世神通.json
--rw-r--r--   0     1001      123     1889 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/音樂劇.json
--rw-r--r--   0     1001      123     5499 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/驅魔少年.json
--rw-r--r--   0     1001      123    14375 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/马来人名地名.json
--rw-r--r--   0     1001      123    16434 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/鬥陣特攻.json
--rw-r--r--   0     1001      123     5689 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/魔法咪路咪路.json
--rw-r--r--   0     1001      123     1103 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/黎巴嫩职业足球联赛.json
--rw-r--r--   0     1001      123    10818 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/黑執事.json
--rw-r--r--   0     1001      123     2840 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/黑塔系列.json
--rw-r--r--   0     1001      123     5472 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/poetry.lock
--rw-r--r--   0     1001      123      308 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/pyproject.toml
--rwxr-xr-x   0     1001      123     3645 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/update_basic.py
--rwxr-xr-x   0     1001      123    12250 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/update_cgroups.py
--rwxr-xr-x   0     1001      123      857 2023-05-15 07:53:25.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/run-maturin-action.sh
--rw-r--r--   0     1001      123    16391 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/src/converter.rs
--rw-r--r--   0     1001      123     3509 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/src/converters.rs
--rw-r--r--   0     1001      123     5075 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/src/lib.rs
--rw-r--r--   0     1001      123     2060 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/src/pagerules.rs
--rw-r--r--   0     1001      123    12097 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/src/rule.rs
--rw-r--r--   0     1001      123     5133 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/src/tables.rs
--rw-r--r--   0     1001      123      409 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/src/utils.rs
--rw-r--r--   0     1001      123     8365 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/src/variant.rs
--rw-r--r--   0     1001      123     2491 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/src/wasm.rs
--rw-r--r--   0     1001      123      342 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/.gitignore
--rw-r--r--   0     1001      123     2113 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/README.md
--rw-r--r--   0     1001      123     1407 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/config-overrides.js
--rw-r--r--   0     1001      123     1350 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/package.json
--rw-r--r--   0     1001      123  3976144 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/public/cgroups.json
--rw-r--r--   0     1001      123     2159 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/public/index.html
--rw-r--r--   0     1001      123     3870 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/public/logo.ico
--rw-r--r--   0     1001      123     5347 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/public/logo192.png
--rw-r--r--   0     1001      123     9664 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/public/logo512.png
--rw-r--r--   0     1001      123      475 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/public/manifest.json
--rw-r--r--   0     1001      123       67 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/public/robots.txt
--rw-r--r--   0     1001      123      564 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/src/App.css
--rw-r--r--   0     1001      123      273 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/src/App.test.tsx
--rw-r--r--   0     1001      123     3332 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/src/App.tsx
--rw-r--r--   0     1001      123     4309 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/src/components/AboutDialog.tsx
--rw-r--r--   0     1001      123      882 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/src/components/CGroupCheckbox.tsx
--rw-r--r--   0     1001      123     6667 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/src/components/CGroupSelect.tsx
--rw-r--r--   0     1001      123     4808 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/src/components/ConvertButton.tsx
--rw-r--r--   0     1001      123     4230 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/src/components/Footer.tsx
--rw-r--r--   0     1001      123     3547 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/src/components/Header.tsx
--rw-r--r--   0     1001      123     1256 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/src/components/InputEditor.tsx
--rw-r--r--   0     1001      123     3874 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/src/components/OptionsControl.tsx
--rw-r--r--   0     1001      123      820 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/src/components/OutputEditor.tsx
--rw-r--r--   0     1001      123      552 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/src/components/OutputStatusLine.tsx
--rw-r--r--   0     1001      123      217 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/src/components/editorCommon.tsx
--rw-r--r--   0     1001      123      366 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/src/index.css
--rw-r--r--   0     1001      123      500 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/src/index.tsx
--rw-r--r--   0     1001      123     2632 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/src/logo.svg
--rw-r--r--   0     1001      123       40 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/src/react-app-env.d.ts
--rw-r--r--   0     1001      123      425 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/src/reportWebVitals.ts
--rw-r--r--   0     1001      123      241 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/src/setupTests.ts
--rw-r--r--   0     1001      123      150 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/src/utils.ts
--rw-r--r--   0     1001      123      535 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/tsconfig.json
--rw-r--r--   0     1001      123   539286 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/yarn.lock
--rw-r--r--   0        0        0      562 1970-01-01 00:00:00.000000 zhconv_rs-0.2.0b0/Cargo.toml
--rw-r--r--   0     1001      123      685 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/.gitignore
--rw-r--r--   0     1001      123    10364 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/README.md
--rw-r--r--   0     1001      123      643 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/pyproject.toml
--rw-r--r--   0     1001      123     5338 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/src/lib.rs
--rw-r--r--   0     1001      123      726 2023-05-15 07:52:47.000000 zhconv_rs-0.2.0b0/zhconv_rs.pyi
--rw-r--r--   0     1001      123    20083 2023-05-15 07:55:18.000000 zhconv_rs-0.2.0b0/Cargo.lock
--rw-r--r--   0        0        0    11103 1970-01-01 00:00:00.000000 zhconv_rs-0.2.0b0/PKG-INFO
+-rw-r--r--   0        0        0     1863 1970-01-01 00:00:00.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/Cargo.toml
+-rw-r--r--   0     1001      123      426 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/.gitattributes
+-rw-r--r--   0     1001      123     1775 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/.github/workflows/main.yml
+-rw-r--r--   0     1001      123     2445 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/.github/workflows/npm.yml
+-rw-r--r--   0     1001      123     1973 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/.github/workflows/pyo3.yml
+-rw-r--r--   0     1001      123     2703 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/.github/workflows/release.yml
+-rw-r--r--   0     1001      123       20 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/.gitignore
+-rw-r--r--   0     1001      123    35149 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/LICENSE
+-rw-r--r--   0     1001      123    10364 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/README.md
+-rw-r--r--   0     1001      123   284864 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/benches/25328-0.txt
+-rw-r--r--   0     1001      123      198 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/benches/LICENSE.md
+-rw-r--r--   0     1001      123  3261912 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/benches/data3185k.txt
+-rw-r--r--   0     1001      123    55192 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/benches/data54k.txt
+-rw-r--r--   0     1001      123   705845 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/benches/data689k.txt
+-rw-r--r--   0     1001      123    79133 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/benches/wikitext.txt
+-rw-r--r--   0     1001      123     5755 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/benches/zhconv_benchmark.rs
+-rw-r--r--   0     1001      123    19923 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/build.rs
+-rw-r--r--   0     1001      123      532 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/HKVariants.txt
+-rw-r--r--   0     1001      123     2709 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/HKVariantsRevPhrases.txt
+-rw-r--r--   0     1001      123      870 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/README.md
+-rw-r--r--   0     1001      123    34353 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/STCharacters.txt
+-rw-r--r--   0     1001      123  1004153 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/STPhrases.txt
+-rw-r--r--   0     1001      123    34627 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/TSCharacters.txt
+-rw-r--r--   0     1001      123     5161 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/TSPhrases.txt
+-rw-r--r--   0     1001      123     7611 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/TWPhrasesIT.txt
+-rw-r--r--   0     1001      123     2121 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/TWPhrasesName.txt
+-rw-r--r--   0     1001      123      571 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/TWPhrasesOther.txt
+-rw-r--r--   0     1001      123      312 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/TWVariants.txt
+-rw-r--r--   0     1001      123     1075 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/TWVariantsRevPhrases.txt
+-rw-r--r--   0     1001      123   447718 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/ZhConversion.php
+-rw-r--r--   0     1001      123     7470 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/1D.json
+-rw-r--r--   0     1001      123     4660 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/2016年太平洋颱風季.json
+-rw-r--r--   0     1001      123     4462 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/2017年太平洋颱風季.json
+-rw-r--r--   0     1001      123     4953 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/2018年太平洋颱風季.json
+-rw-r--r--   0     1001      123     4967 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/2019年太平洋颱風季.json
+-rw-r--r--   0     1001      123     4150 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/2020年太平洋颱風季.json
+-rw-r--r--   0     1001      123     3977 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/2021年太平洋颱風季.json
+-rw-r--r--   0     1001      123     4396 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/2022年太平洋颱風季.json
+-rw-r--r--   0     1001      123      311 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/2023年太平洋颱風季.json
+-rw-r--r--   0     1001      123    18639 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/24.json
+-rw-r--r--   0     1001      123     1347 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/A Pink.json
+-rw-r--r--   0     1001      123     1436 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/A Song of Ice and Fire.json
+-rw-r--r--   0     1001      123     4784 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/ACmilan.json
+-rw-r--r--   0     1001      123     4078 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/ALeague.json
+-rw-r--r--   0     1001      123    12349 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/AT Places.json
+-rw-r--r--   0     1001      123    12270 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/AU Places.json
+-rw-r--r--   0     1001      123     2618 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Adventure Time.json
+-rw-r--r--   0     1001      123    24747 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Aero.json
+-rw-r--r--   0     1001      123     4785 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Aikatsu.json
+-rw-r--r--   0     1001      123    44770 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Anime.json
+-rw-r--r--   0     1001      123    11339 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Apple.json
+-rw-r--r--   0     1001      123     6426 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Aquatics.json
+-rw-r--r--   0     1001      123     3127 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Ariana Grande.json
+-rw-r--r--   0     1001      123      682 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Artist.json
+-rw-r--r--   0     1001      123    11447 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Astronomy.json
+-rw-r--r--   0     1001      123     4837 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Avatar.json
+-rw-r--r--   0     1001      123     3325 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Avril Lavigne.json
+-rw-r--r--   0     1001      123    46163 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/BE Places.json
+-rw-r--r--   0     1001      123    11395 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/BUDDYCOMPLEX.json
+-rw-r--r--   0     1001      123    10696 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Badminton.json
+-rw-r--r--   0     1001      123     2277 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Bakuman.json
+-rw-r--r--   0     1001      123     1911 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Battle Spirits.json
+-rw-r--r--   0     1001      123   108138 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Bird.json
+-rw-r--r--   0     1001      123   891099 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/BirdG.json
+-rw-r--r--   0     1001      123   528555 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/BirdP.json
+-rw-r--r--   0     1001      123     3893 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Black Mirror.json
+-rw-r--r--   0     1001      123     3895 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Bridge.json
+-rw-r--r--   0     1001      123     7962 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Britney Spears.json
+-rw-r--r--   0     1001      123     7729 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Bundesliga.json
+-rw-r--r--   0     1001      123    66546 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Butterfly.json
+-rw-r--r--   0     1001      123     3715 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/C&C.json
+-rw-r--r--   0     1001      123    17645 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/CA Places.json
+-rw-r--r--   0     1001      123     2454 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/CANAAN.json
+-rw-r--r--   0     1001      123    33866 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/CH Places.json
+-rw-r--r--   0     1001      123    13534 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/COD.json
+-rw-r--r--   0     1001      123     9143 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/CWBTyphoonOld.json
+-rw-r--r--   0     1001      123     6467 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Canada.json
+-rw-r--r--   0     1001      123     4462 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Carnivorous Plant.json
+-rw-r--r--   0     1001      123    10024 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Cartoon.json
+-rw-r--r--   0     1001      123      883 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Chanel.json
+-rw-r--r--   0     1001      123    18060 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Chemistry.json
+-rw-r--r--   0     1001      123     5155 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Code Black.json
+-rw-r--r--   0     1001      123     7909 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Code Geass.json
+-rw-r--r--   0     1001      123     2053 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/CodeLyoko.json
+-rw-r--r--   0     1001      123     3078 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Coldplay.json
+-rw-r--r--   0     1001      123    11955 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Communication.json
+-rw-r--r--   0     1001      123     5620 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Composer.json
+-rw-r--r--   0     1001      123     4654 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Copyright.json
+-rw-r--r--   0     1001      123    92366 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Counter-Strike.json
+-rw-r--r--   0     1001      123      294 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/County.json
+-rw-r--r--   0     1001      123    17698 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Crazyracing Kartrider.json
+-rw-r--r--   0     1001      123     3200 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Cyber Formula.json
+-rw-r--r--   0     1001      123     6089 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Cyclone.json
+-rw-r--r--   0     1001      123     1381 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/DCComics.json
+-rw-r--r--   0     1001      123   103362 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/DE Places.json
+-rw-r--r--   0     1001      123    10853 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Danball Senki.json
+-rw-r--r--   0     1001      123     1129 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Dance.json
+-rw-r--r--   0     1001      123     1629 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Death Note.json
+-rw-r--r--   0     1001      123     6663 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Diablo.json
+-rw-r--r--   0     1001      123      783 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Die Weiße Rose.json
+-rw-r--r--   0     1001      123    17587 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Digimon.json
+-rw-r--r--   0     1001      123    33790 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Disney.json
+-rw-r--r--   0     1001      123     3249 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Doctor Who.json
+-rw-r--r--   0     1001      123     7180 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Doraemon.json
+-rw-r--r--   0     1001      123    15722 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/DragonBall.json
+-rw-r--r--   0     1001      123    28035 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/DreamWorks.json
+-rw-r--r--   0     1001      123     5595 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/ED.json
+-rw-r--r--   0     1001      123    23292 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/EPL.json
+-rw-r--r--   0     1001      123     6196 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/EU.json
+-rw-r--r--   0     1001      123    10152 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Earthquake.json
+-rw-r--r--   0     1001      123    34462 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Ecology.json
+-rw-r--r--   0     1001      123    25054 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Economics.json
+-rw-r--r--   0     1001      123    16745 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Electronics.json
+-rw-r--r--   0     1001      123     1949 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Esports.json
+-rw-r--r--   0     1001      123     5832 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Eyeshield21.json
+-rw-r--r--   0     1001      123    16682 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/F1.json
+-rw-r--r--   0     1001      123    12291 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/FAcup.json
+-rw-r--r--   0     1001      123   112357 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/FR Places.json
+-rw-r--r--   0     1001      123     5415 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Family Guy.json
+-rw-r--r--   0     1001      123    38198 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Firearms.json
+-rw-r--r--   0     1001      123    26299 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Food.json
+-rw-r--r--   0     1001      123    23933 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Football.json
+-rw-r--r--   0     1001      123     1431 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Friends.json
+-rw-r--r--   0     1001      123     2301 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Fringe.json
+-rw-r--r--   0     1001      123     5440 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Frozen.json
+-rw-r--r--   0     1001      123    16568 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/FullmetalAlchemist.json
+-rw-r--r--   0     1001      123     3114 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Futurama.json
+-rw-r--r--   0     1001      123    30810 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/GBF.json
+-rw-r--r--   0     1001      123     6024 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/GGundam.json
+-rw-r--r--   0     1001      123     5068 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/GOSICK.json
+-rw-r--r--   0     1001      123     5201 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/GZFC.json
+-rw-r--r--   0     1001      123     6847 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Games-zh.json
+-rw-r--r--   0     1001      123    75060 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Games.json
+-rw-r--r--   0     1001      123     2196 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/GaoGaiGar.json
+-rw-r--r--   0     1001      123     1586 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Geography.json
+-rw-r--r--   0     1001      123     2860 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Getter Robo.json
+-rw-r--r--   0     1001      123     6273 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Ghibli.json
+-rw-r--r--   0     1001      123     7545 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Glee.json
+-rw-r--r--   0     1001      123     5456 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/GossipGirl.json
+-rw-r--r--   0     1001      123     5846 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Guardians of Ga'Hoole.json
+-rw-r--r--   0     1001      123    28072 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Gundam00.json
+-rw-r--r--   0     1001      123    21085 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/GundamAGE.json
+-rw-r--r--   0     1001      123    32810 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/GundamIBO.json
+-rw-r--r--   0     1001      123    37988 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/GundamSeed.json
+-rw-r--r--   0     1001      123    12889 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/GundamTWFM.json
+-rw-r--r--   0     1001      123    72213 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/GundamUC.json
+-rw-r--r--   0     1001      123     7502 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/GundamW.json
+-rw-r--r--   0     1001      123     7651 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/HTGAWM.json
+-rw-r--r--   0     1001      123    14605 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/HUNTER.json
+-rw-r--r--   0     1001      123     6381 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Half-Life.json
+-rw-r--r--   0     1001      123     1213 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Hannibal Lecter.json
+-rw-r--r--   0     1001      123    69432 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/HarryPotter.json
+-rw-r--r--   0     1001      123      771 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Hawaii Five-0.json
+-rw-r--r--   0     1001      123     4149 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Hayate the Combat Butler.json
+-rw-r--r--   0     1001      123    10198 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Heroes of the Storm.json
+-rw-r--r--   0     1001      123    12525 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/House.json
+-rw-r--r--   0     1001      123     1670 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/IMF.json
+-rw-r--r--   0     1001      123   186279 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/IT.json
+-rw-r--r--   0     1001      123     2734 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/JLeague.json
+-rw-r--r--   0     1001      123   214806 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/JP Show.json
+-rw-r--r--   0     1001      123    12353 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/James Bond.json
+-rw-r--r--   0     1001      123    14545 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Jewelpet.json
+-rw-r--r--   0     1001      123     1814 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Justin Bieber.json
+-rw-r--r--   0     1001      123     6140 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/KLeague.json
+-rw-r--r--   0     1001      123    71612 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/KO Movie.json
+-rw-r--r--   0     1001      123    31224 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/KO Show.json
+-rw-r--r--   0     1001      123   124806 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/KO TV Show.json
+-rw-r--r--   0     1001      123    30116 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/KamenRider.json
+-rw-r--r--   0     1001      123     3400 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Kao.json
+-rw-r--r--   0     1001      123     1214 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Katy Perry.json
+-rw-r--r--   0     1001      123     1403 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Korea Comparison.json
+-rw-r--r--   0     1001      123    27780 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Korea.json
+-rw-r--r--   0     1001      123      563 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Korean.json
+-rw-r--r--   0     1001      123     1494 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/LEGO.json
+-rw-r--r--   0     1001      123    20622 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/LOL.json
+-rw-r--r--   0     1001      123     5749 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/LR.json
+-rw-r--r--   0     1001      123     7789 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/La casa de papel.json
+-rw-r--r--   0     1001      123     2998 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Lady Gaga.json
+-rw-r--r--   0     1001      123     5497 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Lana Del Rey.json
+-rw-r--r--   0     1001      123     2009 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Laos.json
+-rw-r--r--   0     1001      123     1545 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Legend of the Guardians.json
+-rw-r--r--   0     1001      123     2412 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Les Misérables.json
+-rw-r--r--   0     1001      123    64760 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Lifesciences.json
+-rw-r--r--   0     1001      123      200 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Linguistics.json
+-rw-r--r--   0     1001      123     3038 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Linkin.json
+-rw-r--r--   0     1001      123     2381 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Lorde.json
+-rw-r--r--   0     1001      123    96457 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/LuaIT.json
+-rw-r--r--   0     1001      123   242697 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/LuaMovie.json
+-rw-r--r--   0     1001      123   113609 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/LuaShow.json
+-rw-r--r--   0     1001      123    14349 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/MA.json
+-rw-r--r--   0     1001      123     5674 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/MCD.json
+-rw-r--r--   0     1001      123     7228 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/MCFC.json
+-rw-r--r--   0     1001      123     3350 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/MLS.json
+-rw-r--r--   0     1001      123    14999 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/MUFC.json
+-rw-r--r--   0     1001      123    14862 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/MY.json
+-rw-r--r--   0     1001      123    17706 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Mabinogi.json
+-rw-r--r--   0     1001      123    14833 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/MapleStory.json
+-rw-r--r--   0     1001      123      946 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Mariah Carey.json
+-rw-r--r--   0     1001      123      215 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/MarvelNetflix.json
+-rw-r--r--   0     1001      123    34592 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Math.json
+-rw-r--r--   0     1001      123    11580 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Mazinger.json
+-rw-r--r--   0     1001      123     5877 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/McDonald's.json
+-rw-r--r--   0     1001      123    16322 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/MediaWiki special.json
+-rw-r--r--   0     1001      123    11410 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/MediaWiki.json
+-rw-r--r--   0     1001      123    19988 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Medicine.json
+-rw-r--r--   0     1001      123     1285 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Michael Jackson.json
+-rw-r--r--   0     1001      123      183 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/MigTest.json
+-rw-r--r--   0     1001      123     3043 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Might&Magic.json
+-rw-r--r--   0     1001      123    44509 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Military.json
+-rw-r--r--   0     1001      123     7029 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Minecraft.json
+-rw-r--r--   0     1001      123   442700 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Movie.json
+-rw-r--r--   0     1001      123    28123 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Music.json
+-rw-r--r--   0     1001      123    44930 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/My Little Pony.json
+-rw-r--r--   0     1001      123     8118 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/MyHeroAcademia.json
+-rw-r--r--   0     1001      123    14670 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/NARUTO.json
+-rw-r--r--   0     1001      123    77638 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/NBA.json
+-rw-r--r--   0     1001      123     5860 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/NFL.json
+-rw-r--r--   0     1001      123     1095 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/NHL.json
+-rw-r--r--   0     1001      123    12730 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Nintendo.json
+-rw-r--r--   0     1001      123     7719 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Nobel Prize.json
+-rw-r--r--   0     1001      123    37371 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/OnePiece.json
+-rw-r--r--   0     1001      123    10030 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Organization.json
+-rw-r--r--   0     1001      123     4166 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Overwatch.json
+-rw-r--r--   0     1001      123     3308 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/P&G.json
+-rw-r--r--   0     1001      123     2081 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/PHL Places.json
+-rw-r--r--   0     1001      123    94006 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/People.json
+-rw-r--r--   0     1001      123     3404 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/PeppaPig.json
+-rw-r--r--   0     1001      123     2479 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Percy Jackson.json
+-rw-r--r--   0     1001      123     3168 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/PerryClass.json
+-rw-r--r--   0     1001      123     6642 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Pesticide.json
+-rw-r--r--   0     1001      123     2918 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Photography.json
+-rw-r--r--   0     1001      123    28389 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Physics.json
+-rw-r--r--   0     1001      123     4149 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Pichi Pichi Pitch.json
+-rw-r--r--   0     1001      123      966 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Pinnacle Islands.json
+-rw-r--r--   0     1001      123    34697 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Pixar.json
+-rw-r--r--   0     1001      123    20027 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Pokemon-old.json
+-rw-r--r--   0     1001      123    20296 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Pokemon.json
+-rw-r--r--   0     1001      123    67585 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/PoliticiansUK.json
+-rw-r--r--   0     1001      123     8551 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Popes.json
+-rw-r--r--   0     1001      123     3495 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Power Rangers.json
+-rw-r--r--   0     1001      123    31357 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/PresidentsUS.json
+-rw-r--r--   0     1001      123    11576 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Pretty Rhythm.json
+-rw-r--r--   0     1001      123     5719 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/PrisonBreak.json
+-rw-r--r--   0     1001      123    17999 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Psychology.json
+-rw-r--r--   0     1001      123    49490 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Racing.json
+-rw-r--r--   0     1001      123    37973 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Railway.json
+-rw-r--r--   0     1001      123     2496 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/RainbowSixSiege.json
+-rw-r--r--   0     1001      123    11105 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Reborn.json
+-rw-r--r--   0     1001      123     6151 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/ResidentEvil.json
+-rw-r--r--   0     1001      123     3555 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Rihanna.json
+-rw-r--r--   0     1001      123    35731 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/SAO.json
+-rw-r--r--   0     1001      123     1842 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/SARS-CoV-2 variant.json
+-rw-r--r--   0     1001      123     5934 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/SEGA.json
+-rw-r--r--   0     1001      123     4084 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/SNSD.json
+-rw-r--r--   0     1001      123     2282 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/SPL.json
+-rw-r--r--   0     1001      123     1598 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/SPY×FAMILY.json
+-rw-r--r--   0     1001      123     3803 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Sailor Moon.json
+-rw-r--r--   0     1001      123     9438 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/SaintSeiyaOmega.json
+-rw-r--r--   0     1001      123    74396 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Sandbox.json
+-rw-r--r--   0     1001      123     1837 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Selena Gomez.json
+-rw-r--r--   0     1001      123    24202 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Shinkalion.json
+-rw-r--r--   0     1001      123     8677 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Shipname.json
+-rw-r--r--   0     1001      123   270643 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Show.json
+-rw-r--r--   0     1001      123     3132 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Shugo Chara!.json
+-rw-r--r--   0     1001      123     2253 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Sia.json
+-rw-r--r--   0     1001      123     2266 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Signals and Systems.json
+-rw-r--r--   0     1001      123      372 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Signpost.json
+-rw-r--r--   0     1001      123    11351 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Sim.json
+-rw-r--r--   0     1001      123    20778 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Simpsons.json
+-rw-r--r--   0     1001      123    10767 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Snooker.json
+-rw-r--r--   0     1001      123     2588 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/SouthPark.json
+-rw-r--r--   0     1001      123     9718 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/SpongeBob SquarePants.json
+-rw-r--r--   0     1001      123    10794 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Sports.json
+-rw-r--r--   0     1001      123    17092 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Square Enix.json
+-rw-r--r--   0     1001      123     7526 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/StarCraft.json
+-rw-r--r--   0     1001      123    11391 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/StarCraft2.json
+-rw-r--r--   0     1001      123    27435 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/StarTrek.json
+-rw-r--r--   0     1001      123    12653 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/StarWars.json
+-rw-r--r--   0     1001      123     6942 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/StephenKing.json
+-rw-r--r--   0     1001      123      549 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Summon Night.json
+-rw-r--r--   0     1001      123     1674 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/TCM.json
+-rw-r--r--   0     1001      123      275 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/TLeague.json
+-rw-r--r--   0     1001      123   105974 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/TV.json
+-rw-r--r--   0     1001      123     5543 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Table Tennis.json
+-rw-r--r--   0     1001      123     3650 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Tales.json
+-rw-r--r--   0     1001      123     5286 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Tamagotchi.json
+-rw-r--r--   0     1001      123    11981 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Taylor Swift.json
+-rw-r--r--   0     1001      123     2419 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Telcom.json
+-rw-r--r--   0     1001      123    71368 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Tennis.json
+-rw-r--r--   0     1001      123      115 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/TfL.json
+-rw-r--r--   0     1001      123      521 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/The Chainsmokers.json
+-rw-r--r--   0     1001      123    12593 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/The Witcher.json
+-rw-r--r--   0     1001      123     4828 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/The World God Only Knows.json
+-rw-r--r--   0     1001      123     3120 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/TheBeatles.json
+-rw-r--r--   0     1001      123     2346 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/ThePeanuts.json
+-rw-r--r--   0     1001      123     3570 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Toaru.json
+-rw-r--r--   0     1001      123    24126 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Transformers.json
+-rw-r--r--   0     1001      123     4352 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Transport for London.json
+-rw-r--r--   0     1001      123    44492 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Transport.json
+-rw-r--r--   0     1001      123    35103 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/TropicalCycloneName.json
+-rw-r--r--   0     1001      123     3253 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Twilight.json
+-rw-r--r--   0     1001      123     6974 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/TyphoonNew.json
+-rw-r--r--   0     1001      123    25610 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/TyphoonOld.json
+-rw-r--r--   0     1001      123     4728 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/UA toponyms.json
+-rw-r--r--   0     1001      123    42557 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/UK Places.json
+-rw-r--r--   0     1001      123     3707 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/US CA Cities.json
+-rw-r--r--   0     1001      123     5434 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/US Government.json
+-rw-r--r--   0     1001      123      584 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/US Senators.json
+-rw-r--r--   0     1001      123    27748 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/USState.json
+-rw-r--r--   0     1001      123    22229 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Ultraman.json
+-rw-r--r--   0     1001      123     1791 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Unilever.json
+-rw-r--r--   0     1001      123     7171 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Unit.json
+-rw-r--r--   0     1001      123     6267 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Urban.json
+-rw-r--r--   0     1001      123      802 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/VLeague.json
+-rw-r--r--   0     1001      123     2372 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Valkyria.json
+-rw-r--r--   0     1001      123     1272 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/WORKING!!.json
+-rw-r--r--   0     1001      123    18912 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Warcraft.json
+-rw-r--r--   0     1001      123     1024 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Warhammer.json
+-rw-r--r--   0     1001      123    11262 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Warriors.json
+-rw-r--r--   0     1001      123     1547 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Watch.json
+-rw-r--r--   0     1001      123     5103 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Weather.json
+-rw-r--r--   0     1001      123    14791 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Windows.json
+-rw-r--r--   0     1001      123    26033 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Wow.json
+-rw-r--r--   0     1001      123     8357 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Yes! 光之美少女5.json
+-rw-r--r--   0     1001      123    63286 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/ZH Show.json
+-rw-r--r--   0     1001      123     9963 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/arsenal.json
+-rwxr-xr-x   0     1001      123     1629 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/check1.py
+-rw-r--r--   0     1001      123    14239 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/chelsea.json
+-rw-r--r--   0     1001      123     8008 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/fcbarcelona.json
+-rw-r--r--   0     1001      123    34236 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/fcbayern.json
+-rw-r--r--   0     1001      123     4414 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/free license.json
+-rw-r--r--   0     1001      123     1071 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/inter.json
+-rw-r--r--   0     1001      123    25910 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/laliga.json
+-rw-r--r--   0     1001      123     4300 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/leek.json
+-rw-r--r--   0     1001      123     4246 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/ligue.json
+-rw-r--r--   0     1001      123    24883 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/liverpoolfc.json
+-rw-r--r--   0     1001      123     8135 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/loghorizon.json
+-rw-r--r--   0     1001      123    17062 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/magi.json
+-rwxr-xr-x   0     1001      123     1497 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/merge_for_web.py
+-rw-r--r--   0     1001      123    27273 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/neo-noir.json
+-rw-r--r--   0     1001      123     4240 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/regalia.json
+-rw-r--r--   0     1001      123     3967 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/specialpages.json
+-rw-r--r--   0     1001      123    39998 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/uefa.json
+-rw-r--r--   0     1001      123     8235 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/vital.json
+-rw-r--r--   0     1001      123    13742 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/一拳超人.json
+-rw-r--r--   0     1001      123     1103 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/伊拉克足球.json
+-rw-r--r--   0     1001      123     2735 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/伊斯蘭.json
+-rw-r--r--   0     1001      123     2399 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/伊朗足球.json
+-rw-r--r--   0     1001      123     1615 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/佛教.json
+-rw-r--r--   0     1001      123     3677 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/俄超.json
+-rw-r--r--   0     1001      123    13456 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/俱乐部足球联赛.json
+-rw-r--r--   0     1001      123    26449 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/列斯聯.json
+-rw-r--r--   0     1001      123     2010 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/加超聯.json
+-rw-r--r--   0     1001      123    11913 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/南美球會.json
+-rw-r--r--   0     1001      123     1870 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/博弈论.json
+-rw-r--r--   0     1001      123     2466 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/卡塔尔星级足球联赛.json
+-rw-r--r--   0     1001      123     2990 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/叙利亚职业足球联赛.json
+-rw-r--r--   0     1001      123     4356 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/名偵探柯南.json
+-rw-r--r--   0     1001      123     7683 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/咕嚕咕嚕魔法陣.json
+-rw-r--r--   0     1001      123     3368 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/咲-Saki-.json
+-rw-r--r--   0     1001      123      413 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/單雙書名號轉換.json
+-rw-r--r--   0     1001      123     8161 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/四驅兄弟.json
+-rw-r--r--   0     1001      123     1765 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/圍棋.json
+-rw-r--r--   0     1001      123    91171 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/地名.json
+-rw-r--r--   0     1001      123    11946 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/声临其境.json
+-rw-r--r--   0     1001      123    16032 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/妖怪手錶.json
+-rw-r--r--   0     1001      123     4612 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/姓氏.json
+-rw-r--r--   0     1001      123     1706 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/娛樂.json
+-rw-r--r--   0     1001      123     6143 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/小魔女DoReMi.json
+-rw-r--r--   0     1001      123     1049 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/巴勒斯坦职业足球联赛.json
+-rw-r--r--   0     1001      123     3401 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/巴林职业足球联赛.json
+-rw-r--r--   0     1001      123     7552 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/幸福爆發！光之美少女.json
+-rw-r--r--   0     1001      123    18532 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/意甲.json
+-rw-r--r--   0     1001      123     5596 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/愛天使傳說.json
+-rw-r--r--   0     1001      123     8810 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/戰鬥陀螺 鋼鐵奇兵.json
+-rw-r--r--   0     1001      123     5374 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/打工吧！魔王大人.json
+-rw-r--r--   0     1001      123    12531 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/政治人物.json
+-rw-r--r--   0     1001      123    24277 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/文學.json
+-rw-r--r--   0     1001      123    21774 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/星光樂園.json
+-rw-r--r--   0     1001      123     2086 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/暗影诗章 (动画).json
+-rw-r--r--   0     1001      123     1937 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/村上春樹.json
+-rw-r--r--   0     1001      123     2512 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/核能.json
+-rw-r--r--   0     1001      123     7040 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/機獸系列.json
+-rw-r--r--   0     1001      123      672 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/民族.json
+-rw-r--r--   0     1001      123     7491 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/沙特职业足球联赛.json
+-rw-r--r--   0     1001      123     2691 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/泰國人名.json
+-rw-r--r--   0     1001      123     1917 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/涼宮春日的憂鬱.json
+-rw-r--r--   0     1001      123     4807 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/潘朵拉之心.json
+-rw-r--r--   0     1001      123     3560 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/烏茲別克足球會.json
+-rw-r--r--   0     1001      123     7746 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/爆丸.json
+-rw-r--r--   0     1001      123     1968 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/畜牧.json
+-rw-r--r--   0     1001      123      476 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/當個創世神.json
+-rw-r--r--   0     1001      123     4081 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/百變小櫻.json
+-rw-r--r--   0     1001      123     1690 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/科威特职业足球联赛.json
+-rw-r--r--   0     1001      123     4326 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/童話槍手小紅帽.json
+-rw-r--r--   0     1001      123     1287 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/约旦职业足球联赛.json
+-rw-r--r--   0     1001      123    50765 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/美国漫画.json
+-rw-r--r--   0     1001      123      358 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/艾维里奥斯.json
+-rw-r--r--   0     1001      123     4284 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/荷蘭足球聯賽.json
+-rw-r--r--   0     1001      123     5889 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/菁英殺機.json
+-rw-r--r--   0     1001      123     2402 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/葡超.json
+-rw-r--r--   0     1001      123     4186 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/蠟筆小新.json
+-rw-r--r--   0     1001      123      332 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/语言与语音.json
+-rw-r--r--   0     1001      123     4180 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/通靈王.json
+-rw-r--r--   0     1001      123    12331 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/進擊的巨人.json
+-rw-r--r--   0     1001      123      964 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/釣魚臺列嶼.json
+-rw-r--r--   0     1001      123    29385 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/閃電十一人.json
+-rw-r--r--   0     1001      123     2453 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/闇.json
+-rw-r--r--   0     1001      123      919 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/阿曼职业足球联赛.json
+-rw-r--r--   0     1001      123     4315 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/阿联酋职业足球联赛.json
+-rw-r--r--   0     1001      123     2845 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/降世神通.json
+-rw-r--r--   0     1001      123     1889 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/音樂劇.json
+-rw-r--r--   0     1001      123     5499 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/驅魔少年.json
+-rw-r--r--   0     1001      123    14375 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/马来人名地名.json
+-rw-r--r--   0     1001      123    16434 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/鬥陣特攻.json
+-rw-r--r--   0     1001      123     5689 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/魔法咪路咪路.json
+-rw-r--r--   0     1001      123     1103 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/黎巴嫩职业足球联赛.json
+-rw-r--r--   0     1001      123    10818 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/黑執事.json
+-rw-r--r--   0     1001      123     2840 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/黑塔系列.json
+-rw-r--r--   0     1001      123     5472 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/poetry.lock
+-rw-r--r--   0     1001      123      308 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/pyproject.toml
+-rwxr-xr-x   0     1001      123     3645 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/update_basic.py
+-rwxr-xr-x   0     1001      123    12250 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/update_cgroups.py
+-rwxr-xr-x   0     1001      123      857 2023-06-27 06:57:43.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/run-maturin-action.sh
+-rw-r--r--   0     1001      123    30931 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/src/converter.rs
+-rw-r--r--   0     1001      123     4198 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/src/converters.rs
+-rw-r--r--   0     1001      123     9591 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/src/lib.rs
+-rw-r--r--   0     1001      123     2060 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/src/pagerules.rs
+-rw-r--r--   0     1001      123    12790 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/src/rule.rs
+-rw-r--r--   0     1001      123    10529 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/src/tables.rs
+-rw-r--r--   0     1001      123     1217 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/src/utils.rs
+-rw-r--r--   0     1001      123     8918 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/src/variant.rs
+-rw-r--r--   0     1001      123     2880 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/src/wasm.rs
+-rw-r--r--   0     1001      123      342 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/.gitignore
+-rw-r--r--   0     1001      123     2113 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/README.md
+-rw-r--r--   0     1001      123     5266 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/bench.tmp
+-rw-r--r--   0     1001      123     1407 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/config-overrides.js
+-rw-r--r--   0     1001      123     1350 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/package.json
+-rw-r--r--   0     1001      123  3976144 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/public/cgroups.json
+-rw-r--r--   0     1001      123     2159 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/public/index.html
+-rw-r--r--   0     1001      123     3870 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/public/logo.ico
+-rw-r--r--   0     1001      123     5347 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/public/logo192.png
+-rw-r--r--   0     1001      123     9664 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/public/logo512.png
+-rw-r--r--   0     1001      123      475 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/public/manifest.json
+-rw-r--r--   0     1001      123       67 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/public/robots.txt
+-rwxr-xr-x   0     1001      123    23159 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/rustup.sh
+-rw-r--r--   0     1001      123      564 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/App.css
+-rw-r--r--   0     1001      123      273 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/App.test.tsx
+-rw-r--r--   0     1001      123     3332 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/App.tsx
+-rw-r--r--   0     1001      123     4309 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/components/AboutDialog.tsx
+-rw-r--r--   0     1001      123      882 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/components/CGroupCheckbox.tsx
+-rw-r--r--   0     1001      123     6667 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/components/CGroupSelect.tsx
+-rw-r--r--   0     1001      123     4808 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/components/ConvertButton.tsx
+-rw-r--r--   0     1001      123     4230 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/components/Footer.tsx
+-rw-r--r--   0     1001      123     3547 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/components/Header.tsx
+-rw-r--r--   0     1001      123     2720 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/components/InputEditor.tsx
+-rw-r--r--   0     1001      123     3874 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/components/OptionsControl.tsx
+-rw-r--r--   0     1001      123      820 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/components/OutputEditor.tsx
+-rw-r--r--   0     1001      123      552 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/components/OutputStatusLine.tsx
+-rw-r--r--   0     1001      123      217 2023-06-27 06:57:10.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/components/editorCommon.tsx
+-rw-r--r--   0     1001      123      366 2023-06-27 06:57:10.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/index.css
+-rw-r--r--   0     1001      123      500 2023-06-27 06:57:10.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/index.tsx
+-rw-r--r--   0     1001      123     2632 2023-06-27 06:57:10.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/logo.svg
+-rw-r--r--   0     1001      123       40 2023-06-27 06:57:10.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/react-app-env.d.ts
+-rw-r--r--   0     1001      123      425 2023-06-27 06:57:10.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/reportWebVitals.ts
+-rw-r--r--   0     1001      123      241 2023-06-27 06:57:10.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/setupTests.ts
+-rw-r--r--   0     1001      123      150 2023-06-27 06:57:10.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/utils.ts
+-rw-r--r--   0     1001      123      535 2023-06-27 06:57:10.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/tsconfig.json
+-rw-r--r--   0     1001      123   539286 2023-06-27 06:57:10.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/yarn.lock
+-rw-r--r--   0        0        0      597 1970-01-01 00:00:00.000000 zhconv_rs-0.3.0b0/Cargo.toml
+-rw-r--r--   0     1001      123      685 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/.gitignore
+-rw-r--r--   0     1001      123    10364 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/README.md
+-rw-r--r--   0     1001      123      643 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/pyproject.toml
+-rw-r--r--   0     1001      123     5065 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/src/lib.rs
+-rw-r--r--   0     1001      123      758 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/zhconv_rs.pyi
+-rw-r--r--   0     1001      123    23998 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/Cargo.lock
+-rw-r--r--   0        0        0    11135 1970-01-01 00:00:00.000000 zhconv_rs-0.3.0b0/PKG-INFO
```

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/Cargo.toml` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/Cargo.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,56 @@
 [package]
-name = "zhconv"
-version = "0.2.0-beta"
-edition = "2021"
 authors = ["Hung-I Wang <whygowe@gmail.com>"]
+categories = ["text-processing", "localization", "value-formatting", "wasm"]
+description = "Traditional/Simplified and regional Chinese variants converter based on MediaWiki & OpenCC rulesets and powered by AC automata  轉換简体、繁體及兩岸、新馬中文地區詞，基於MediaWiki和OpenCC之字詞轉換表"
+edition = "2021"
 license = "GPL-2.0-or-later"
+name = "zhconv"
 repository = "https://github.com/Gowee/zhconv-rs"
-description = "Traditional/Simplified and regional Chinese variants converter based on MediaWiki & OpenCC rulesets and powered by AC automata  轉換简体、繁體及兩岸、新馬中文地區詞，基於MediaWiki和OpenCC之字詞轉換表"
-categories = ["text-processing", "localization", "value-formatting", "wasm"]
+version = "0.3.0-beta"
 
 [lib]
 crate-type = ["cdylib", "rlib"]
 
 [features]
 # OpenCC rulesets are activated by default.
 # Disabling the feature would boost performance further at the cost of less accuracy.
-default = [ "opencc" ]
-opencc = [ "aho-corasick", "lazy_static" ]
+compress = []
+default = ["opencc", "compress"]
+opencc = ["aho-corasick", "lazy_static"]
 
 [dependencies]
-regex = "1.5"   
-lazy_static = "1.4"
+daachorse = "1.0"
 itertools = "0.10"
-strum = { version = "0.24", features = ["derive"] }
+lazy_static = "1.4"
 once_cell = "1.8"
-aho-corasick = "1.0"
+regex = "1.5"
+ruzstd = {version = "0.4"}
+strum = {version = "0.24", features = ["derive"]}
 
 [target.'cfg(target_arch = "wasm32")'.dependencies]
 wasm-bindgen = "0.2"
 
 # The `console_error_panic_hook` crate provides better debugging of panics by
 # logging them with `console.error`. This is great for development, but requires
 # all the `std::fmt` and `std::panicking` infrastructure, so isn't great for
 # code size when deploying.
-console_error_panic_hook = {version = "0.1"} #, default-features = true, optional = true}
+console_error_panic_hook = {version = "0.1"}#, default-features = true, optional = true}
 
 [build-dependencies]
-sha2 = "0.10"
+aho-corasick = {version = "1.0", optional = true}
+daachorse = "1.0"
 hex-literal = "0.4"
-regex = "1.5"
 itertools = "0.10"
+lazy_static = {version = "1.4", optional = true}
+lz4_flex = "0.10"
 once_cell = "1.8"
-vergen = "8.1"
-lazy_static = { version = "1.4", optional = true }
-aho-corasick = { version = "1.0", optional = true }
+regex = "1.5"
+sha2 = "0.10"
+vergen = {version = "8.2", features = ["build", "git", "gitcl"]}
+zstd = "0.12"
 
 [[bench]]
-name = "zhconv_benchmark"
 harness = false
-
+name = "zhconv_benchmark"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
```

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/.github/workflows/main.yml` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/.github/workflows/npm.yml` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/.github/workflows/npm.yml`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/.github/workflows/pyo3.yml` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/.github/workflows/pyo3.yml`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/.github/workflows/release.yml` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/LICENSE` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/LICENSE`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/README.md` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/README.md`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/benches/25328-0.txt` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/benches/25328-0.txt`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/benches/data3185k.txt` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/benches/data3185k.txt`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/benches/data54k.txt` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/benches/data54k.txt`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/benches/data689k.txt` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/benches/data689k.txt`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/benches/zhconv_benchmark.rs` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/benches/zhconv_benchmark.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,107 @@
 use criterion::{black_box, criterion_group, criterion_main, Criterion};
 
-use zhconv::{tables::*, Variant};
+use zhconv::{converters::deserialize_converter, tables::*, Variant};
 
+const WIKITEXT: &str = include_str!("wikitext.txt");
 const DATA54K: &str = include_str!("data54k.txt");
 const DATA689K: &str = include_str!("data689k.txt");
 const DATA3185K: &str = include_str!("data3185k.txt");
 
+const CONVTUPLES: [(&str, Variant); 8] = [
+    ("zh2Hant", Variant::ZhHant),
+    ("zh2Hans", Variant::ZhHans),
+    ("zh2TW", Variant::ZhTW),
+    ("zh2HK", Variant::ZhHK),
+    ("zh2MO", Variant::ZhMO),
+    ("zh2CN", Variant::ZhCN),
+    ("zh2SG", Variant::ZhSG),
+    ("zh2MY", Variant::ZhMY),
+];
+
 fn criterion_benchmark(c: &mut Criterion) {
-    c.bench_function("build zh-Hant-HK", |b| {
-        b.iter_with_large_drop(|| merge_tables(black_box(ZH_HANT_TABLE), black_box(ZH_HK_TABLE)))
-    });
-    c.bench_function("build zh-Hant-MO", |b| {
-        b.iter_with_large_drop(|| merge_tables(black_box(ZH_HANT_TABLE), black_box(ZH_MO_TABLE)))
-    });
-    c.bench_function("build zh-Hans-CN", |b| {
-        b.iter_with_large_drop(|| merge_tables(black_box(ZH_HANS_TABLE), black_box(ZH_CN_TABLE)))
-    });
-    c.bench_function("build zh-Hans-SG", |b| {
-        b.iter_with_large_drop(|| merge_tables(black_box(ZH_HANS_TABLE), black_box(ZH_SG_TABLE)))
-    });
-    c.bench_function("build zh-Hans-MY", |b| {
-        b.iter_with_large_drop(|| merge_tables(black_box(ZH_HANS_TABLE), black_box(ZH_MY_TABLE)))
-    });
-    c.bench_function("load zh2Hant", |b| {
-        b.iter_with_large_drop(|| build_converter(Variant::Zh, black_box(ZH_HANT_TABLE)))
-    });
-    c.bench_function("load zh2Hans", |b| {
-        b.iter_with_large_drop(|| build_converter(Variant::Zh, black_box(ZH_HANS_TABLE)))
-    });
-    c.bench_function("load zh2TW", |b| {
-        b.iter_with_large_drop(|| build_converter(Variant::Zh, black_box(*ZH_HANT_TW_TABLE)))
-    });
-    c.bench_function("load zh2HK", |b| {
-        b.iter_with_large_drop(|| build_converter(Variant::Zh, black_box(*ZH_HANT_HK_TABLE)))
-    });
-    c.bench_function("load zh2MO", |b| {
-        b.iter_with_large_drop(|| build_converter(Variant::Zh, black_box(*ZH_HANT_MO_TABLE)))
-    });
-    c.bench_function("load zh2CN", |b| {
-        b.iter_with_large_drop(|| build_converter(Variant::Zh, black_box(*ZH_HANS_CN_TABLE)))
-    });
-    c.bench_function("load zh2SG", |b| {
-        b.iter_with_large_drop(|| build_converter(Variant::Zh, black_box(*ZH_HANS_SG_TABLE)))
-    });
-    c.bench_function("load zh2MY", |b| {
-        b.iter_with_large_drop(|| build_converter(Variant::Zh, black_box(*ZH_HANS_MY_TABLE)))
-    });
-    // c.bench_function("load all", |b| {
+    // c.bench_function("build zh-Hant-HK", |b| {
+    //     b.iter_with_large_drop(|| merge_tables(black_box(ZH_HANT_TABLE), black_box(ZH_HK_TABLE)))
+    // });
+    // c.bench_function("build zh-Hant-MO", |b| {
+    //     b.iter_with_large_drop(|| merge_tables(black_box(ZH_HANT_TABLE), black_box(ZH_MO_TABLE)))
+    // });
+    // c.bench_function("build zh-Hans-CN", |b| {
+    //     b.iter_with_large_drop(|| merge_tables(black_box(ZH_HANS_TABLE), black_box(ZH_CN_TABLE)))
+    // });
+    // c.bench_function("build zh-Hans-SG", |b| {
+    //     b.iter_with_large_drop(|| merge_tables(black_box(ZH_HANS_TABLE), black_box(ZH_SG_TABLE)))
+    // });
+    // c.bench_function("build zh-Hans-MY", |b| {
+    //     b.iter_with_large_drop(|| merge_tables(black_box(ZH_HANS_TABLE), black_box(ZH_MY_TABLE)))
+    // });
+
+    // c.bench_function("test", |b| {
     //     b.iter_with_large_drop(|| {
-    //         (
-    //             make_converter(black_box(ZH_HANS_TABLE)),
-    //             make_converter(black_box(ZH_HANT_TABLE)),
-    //             make_converter(black_box(ZH_CN_TABLE)),
-    //             make_converter(black_box(ZH_HK_TABLE)),
-    //             make_converter(black_box(ZH_TW_TABLE)),
-    //         )
+    //         black_box(zhconv::tables::daac())
     //     })
-    // });
+    // });//lz4_flex::compress_prepend_size
+    {
+        // let mut build = c.benchmark_group("build-from-scratch");
+        // for (name, variant) in CONVTUPLES {
+        //     build.bench_function(name, |b| {
+        //         b.iter_with_large_drop(|| {
+        //             build_converter(variant, black_box(get_builtin_table(variant)))
+        //         })
+        //     });
+        // }
 
+        // c.bench_function("build all from scratch", |b| {
+        //     b.iter_with_large_drop(|| {
+        //         (
+        //             make_converter(black_box(ZH_HANS_TABLE)),
+        //             make_converter(black_box(ZH_HANT_TABLE)),
+        //             make_converter(black_box(ZH_CN_TABLE)),
+        //             make_converter(black_box(ZH_HK_TABLE)),
+        //             make_converter(black_box(ZH_TW_TABLE)),
+        //         )
+        //     })
+        // });
+    }
+
+    {
+        let tag = if cfg!(feature = "compress") {
+            "load-compressed-serialized"
+        } else {
+            "load-serialized"
+        };
+        let mut load = c.benchmark_group(tag);
+        for (name, variant) in CONVTUPLES {
+            load.bench_function(name, |b| {
+                b.iter_with_large_drop(|| {
+                    deserialize_converter(
+                        variant,
+                        black_box(get_builtin_serialized_daac(variant)),
+                        black_box(get_builtin_tables(variant).iter().cloned()),
+                    )
+                })
+            });
+        }
+    }
+
+    c.bench_function("zh2CN wikitext basic", |b| {
+        b.iter_with_large_drop(|| {
+            zhconv::converters::ZH_TO_CN_CONVERTER.convert_as_wikitext_basic(WIKITEXT)
+        })
+    });
+    c.bench_function("zh2TW wikitext basic", |b| {
+        b.iter_with_large_drop(|| {
+            zhconv::converters::ZH_TO_TW_CONVERTER.convert_as_wikitext_basic(WIKITEXT)
+        })
+    });
+    c.bench_function("zh2TW wikitext extended", |b| {
+        b.iter_with_large_drop(|| {
+            zhconv::converters::ZH_TO_TW_CONVERTER.convert_as_wikitext_extended(WIKITEXT)
+        })
+    });
     c.bench_function("zh2CN 天乾物燥", |b| {
         b.iter_with_large_drop(|| zhconv::converters::ZH_TO_CN_CONVERTER.convert("天乾物燥"))
     });
     c.bench_function("zh2TW data54k", |b| {
         b.iter_with_large_drop(|| zhconv::converters::ZH_TO_TW_CONVERTER.convert(DATA54K))
     });
     c.bench_function("zh2CN data54k", |b| {
```

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/build.rs` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/src/rule.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,366 +1,400 @@
+//! Structs and functions for processing conversion rule, as is defined in [ConverterRule.php](https://doc.wikimedia.org/mediawiki-core/master/php/ConverterRule_8php.html).
+//!
+//! **Note**: This module is not stable yet and just exposed for convenience. It might have
+//! breaking changes at any time in violation of semver.
+
 use std::collections::HashMap;
-use std::collections::HashSet;
-use std::convert::TryInto;
-use std::env;
-use std::fs::{self, File};
-use std::io::Write;
-use std::path::Path;
-
-use hex_literal::hex;
-use itertools::Itertools;
-use regex::Regex;
-use sha2::{Digest, Sha256};
-use vergen::EmitBuilder;
-
-#[cfg(feature = "opencc")]
-use self::opencc::load_opencc_to;
-
-// To update upstream dataset: manually update commits here and run data/update_basic.py
-const MEDIAWIKI_COMMIT: &str = "bcaab3d057c8e550793100448f725761e1a8e017";
-const MEDIAWIKI_SHA256: [u8; 32] =
-    hex!("37c17b6361ab774b0b7dab801aa7ff919f8efa6e2ad3f66ccb051e9c1a848f6e");
-
-#[cfg(feature = "opencc")]
-const OPENCC_COMMIT: &str = "5750d92a92ac1f2d64c880c1f6f1a5e382d7d199";
-#[cfg(feature = "opencc")]
-const OPENCC_SHA256: [(&str, [u8; 32]); 11] = [
-    (
-        "HKVariants.txt",
-        hex!("c3c93c35885902ba2b12a3235a7761b00fb2b027f36aa8314db2f6b6ad51d374"),
-    ),
-    (
-        "HKVariantsRevPhrases.txt",
-        hex!("c2da309afa7fdd9061f204664039d33b000a4dca0ecae4e7480dcbf9e20f658e"),
-    ),
-    (
-        "STCharacters.txt",
-        hex!("9207708da9f2e2a248f39c457b2fccad26ec42e7efaf47a860e6900464f4cac5"),
-    ),
-    (
-        "STPhrases.txt",
-        hex!("a4de4d2471f73cdb7e5b1b22920139aa4e4bbb1ebeea8f1fc341f988aa75c586"),
-    ),
-    (
-        "TSCharacters.txt",
-        hex!("6b5a0a799bea2bb22c001f635eaa3fc2904310f0c08addbff275477a80ecf09a"),
-    ),
-    (
-        "TSPhrases.txt",
-        hex!("b2ef895dd4953b4bb77fc8ef8d26a2a9ca6d43a760ed9a1d767672cfafa6324f"),
-    ),
-    (
-        "TWPhrasesIT.txt",
-        hex!("8a129130a10c57278485c4b7a81c4c74a8242239576018d9bfd2149e2d3c2af6"),
-    ),
-    (
-        "TWPhrasesName.txt",
-        hex!("76e643569a30ea54e7ab6e52621fd4c396e01ee6dc2d15b7d25bf23addf4438a"),
-    ),
-    (
-        "TWPhrasesOther.txt",
-        hex!("06d9e1a24b1f87431e029d38cdf67a35d32b96a08df736cf1a362477dd39f7c7"),
-    ),
-    (
-        "TWVariants.txt",
-        hex!("30e6f8395edbfdd74e293fd8b9c62105d787c849fbb208d2a7832eac696734d7"),
-    ),
-    (
-        "TWVariantsRevPhrases.txt",
-        hex!("bef60ceb4e57b6b062351406cb5d4644875574231d64787e03711317b7e773f3"),
-    ),
-];
-
-fn main() {
-    let out_dir = env::var_os("OUT_DIR").unwrap();
-
-    let zhconv = read_and_validate_file("data/ZhConversion.php", &MEDIAWIKI_SHA256);
-    let zhconvs = parse_mediawiki(&zhconv);
-    for (name, pairs) in zhconvs.iter() {
-        let mut pairs = pairs.clone();
-        // Load and append OpenCC rulesets to the Mediawiki ones
-        // ref: https://github.com/BYVoid/OpenCC/blob/29d33fb8edb8c95e34691c8bd1ef76a50d0b5251/data/config/
-
-        // Note: OpenCC conversion procededures take multi-pass for chaining rulesets.
-        // For efficiency and re-using the existing implementation, we chain the rulesets
-        // straightforward by chaining conversion pairs at different level in advance.
-        // It may result in conversion results different to the stock OpenCC implementation
-        // considering that some conversion pairs span over the border of several natural phrases
-        // while not covering them in whole.
-        #[cfg(feature = "opencc")]
-        match name.as_ref() {
-            "zh2Hans" => {
-                // hk2s & tw2s & t2s
-                load_opencc_to!(
-                    &mut pairs,
-                    [HKVariantsRevPhrases, !HKVariants],
-                    [TSCharacters, TSPhrases]
-                );
-                load_opencc_to!(
-                    &mut pairs,
-                    [TWVariantsRevPhrases, !TWVariants],
-                    [TSCharacters, TSPhrases]
-                );
-            }
-            "zh2Hant" => {
-                // s2t & hk2t & tw2t
-                load_opencc_to!(&mut pairs, [HKVariantsRevPhrases, !HKVariants]);
-                load_opencc_to!(&mut pairs, [TWVariantsRevPhrases, !TWVariants]);
-                load_opencc_to!(&mut pairs, [STCharacters, STPhrases]);
-            }
-            "zh2TW" => {
-                // s2twp & t2tw
-                load_opencc_to!(
-                    &mut pairs,
-                    [STPhrases, STCharacters],
-                    [TWPhrasesIT, TWPhrasesName, TWPhrasesOther],
-                    [TWVariants]
-                );
-            }
-            "zh2HK" => {
-                // s2hk & t2hk
-                load_opencc_to!(&mut pairs, [STPhrases, STCharacters], [HKVariants]);
-            }
-            "zh2MO" => {}
-            "zh2CN" => {
-                // tw2sp & hk2s
-                load_opencc_to!(
-                    &mut pairs,
-                    [
-                        !TWPhrasesIT,
-                        !TWPhrasesName,
-                        !TWPhrasesOther,
-                        TWVariantsRevPhrases,
-                        !TWVariants
-                    ],
-                    [TSPhrases, TSCharacters]
-                );
-                load_opencc_to!(
-                    &mut pairs,
-                    [HKVariantsRevPhrases, !HKVariants],
-                    [TSPhrases, TSCharacters]
-                );
-            }
-            "zh2SG" => {}
-            "zh2MY" => {}
-            _ => (),
-        }
-
-        let dest_path_from = Path::new(&out_dir).join(format!("{}.from.conv", name));
-        let dest_path_to = Path::new(&out_dir).join(format!("{}.to.conv", name));
-        let mut ffrom = File::create(dest_path_from).unwrap();
-        let mut fto = File::create(dest_path_to).unwrap();
-
-        // longer phrases come first; lexicographically smaller phrases come first
-        pairs.sort_by(|a, b| b.0.len().cmp(&a.0.len()).then(a.0.cmp(&b.0)));
-        pairs.dedup_by(|a, b| a.0 == b.0);
-
-        assert_eq!(
-            pairs.len(),
-            pairs
-                .iter()
-                .map(|(from, _to_)| from)
-                .collect::<HashSet<_>>()
-                .len(),
-            "deduping keys of {}",
-            name
-        );
+use std::convert::AsRef;
+use std::fmt::{self, Display};
+use std::iter::{self, Map};
+use std::str::FromStr;
+
+use once_cell::sync::Lazy;
+use regex::{Match, Matches, Regex};
+
+use crate::variant::{Variant, VariantMap};
+
+/// A single rule used for language conversion, usually extracted from wikitext in the syntax `-{ }-`.
+///
+/// Ref: [ConverterRule.php](https://doc.wikimedia.org/mediawiki-core/master/php/ConverterRule_8php.html)
+/// and [Help:高级字词转换语法](https://zh.wikipedia.org/wiki/Help:%E9%AB%98%E7%BA%A7%E5%AD%97%E8%AF%8D%E8%BD%AC%E6%8D%A2%E8%AF%AD%E6%B3%95)
+/// (not fully compliant)
+#[derive(Debug, Clone)]
+pub struct ConvRule {
+    pub(crate) action: Option<Action>,
+    pub(crate) output: Option<Output>,
+    pub(crate) conv: Option<Conv>,
+    pub(crate) set_title: bool,
+}
 
-        for e in Itertools::intersperse(pairs.iter().map(|(from, _to)| from.as_str()), "|") {
-            write!(ffrom, "{}", e).unwrap();
-        }
-        for e in Itertools::intersperse(pairs.iter().map(|(_from, to)| to.as_str()), "|") {
-            write!(fto, "{}", e).unwrap();
+#[derive(Debug, Clone)]
+pub struct ConvRuleWithVariant<'r> {
+    rule: &'r ConvRule,
+    variant: Variant,
+}
+
+#[derive(Debug, Clone, PartialEq, Eq)]
+pub enum Output {
+    Normal,
+    VariantName(Variant),
+    Description,
+}
+
+#[derive(Debug, Copy, Clone, PartialEq, Eq)]
+pub enum Action {
+    Add,
+    Remove,
+}
+
+#[derive(Debug, Copy, Clone, PartialEq, Eq)]
+pub enum RuleError {
+    InvalidFlag(char),
+    InvalidConv,
+    InvalidConvForTitle,
+    InvalidVariant,
+}
+
+impl ConvRule {
+    pub fn targeted(&self, target: Variant) -> ConvRuleWithVariant {
+        ConvRuleWithVariant {
+            rule: self,
+            variant: target,
         }
     }
 
-    if std::env::var("DOCS_RS").is_err() {
-        // vergen panics in docs.rs. It is only used by wasm.rs for now.
-        // So it is ok to disable it in docs.rs.
-
-        // Note: conditional compilation tricks won't be effective since it is cross compiling here.
-        // Ref:
-        //   https://kazlauskas.me/entries/writing-proper-buildrs-scripts
-        //   https://github.com/rust-lang/cargo/issues/4302
-        // #[cfg(target_arch = "wasm32")] #[cfg(all(target_arch = "wasm32", target_os = "unknown"))]
-        if env::var("CARGO_CFG_TARGET_ARCH") == Ok("wasm32".to_owned()) {
-            EmitBuilder::builder()
-                .emit()
-                .unwrap_or_else(|e| println!("cargo:warning=vergen failed: {:?}", e));
+    pub fn into_conv_action(self) -> Option<ConvAction> {
+        if let (Some(action), Some(conv)) = (self.action, self.conv) {
+            Some(ConvAction(action, conv))
+        } else {
+            None
         }
     }
-    println!("cargo:rustc-env=MEDIAWIKI_COMMIT_HASH={}", MEDIAWIKI_COMMIT);
-    #[cfg(feature = "opencc")]
-    println!("cargo:rustc-env=OPENCC_COMMIT_HASH={}", OPENCC_COMMIT);
-    println!("cargo:rerun-if-changed=build.rs");
-    println!("cargo:rerun-if-changed=data/ZhConversion.php");
-    #[cfg(feature = "opencc")]
-    for (opencc, _) in OPENCC_SHA256.iter() {
-        println!("cargo:rerun-if-changed=data/{}", opencc);
+
+    /// Same as `from_str`, except that any unrecognized rule is treated as [`Conv::Asis`]
+    pub fn from_str_infallible(s: &str) -> ConvRule {
+        s.parse().unwrap_or_else(|_| ConvRule {
+            action: None,
+            output: Some(Output::Normal),
+            conv: Some(Conv::Asis(s.to_owned())),
+            set_title: true,
+        })
     }
-    println!("cargo:rerun-if-changed=Cargo.toml");
 }
 
-fn parse_mediawiki(text: &str) -> HashMap<String, Vec<(String, String)>> {
-    let patb = Regex::new(r"public static \$(\w+) = \[([^]]+)\]?;").unwrap();
-    let patl = Regex::new(r"'(.+?)' *=> *'(.+?)' *,?\n").unwrap();
-    let mut res = HashMap::new();
+impl FromStr for ConvRule {
+    type Err = RuleError;
 
-    for block in patb.captures_iter(text) {
-        let name = block.get(1).unwrap().as_str();
-        let body = block.get(2).unwrap().as_str();
-        let mut pairs = vec![];
-        for line in patl.captures_iter(body) {
-            let from = line.get(1).unwrap().as_str();
-            let to = line.get(2).unwrap().as_str();
-            pairs.push((from.to_owned(), to.to_owned()));
+    fn from_str(s: &str) -> Result<Self, Self::Err> {
+        let (flags, body) = s.find('|').map_or_else(
+            || ("", s),
+            |i| {
+                let (first, last) = s.split_at(i);
+                (first, &last[1..])
+            },
+        );
+        let mut set_title = false;
+        let mut action = None;
+        let mut output = Some(Output::Normal);
+        // Ref: https://github.com/wikimedia/mediawiki/blob/7bf779524ab1fd8e1d74f79ea4840564d48eea4d/includes/language/LanguageConverter.php#L158
+        //  and https://github.com/wikimedia/mediawiki/blob/ec6fd491074a6ace5ccc7bc05b01c30512a5723d/includes/language/ConverterRule.php#L408
+        //  (not fully compliant, especially for multi-flags cases)
+        for flag in flags.chars() {
+            match flag {
+                // FIX: 'A'
+                '+' => action = Some(Action::Add),
+                '-' => action = Some(Action::Remove),
+                // no conv, just display the inner as-is
+                'R' => {
+                    return Ok(ConvRule {
+                        action: None,
+                        output: Some(Output::Normal),
+                        conv: Some(Conv::Asis(body.to_owned())),
+                        set_title: false,
+                    });
+                }
+                // output the variant name of the context
+                'N' => {
+                    output = Some(Output::VariantName(
+                        Variant::from_str(body).map_err(|_| RuleError::InvalidVariant)?,
+                    ));
+                }
+                // Display the rule **D**escription
+                'D' => {
+                    output = Some(Output::Description);
+                }
+                // add a global rule without displaying anything (**H**idden)
+                'H' => {
+                    action = Some(Action::Add);
+                    output = None;
+                }
+                // display as normal (by default)
+                'S' => {}
+                // add a global rule; A implies +S
+                'A' => action = Some(Action::Add),
+                // convert the title of some an article
+                'T' => {
+                    set_title = true;
+                    output = None
+                }
+                unknown => return Err(RuleError::InvalidFlag(unknown)),
+            }
+        }
+        let conv = if let Some(Output::VariantName(_)) = output {
+            None
+        } else {
+            Some(Conv::from_str(body).map_err(|_| RuleError::InvalidConv)?)
+        };
+        if set_title
+            && conv
+                .as_ref()
+                .and_then(|c| c.get_bid())
+                .map(|b| !b.is_empty())
+                != Some(true)
+        {
+            return Err(RuleError::InvalidConvForTitle);
+        }
+        Ok(Self {
+            action,
+            output,
+            conv,
+            set_title,
+        })
+    }
+}
+
+impl<'r> Display for ConvRuleWithVariant<'r> {
+    fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
+        let rule = self.rule;
+        match &rule.output {
+            None => Ok(()),
+            Some(Output::Normal) => write!(
+                f,
+                "{}",
+                rule.conv
+                    .as_ref()
+                    .and_then(|c| c.get_text_by_target(self.variant))
+                    .unwrap_or("") // mediawiki would show: 在手动语言转换规则中检测到错误
+            ),
+            Some(Output::VariantName(variant)) => write!(f, "{}", variant.get_name()),
+            Some(Output::Description) => {
+                if let Some(conv) = rule.conv.as_ref() {
+                    write!(f, "{}", conv)
+                } else {
+                    Ok(())
+                }
+            }
         }
-        assert!(res.insert(name.to_owned(), pairs).is_none());
     }
-    res
 }
 
-#[cfg(feature = "opencc")]
-mod opencc {
-    use aho_corasick::{AhoCorasick, AhoCorasickBuilder, MatchKind};
-    use lazy_static::lazy_static;
-    use std::collections::HashMap;
+/// The inner of a [`ConvRule`] without flags and actions
+///
+/// A single `Conv` may consist of multiple uni-directional and/or bi-diretional mappings in any
+/// order. e.g.,
+/// uni-directional mapping: `巨集=>zh-cn:宏;`,
+/// bi-directional mapping: `zh-hans:计算机; zh-hant:電腦;`,
+/// mixed: `zh-hk:橘;zh-tw:芭樂;蘋果=>zh-cn:梨;`.
+///
+/// Or it can be an as-is text which prevents such text being converted by other rules. Typically,
+/// it helps avoid over-conversion applied to surnames. Be noted that it might not be effective in
+/// rare cases due to the leftmost-longest matching strategy.
+#[derive(Debug, Clone)]
+pub enum Conv {
+    Asis(String),
+    Map(ConvMap),
+}
 
-    use super::OPENCC_SHA256;
+#[derive(Debug, Clone)]
+pub struct ConvMap {
+    pub bid: VariantMap<String>,
+    pub unid: VariantMap<Vec<(String, String)>>,
+}
 
-    lazy_static! {
-        pub static ref OPENCC_SHA256_MAP: HashMap<String, [u8; 32]> = OPENCC_SHA256
-            .into_iter()
-            .map(|(n, s)| (n.to_owned(), s))
-            .collect();
+impl Conv {
+    #[inline]
+    /// The text to display for the target variant
+    pub fn get_text_by_target(&self, target: Variant) -> Option<&str> {
+        use Conv::*;
+        match self {
+            Asis(s) => Some(s),
+            Map(m) => m.bid.get_text_with_fallback(target),
+        }
     }
 
-    macro_rules! load_opencc_to {
-        ( @read_to $out_conv: expr, $out_revconv: expr, $name: ident) => {
-            let s = read_and_validate_file(concat!("data/", stringify!($name), ".txt"), crate::opencc::OPENCC_SHA256_MAP.get(stringify!($name.txt)).expect(stringify!($name.txt not found)));
-            crate::opencc::parse_opencc_to($out_conv, $out_revconv, &s);
-        };
-        ( @parse_to $out_conv: expr, $out_revconv: expr, $name: ident, $($remainings: tt)* ) => {
-            load_opencc_to!(@read_to $out_conv, $out_revconv, $name);
-            load_opencc_to!(@parse_to $out_conv, $out_revconv, $($remainings)*);
-        };
-        ( @parse_to $out_conv: expr, $out_revconv: expr, $name: ident ) => {
-            load_opencc_to!(@read_to $out_conv, $out_revconv, $name);
-        };
-        ( @parse_to $out_conv: expr, $out_revconv: expr, ! $name: ident, $($remainings: tt)* ) => {
-            load_opencc_to!(@read_to $out_revconv, $out_conv, $name);
-            load_opencc_to!(@parse_to $out_conv, $out_revconv, $($remainings)*);
-        };
-        ( @parse_to $out_conv: expr, $out_revconv: expr, ! $name: ident ) => {
-            load_opencc_to!(@read_to $out_revconv, $out_conv, $name);
-        };
-        ( @load_stage $out: expr, $prev_stage: ident, [ $($rule: tt)+ ] ) => {
-            let (mut prev_convs, prev_revconvs): (HashMap<String, String>, HashMap<String, String>) = $prev_stage.unwrap_or_else(|| (HashMap::new(), HashMap::new()));
-            let mut convs: HashMap<String, String> = HashMap::new();
-            let mut revconvs: HashMap<String, String> = HashMap::new();
-            load_opencc_to!(@parse_to &mut convs, &mut revconvs, $($rule)*);
-            let conver: crate::opencc::SimpleConverter = convs.clone().into();
-            let prev_revconver: crate::opencc::SimpleConverter = prev_revconvs.clone().into();
-            for (_f, t) in prev_convs.iter_mut() {
-                *t = conver.convert(t);
-            }
-            for (f, t) in convs.iter() {
-                prev_convs.insert(f.clone(), t.clone());
-                let ff = prev_revconver.convert(f);
-                if &ff != f && &ff != t /* ? */ {
-                    prev_convs.insert(ff.to_owned(), t.to_owned());
-                }
-            }
-            for (_f, t) in revconvs.iter_mut() {
-                *t = prev_revconver.convert(t);
+    pub fn get_conv_pairs(&self, target: Variant) -> impl Iterator<Item = (&str, &str)> {
+        let mut mit = self
+            .as_map()
+            .map(|m| {
+                m.bid.get_conv_pairs(target).chain(
+                    m.unid
+                        .get_conv_pairs(target)
+                        .iter()
+                        .map(|(f, t)| (f.as_ref(), t.as_ref())),
+                )
+            })
+            .into_iter()
+            .flatten()
+            .filter(|(f, _t)| !f.is_empty()); // filter out emtpy froms that troubles AC
+        let mut maybe_asis = self.as_asis().map(|s| Some((s, s)));
+
+        iter::from_fn(move || {
+            if let Some(asis_yielding) = maybe_asis.as_mut() {
+                asis_yielding.take()
+            } else {
+                mit.next()
             }
-            revconvs.extend(prev_revconvs.iter().map(|(f, t)| (conver.convert(f), t.to_owned())));
-            revconvs.extend(prev_revconvs.iter().map(|(f, t)| (f.to_owned(), t.to_owned())));
-            $prev_stage = Some((prev_convs, revconvs));
-        };
-        ( $out: expr, $($stage: tt),+ ) => {
-            let mut prev_stage = None;
-            $(load_opencc_to!(@load_stage $out, prev_stage, $stage);)*
-            let (convs, _) = prev_stage.unwrap();
-            $out.extend(convs.into_iter());
-        };
+        })
     }
-    pub(crate) use load_opencc_to;
 
-    pub fn parse_opencc_to(
-        out_conv: &mut HashMap<String, String>,
-        out_revconv: &mut HashMap<String, String>,
-        s: &str,
-    ) {
-        for line in s.lines().map(|l| l.trim()).filter(|l| !l.is_empty()) {
-            let mut it = line.split_whitespace();
-            if let (Some(f), Some(t)) = (it.next(), it.next()) {
-                out_conv.insert(f.to_owned(), t.to_owned());
-                out_revconv.insert(t.to_owned(), f.to_owned());
-                for tt in it {
-                    out_revconv.insert(tt.to_owned(), f.to_owned());
-                }
-            }
+    pub fn as_asis(&self) -> Option<&str> {
+        use Conv::*;
+        match self {
+            Asis(s) => Some(s.as_ref()),
+            _ => None,
         }
     }
 
-    /// Simplified `ZhConverter` implementation for pre-processing rulesets from OpenCC
-    pub struct SimpleConverter {
-        automaton: AhoCorasick,
-        mapping: HashMap<String, String>,
-    }
-
-    impl From<HashMap<String, String>> for SimpleConverter {
-        fn from(mapping: HashMap<String, String>) -> Self {
-            let automaton = AhoCorasickBuilder::new()
-                .match_kind(MatchKind::LeftmostLongest)
-                .build(mapping.keys())
-                .unwrap();
-            Self { automaton, mapping }
+    pub fn as_map(&self) -> Option<&ConvMap> {
+        use Conv::*;
+        match self {
+            Map(m) => Some(m),
+            _ => None,
         }
     }
 
-    impl SimpleConverter {
-        #[allow(dead_code)]
-        pub fn build<'s>(pairs: impl Iterator<Item = (&'s str, &'s str)>) -> Self {
-            let mapping = HashMap::from_iter(pairs.map(|(a, b)| (a.to_owned(), b.to_owned())));
-            mapping.into()
-        }
-
-        pub fn convert(&self, text: &str) -> String {
-            let mut output = String::new();
-            let mut last = 0;
-            // leftmost-longest matching
-            for (s, e) in self.automaton.find_iter(text).map(|m| (m.start(), m.end())) {
-                if s > last {
-                    output.push_str(&text[last..s]);
+    /// Get the inner bi-directional map, if any.
+    ///
+    /// Typically intended to be used by [`PageRules`](crate::pagerules:PageRules) to extract the
+    /// map for a page title (e.g. `-{T|zh:黑;zh-cn:白}-`).
+    pub fn get_bid(&self) -> Option<&VariantMap<String>> {
+        self.as_map().map(|m| &m.bid)
+    }
+
+    /// Same as `from_str`, except that any unrecognized conv is treated as [`Conv::Asis`]
+    pub fn from_str_infallible(s: &str) -> Conv {
+        s.parse().unwrap_or_else(|_| Conv::Asis(s.to_owned()))
+    }
+}
+
+impl Display for Conv {
+    fn fmt(&self, fmt: &mut fmt::Formatter) -> fmt::Result {
+        use Conv::*;
+        match self {
+            Asis(s) => write!(fmt, "{}", s),
+            Map(m) => {
+                write!(fmt, "{}{}", m.bid, m.unid)
+            }
+        }
+    }
+}
+
+impl FromStr for Conv {
+    type Err = ();
+
+    fn from_str(s: &str) -> Result<Conv, Self::Err> {
+        let s = s.trim();
+        if s.is_empty() {
+            // TODO: return?
+        }
+        let mut bid = HashMap::new();
+        let mut unid = HashMap::new();
+        // TODO: implement a clean iterator instead
+        let mut parse_single = |s: &str| -> Result<(), Self::Err> {
+            if s.trim().is_empty() {
+                return Ok(());
+            };
+            let (left, right) = s.find("=>").map_or_else(
+                || (None, s),
+                |i| {
+                    assert!(0 < i && i < s.len());
+                    let (first, last) = s.split_at(i);
+                    (Some(first), &last[2..])
+                },
+            );
+            let (variant, to) = right.split_at(right.find(':').ok_or(())?);
+            let to = &to[1..]; // strip ":"
+            let variant = variant.trim().parse::<Variant>().map_err(|_| ())?;
+            if let Some(from) = left {
+                if from.is_empty() {
+                    return Err(()); // e.g. {EMPTY}=>zh:foobar
+                }
+                unid.entry(variant)
+                    .or_insert_with(Vec::new)
+                    .push((from.to_owned(), to.to_owned()));
+            } else {
+                bid.insert(variant, to.to_owned());
+            }
+            Ok(())
+        };
+        let mut i = 0;
+        let mut ampersand = None; // handle entity escape
+        for (j, &c) in s.as_bytes().iter().enumerate() {
+            match c {
+                b'&' => {
+                    ampersand = Some(j);
+                    // if ampersand, the new & is the new start
+                }
+                b';' => {
+                    if !(ampersand.is_some() && j - ampersand.unwrap() > 1) {
+                        parse_single(&s[i..j])?;
+                        i = j + 1;
+                    }
+                }
+                _ => {
+                    if ampersand.is_some() & !(b'#' == c || char::from(c).is_ascii_alphanumeric()) {
+                        ampersand = None;
+                    }
                 }
-                output.push_str(self.mapping.get(&text[s..e]).unwrap());
-                last = e;
             }
-            output.push_str(&text[last..]);
-            output
         }
+        if i != s.as_bytes().len() && parse_single(&s[i..]).is_err() {
+            if bid.is_empty() && unid.is_empty() {
+                return Ok(Conv::Asis(s.to_owned()));
+            } else {
+                return Err(());
+                // Or we just discard this part?
+            }
+        }
+        Ok(Conv::Map(ConvMap {
+            bid: bid.into(),
+            unid: unid.into(),
+        }))
+    }
+}
+
+/// A `([Action], [Conv])` pair with some helper methods
+#[derive(Debug, Clone)]
+pub struct ConvAction(Action, Conv);
+
+impl ConvAction {
+    pub fn is_add(&self) -> bool {
+        self.0 == Action::Add
+    }
+
+    pub fn is_remove(&self) -> bool {
+        self.0 == Action::Remove
+    }
+
+    pub fn as_conv(&self) -> &Conv {
+        &self.1
     }
 }
 
-fn read_and_validate_file(path: &str, sha256sum: &[u8; 32]) -> String {
-    let data_dir = env::var_os("CARGO_MANIFEST_DIR").unwrap();
-    let path = Path::new(&data_dir).join(path);
-    let content = String::from_utf8(
-        fs::read(&path).unwrap_or_else(|e| panic!("{} when reading {}", e, path.display())),
-    )
-    .unwrap_or_else(|e| panic!("{} is not in valid UTF-8 ({})", path.display(), e));
-    assert_eq!(
-        &sha256(&content),
-        sha256sum,
-        "Validating the checksum of {}",
-        path.display()
-    );
-    content
-}
-
-fn sha256(text: &str) -> [u8; 32] {
-    let mut hasher = Sha256::new();
-    hasher.update(text.as_bytes());
-    hasher.finalize().try_into().unwrap()
+impl AsRef<Conv> for ConvAction {
+    fn as_ref(&self) -> &Conv {
+        &self.1
+    }
+}
+
+static REGEX_RULE: Lazy<Regex> = Lazy::new(|| Regex::new(r"-\{.+?\}-").unwrap());
+
+/// Extract a set rules from a text.
+pub fn extract_rules<'s>(
+    text: &'s str,
+) -> Map<Matches<'static, 's>, impl FnMut(Match<'s>) -> Result<ConvRule, RuleError>> {
+    // note: the regex works a little differently from the parser in converter
+    (*REGEX_RULE).find_iter(text).map(|m| {
+        let rule = m.as_str();
+        ConvRule::from_str(&rule[2..rule.len() - 2])
+    })
 }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/HKVariants.txt` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/HKVariants.txt`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/HKVariantsRevPhrases.txt` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/HKVariantsRevPhrases.txt`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/README.md` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/README.md`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/STCharacters.txt` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/STCharacters.txt`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/STPhrases.txt` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/STPhrases.txt`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/TSCharacters.txt` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/TSCharacters.txt`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/TSPhrases.txt` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/TSPhrases.txt`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/TWPhrasesIT.txt` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/TWPhrasesIT.txt`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/TWPhrasesName.txt` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/TWPhrasesName.txt`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/TWPhrasesOther.txt` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/TWPhrasesOther.txt`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/TWVariantsRevPhrases.txt` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/TWVariantsRevPhrases.txt`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/ZhConversion.php` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/ZhConversion.php`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/1D.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/1D.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/2016年太平洋颱風季.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/2016年太平洋颱風季.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/2017年太平洋颱風季.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/2017年太平洋颱風季.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/2018年太平洋颱風季.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/2018年太平洋颱風季.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/2019年太平洋颱風季.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/2019年太平洋颱風季.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/2020年太平洋颱風季.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/2020年太平洋颱風季.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/2021年太平洋颱風季.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/2021年太平洋颱風季.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/2022年太平洋颱風季.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/2022年太平洋颱風季.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/24.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/24.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/A Pink.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/A Pink.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/A Song of Ice and Fire.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/A Song of Ice and Fire.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/ACmilan.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/ACmilan.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/ALeague.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/ALeague.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/AT Places.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/AT Places.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/AU Places.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/AU Places.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Adventure Time.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Adventure Time.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Aero.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Aero.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Aikatsu.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Aikatsu.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Anime.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Anime.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Apple.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Apple.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Aquatics.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Aquatics.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Ariana Grande.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Ariana Grande.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Artist.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Artist.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Astronomy.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Astronomy.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Avatar.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Avatar.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Avril Lavigne.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Avril Lavigne.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/BE Places.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/BE Places.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/BUDDYCOMPLEX.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/BUDDYCOMPLEX.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Badminton.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Badminton.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Bakuman.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Bakuman.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Battle Spirits.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Battle Spirits.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Bird.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Bird.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/BirdG.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/BirdG.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/BirdP.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/BirdP.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Black Mirror.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Black Mirror.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Bridge.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Bridge.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Britney Spears.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Britney Spears.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Bundesliga.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Bundesliga.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Butterfly.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Butterfly.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/C&C.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/C&C.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/CA Places.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/CA Places.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/CANAAN.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/CANAAN.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/CH Places.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/CH Places.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/COD.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/COD.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/CWBTyphoonOld.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/CWBTyphoonOld.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Canada.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Canada.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Carnivorous Plant.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Carnivorous Plant.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Cartoon.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Cartoon.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Chanel.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Chanel.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Chemistry.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Chemistry.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Code Black.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Code Black.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Code Geass.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Code Geass.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/CodeLyoko.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/CodeLyoko.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Coldplay.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Coldplay.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Communication.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Communication.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Composer.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Composer.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Copyright.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Copyright.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Counter-Strike.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Counter-Strike.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Crazyracing Kartrider.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Crazyracing Kartrider.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Cyber Formula.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Cyber Formula.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Cyclone.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Cyclone.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/DCComics.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/DCComics.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/DE Places.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/DE Places.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Danball Senki.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Danball Senki.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Dance.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Dance.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Death Note.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Death Note.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Diablo.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Diablo.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Die Weiße Rose.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Die Weiße Rose.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Digimon.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Digimon.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Disney.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Disney.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Doctor Who.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Doctor Who.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Doraemon.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Doraemon.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/DragonBall.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/DragonBall.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/DreamWorks.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/DreamWorks.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/ED.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/ED.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/EPL.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/EPL.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/EU.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/EU.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Earthquake.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Earthquake.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Ecology.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Ecology.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Economics.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Economics.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Electronics.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Electronics.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Esports.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Esports.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Eyeshield21.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Eyeshield21.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/F1.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/F1.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/FAcup.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/FAcup.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/FR Places.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/FR Places.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Family Guy.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Family Guy.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Firearms.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Firearms.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Food.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Food.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Football.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Football.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Friends.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Friends.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Fringe.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Fringe.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Frozen.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Frozen.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/FullmetalAlchemist.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/FullmetalAlchemist.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Futurama.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Futurama.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/GBF.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/GBF.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/GGundam.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/GGundam.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/GOSICK.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/GOSICK.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/GZFC.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/GZFC.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Games-zh.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Games-zh.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Games.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Games.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/GaoGaiGar.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/GaoGaiGar.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Geography.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Geography.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Getter Robo.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Getter Robo.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Ghibli.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Ghibli.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Glee.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Glee.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/GossipGirl.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/GossipGirl.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Guardians of Ga'Hoole.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Guardians of Ga'Hoole.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Gundam00.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Gundam00.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/GundamAGE.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/GundamAGE.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/GundamIBO.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/GundamIBO.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/GundamSeed.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/GundamSeed.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/GundamTWFM.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/GundamTWFM.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/GundamUC.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/GundamUC.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/GundamW.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/GundamW.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/HTGAWM.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/HTGAWM.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/HUNTER.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/HUNTER.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Half-Life.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Half-Life.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Hannibal Lecter.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Hannibal Lecter.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/HarryPotter.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/HarryPotter.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Hawaii Five-0.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Hawaii Five-0.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Hayate the Combat Butler.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Hayate the Combat Butler.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Heroes of the Storm.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Heroes of the Storm.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/House.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/House.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/IMF.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/IMF.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/IT.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/IT.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/JLeague.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/JLeague.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/JP Show.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/JP Show.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/James Bond.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/James Bond.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Jewelpet.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Jewelpet.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Justin Bieber.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Justin Bieber.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/KLeague.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/KLeague.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/KO Movie.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/KO Movie.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/KO Show.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/KO Show.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/KO TV Show.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/KO TV Show.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/KamenRider.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/KamenRider.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Kao.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Kao.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Katy Perry.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Katy Perry.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Korea Comparison.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Korea Comparison.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Korea.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Korea.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Korean.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Korean.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/LEGO.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/LEGO.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/LOL.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/LOL.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/LR.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/LR.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/La casa de papel.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/La casa de papel.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Lady Gaga.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Lady Gaga.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Lana Del Rey.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Lana Del Rey.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Laos.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Laos.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Legend of the Guardians.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Legend of the Guardians.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Les Misérables.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Les Misérables.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Lifesciences.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Lifesciences.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Linkin.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Linkin.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Lorde.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Lorde.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/LuaIT.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/LuaIT.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/LuaMovie.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/LuaMovie.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/LuaShow.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/LuaShow.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/MA.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/MA.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/MCD.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/MCD.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/MCFC.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/MCFC.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/MLS.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/MLS.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/MUFC.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/MUFC.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/MY.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/MY.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Mabinogi.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Mabinogi.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/MapleStory.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/MapleStory.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Mariah Carey.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Mariah Carey.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Math.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Math.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Mazinger.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Mazinger.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/McDonald's.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/McDonald's.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/MediaWiki special.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/MediaWiki special.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/MediaWiki.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/MediaWiki.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Medicine.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Medicine.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Michael Jackson.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Michael Jackson.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Might&Magic.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Might&Magic.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Military.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Military.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Minecraft.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Minecraft.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Movie.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Movie.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Music.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Music.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/My Little Pony.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/My Little Pony.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/MyHeroAcademia.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/MyHeroAcademia.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/NARUTO.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/NARUTO.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/NBA.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/NBA.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/NFL.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/NFL.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/NHL.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/NHL.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Nintendo.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Nintendo.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Nobel Prize.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Nobel Prize.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/OnePiece.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/OnePiece.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Organization.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Organization.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Overwatch.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Overwatch.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/P&G.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/P&G.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/PHL Places.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/PHL Places.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/People.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/People.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/PeppaPig.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/PeppaPig.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Percy Jackson.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Percy Jackson.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/PerryClass.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/PerryClass.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Pesticide.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Pesticide.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Photography.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Photography.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Physics.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Physics.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Pichi Pichi Pitch.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Pichi Pichi Pitch.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Pinnacle Islands.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Pinnacle Islands.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Pixar.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Pixar.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Pokemon-old.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Pokemon-old.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Pokemon.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Pokemon.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/PoliticiansUK.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/PoliticiansUK.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Popes.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Popes.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Power Rangers.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Power Rangers.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/PresidentsUS.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/PresidentsUS.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Pretty Rhythm.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Pretty Rhythm.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/PrisonBreak.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/PrisonBreak.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Psychology.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Psychology.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Racing.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Racing.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Railway.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Railway.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/RainbowSixSiege.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/RainbowSixSiege.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Reborn.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Reborn.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/ResidentEvil.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/ResidentEvil.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Rihanna.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Rihanna.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/SAO.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/SAO.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/SARS-CoV-2 variant.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/SARS-CoV-2 variant.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/SEGA.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/SEGA.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/SNSD.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/SNSD.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/SPL.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/SPL.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/SPY×FAMILY.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/SPY×FAMILY.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Sailor Moon.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Sailor Moon.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/SaintSeiyaOmega.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/SaintSeiyaOmega.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Sandbox.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Sandbox.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Selena Gomez.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Selena Gomez.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Shinkalion.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Shinkalion.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Shipname.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Shipname.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Show.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Show.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Shugo Chara!.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Shugo Chara!.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Sia.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Sia.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Signals and Systems.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Signals and Systems.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Sim.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Sim.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Simpsons.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Simpsons.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Snooker.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Snooker.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/SouthPark.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/SouthPark.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/SpongeBob SquarePants.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/SpongeBob SquarePants.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Sports.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Sports.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Square Enix.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Square Enix.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/StarCraft.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/StarCraft.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/StarCraft2.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/StarCraft2.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/StarTrek.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/StarTrek.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/StarWars.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/StarWars.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/StephenKing.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/StephenKing.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Summon Night.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Summon Night.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/TCM.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/TCM.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/TV.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/TV.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Table Tennis.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Table Tennis.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Tales.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Tales.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Tamagotchi.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Tamagotchi.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Taylor Swift.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Taylor Swift.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Telcom.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Telcom.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Tennis.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Tennis.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/The Chainsmokers.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/The Chainsmokers.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/The Witcher.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/The Witcher.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/The World God Only Knows.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/The World God Only Knows.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/TheBeatles.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/TheBeatles.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/ThePeanuts.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/ThePeanuts.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Toaru.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Toaru.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Transformers.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Transformers.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Transport for London.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Transport for London.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Transport.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Transport.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/TropicalCycloneName.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/TropicalCycloneName.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Twilight.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Twilight.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/TyphoonNew.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/TyphoonNew.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/TyphoonOld.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/TyphoonOld.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/UA toponyms.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/UA toponyms.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/UK Places.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/UK Places.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/US CA Cities.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/US CA Cities.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/US Government.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/US Government.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/US Senators.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/US Senators.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/USState.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/USState.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Ultraman.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Ultraman.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Unilever.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Unilever.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Unit.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Unit.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Urban.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Urban.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/VLeague.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/VLeague.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Valkyria.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Valkyria.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/WORKING!!.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/WORKING!!.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Warcraft.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Warcraft.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Warhammer.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Warhammer.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Warriors.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Warriors.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Watch.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Watch.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Weather.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Weather.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Windows.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Windows.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Wow.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Wow.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/Yes! 光之美少女5.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Yes! 光之美少女5.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/ZH Show.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/ZH Show.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/arsenal.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/arsenal.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/check1.py` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/check1.py`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/chelsea.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/chelsea.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/fcbarcelona.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/fcbarcelona.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/fcbayern.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/fcbayern.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/free license.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/free license.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/inter.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/inter.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/laliga.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/laliga.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/leek.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/leek.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/ligue.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/ligue.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/liverpoolfc.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/liverpoolfc.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/loghorizon.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/loghorizon.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/magi.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/magi.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/merge_for_web.py` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/merge_for_web.py`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/neo-noir.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/neo-noir.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/regalia.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/regalia.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/specialpages.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/specialpages.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/uefa.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/uefa.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/vital.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/vital.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/一拳超人.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/一拳超人.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/伊拉克足球.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/伊拉克足球.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/伊斯蘭.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/伊斯蘭.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/伊朗足球.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/伊朗足球.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/佛教.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/佛教.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/俄超.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/俄超.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/俱乐部足球联赛.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/俱乐部足球联赛.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/列斯聯.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/列斯聯.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/加超聯.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/加超聯.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/南美球會.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/南美球會.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/博弈论.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/博弈论.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/卡塔尔星级足球联赛.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/卡塔尔星级足球联赛.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/叙利亚职业足球联赛.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/叙利亚职业足球联赛.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/名偵探柯南.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/名偵探柯南.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/咕嚕咕嚕魔法陣.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/咕嚕咕嚕魔法陣.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/咲-Saki-.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/咲-Saki-.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/四驅兄弟.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/四驅兄弟.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/圍棋.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/圍棋.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/地名.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/地名.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/声临其境.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/声临其境.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/妖怪手錶.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/妖怪手錶.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/姓氏.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/姓氏.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/娛樂.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/娛樂.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/小魔女DoReMi.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/小魔女DoReMi.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/巴勒斯坦职业足球联赛.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/巴勒斯坦职业足球联赛.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/巴林职业足球联赛.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/巴林职业足球联赛.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/幸福爆發！光之美少女.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/幸福爆發！光之美少女.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/意甲.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/意甲.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/愛天使傳說.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/愛天使傳說.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/戰鬥陀螺 鋼鐵奇兵.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/戰鬥陀螺 鋼鐵奇兵.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/打工吧！魔王大人.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/打工吧！魔王大人.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/政治人物.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/政治人物.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/文學.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/文學.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/星光樂園.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/星光樂園.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/暗影诗章 (动画).json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/暗影诗章 (动画).json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/村上春樹.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/村上春樹.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/核能.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/核能.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/機獸系列.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/機獸系列.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/民族.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/民族.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/沙特职业足球联赛.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/沙特职业足球联赛.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/泰國人名.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/泰國人名.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/涼宮春日的憂鬱.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/涼宮春日的憂鬱.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/潘朵拉之心.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/潘朵拉之心.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/烏茲別克足球會.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/烏茲別克足球會.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/爆丸.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/爆丸.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/畜牧.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/畜牧.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/百變小櫻.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/百變小櫻.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/科威特职业足球联赛.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/科威特职业足球联赛.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/童話槍手小紅帽.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/童話槍手小紅帽.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/约旦职业足球联赛.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/约旦职业足球联赛.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/美国漫画.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/美国漫画.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/荷蘭足球聯賽.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/荷蘭足球聯賽.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/菁英殺機.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/菁英殺機.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/葡超.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/葡超.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/蠟筆小新.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/蠟筆小新.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/通靈王.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/通靈王.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/進擊的巨人.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/進擊的巨人.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/釣魚臺列嶼.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/釣魚臺列嶼.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/閃電十一人.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/閃電十一人.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/闇.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/闇.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/阿曼职业足球联赛.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/阿曼职业足球联赛.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/阿联酋职业足球联赛.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/阿联酋职业足球联赛.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/降世神通.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/降世神通.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/音樂劇.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/音樂劇.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/驅魔少年.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/驅魔少年.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/马来人名地名.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/马来人名地名.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/鬥陣特攻.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/鬥陣特攻.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/魔法咪路咪路.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/魔法咪路咪路.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/黎巴嫩职业足球联赛.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/黎巴嫩职业足球联赛.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/黑執事.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/黑執事.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/cgroups/黑塔系列.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/黑塔系列.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/poetry.lock` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/poetry.lock`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/update_basic.py` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/update_basic.py`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/data/update_cgroups.py` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/update_cgroups.py`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/run-maturin-action.sh` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/run-maturin-action.sh`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/src/converter.rs` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/src/converter.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,122 +1,436 @@
-use std::collections::HashMap;
+use std::collections::{HashMap, HashSet};
+use std::fmt::Write;
 use std::iter::IntoIterator;
+
 use std::str::FromStr;
 
-use aho_corasick::{AhoCorasick, AhoCorasickBuilder, AhoCorasickKind, MatchKind};
-use once_cell::unsync::Lazy;
-use regex::Regex;
+use daachorse::{CharwiseDoubleArrayAhoCorasick, CharwiseDoubleArrayAhoCorasickBuilder, MatchKind};
 
+use crate::tables::Table;
 use crate::{
     pagerules::PageRules,
     rule::{Conv, ConvAction, ConvRule},
+    tables::expand_table,
+    utils::{regex, unwrap_or_return},
     variant::Variant,
 };
 
 // Ref: https://github.com/wikimedia/mediawiki/blob/7bf779524ab1fd8e1d74f79ea4840564d48eea4d/includes/language/LanguageConverter.php#L76
 const NESTED_RULE_MAX_DEPTH: usize = 10;
 
-/// A ZhConverter. See also [`ZhConverterBuilder`].
+/// A ZhConverter, built by [`ZhConverterBuilder`].
 pub struct ZhConverter {
     variant: Variant,
-    automaton: AhoCorasick,
-    mapping: HashMap<String, String>,
+    automaton: Option<CharwiseDoubleArrayAhoCorasick<u32>>,
+    target_words: Vec<String>,
 }
 
 impl ZhConverter {
     /// Create a new converter from a automaton and a mapping.
     ///
     /// It is provided for convenience and not expected to be called directly.
     /// [`ZhConverterBuilder`] would take care of these
     /// details.
-    pub fn new(automaton: AhoCorasick, mapping: HashMap<String, String>) -> ZhConverter {
+    pub fn new(
+        automaton: CharwiseDoubleArrayAhoCorasick<u32>,
+        target_words: Vec<String>,
+    ) -> ZhConverter {
         ZhConverter {
             variant: Variant::Zh,
-            automaton,
-            mapping,
+            automaton: Some(automaton),
+            target_words,
+        }
+    }
+
+    /// Create a new converter from a automaton and a mapping, as well as specifying a target
+    /// variant to be used by [`convert_as_wikitext_basic`](Self::convert_as_wikitext_basic) and
+    /// [`convert_as_wikitext_extended`](Self::convert_as_wikitext_extended) and related functions.
+    ///
+    /// It is provided for convenience and not expected to be called directly.
+    /// [`ZhConverterBuilder`] would take care of these details.
+    pub fn with_target_variant(
+        automaton: CharwiseDoubleArrayAhoCorasick<u32>,
+        target_words: Vec<String>,
+        variant: Variant,
+    ) -> ZhConverter {
+        ZhConverter {
+            variant,
+            automaton: Some(automaton),
+            target_words,
         }
     }
 
     /// Create a new converter of a sequence of `(from, to)` pairs.
     ///
     /// It use [`ZhConverterBuilder`] internally.
     #[inline(always)]
-    pub fn from_pairs(pairs: &[(impl AsRef<str>, impl AsRef<str>)]) -> ZhConverter {
-        let mut builder = ZhConverterBuilder::new();
-        for (from, to) in pairs {
-            builder = builder.add_conv_pair(from, to);
-        }
-        builder.build()
+    pub fn from_pairs(
+        pairs: impl IntoIterator<Item = (impl Into<String>, impl Into<String>)>,
+    ) -> ZhConverter {
+        ZhConverterBuilder::new().conv_pairs(pairs).build()
+    }
+
+    /// Create a new converter of a sequence of `(from, to)` pairs.
+    ///
+    /// It takes a target variant to be used by [`convert_as_wikitext_basic`](Self::convert_as_wikitext_basic)
+    /// and [`convert_as_wikitext_extended`](Self::convert_as_wikitext_extended) and related
+    /// functions, in addition to [`from_pairs`](Self::from_pairs).
+    ///
+    /// It use [`ZhConverterBuilder`] internally.
+    #[inline(always)]
+    pub fn from_pairs_with_target_variant(
+        variant: Variant,
+        pairs: impl IntoIterator<Item = (impl Into<String>, impl Into<String>)>,
+    ) -> ZhConverter {
+        ZhConverterBuilder::new()
+            .target(variant)
+            .conv_pairs(pairs)
+            .build()
     }
 
     /// Convert a text.
+    #[inline(always)]
     pub fn convert(&self, text: &str) -> String {
         let mut output = String::with_capacity(text.len());
-        self.converted(text, &mut output);
+        self.convert_to(text, &mut output);
         output
     }
 
     /// Same as `convert`, except that it takes a `&mut String` as dest instead of returning a `String`.
-    pub fn converted(&self, text: &str, output: &mut String) {
+    pub fn convert_to(&self, text: &str, output: &mut String) {
+        let automaton = unwrap_or_return!(self.automaton.as_ref().or_else(|| {
+            output.push_str(text);
+            None
+        }));
+
         // Ref: https://github.dev/rust-lang/regex/blob/5197f21287344d2994f9cf06758a3ea30f5a26c3/src/re_trait.rs#L192
         let mut last = 0;
         // let mut cnt = HashMap::<usize, usize>::new();
         // leftmost-longest matching
-        for (s, e) in self.automaton.find_iter(text).map(|m| (m.start(), m.end())) {
+        for (s, e, ti) in automaton
+            .leftmost_find_iter(text)
+            .map(|m| (m.start(), m.end(), m.value()))
+        {
             if s > last {
                 output.push_str(&text[last..s]);
             }
             // *cnt.entry(text[s..e].chars().count()).or_insert(0) += 1;
-            output.push_str(self.mapping.get(&text[s..e]).unwrap());
+            output.push_str(&self.target_words[ti as usize]);
             last = e;
         }
         output.push_str(&text[last..]);
     }
 
-    /// Convert a text with inline conv rules applied.
+    /// Convert a text, a long with a secondary converter.
     ///
-    /// It only processes the display output of inline rules. Mutations to global rules specified
-    /// via inline rules are just ignored. To activate global rules, build a [`ZhConverterBuilder`]
-    /// with [`PageRules`](crate::pagerules::PageRules).
+    /// Conversion rules in the secondary converter shadow these existing ones in the original
+    /// converter.
+    /// For example, if the original converter contains a rule `香菜 -> 芫荽`, and the the secondary
+    /// converter contains a rule `香菜 -> 鹽須`, the latter would take effect and `香菜` is converted
+    /// to `鹽須`.
+    ///
+    /// The implementation match the text against the two converter alternatively, resulting in
+    /// degraded performance. It would be better to build a new converter that combines the
+    /// rulesets of both the two, especially when the secondary rulsets are non-trivial or the
+    /// input text is large.
+    ///
+    /// The worst-case time complexity of the implementation is `O(n*m)` where `n` and `m` are the
+    /// length of the text and the maximum lengths of sources words in conversion rulesets (i.e.
+    /// brute-force).
+    #[inline(always)]
+    pub fn convert_with_secondary_converter(
+        &self,
+        text: &str,
+        secondary_converter: &ZhConverter,
+    ) -> String {
+        let mut output = String::with_capacity(text.len());
+        self.convert_to_with_secondary_converter(text, &mut output, secondary_converter);
+        output
+    }
+
+    /// Same as [`convert_to_with_secondary_converter`](Self::convert_to_with_secondary_converter), except
+    /// that it takes a `&mut String` as dest instead of returning a `String`.
+    pub fn convert_to_with_secondary_converter(
+        &self,
+        text: &str,
+        output: &mut String,
+        secondary_converter: &ZhConverter,
+    ) {
+        let ZhConverter {
+            automaton: shadowing_automaton,
+            target_words: shadowing_target_words,
+            ..
+        } = secondary_converter;
+        match shadowing_automaton {
+            Some(shadowing_automaton) => self.convert_to_with(
+                text,
+                output,
+                Some(shadowing_automaton),
+                shadowing_target_words.as_slice(),
+                &Default::default(),
+            ),
+            None => self.convert_to(text, output),
+        }
+    }
+
+    /// Convert a text, a long with a secondary conversion table (typically temporary).
+    ///
+    /// The worst-case time complexity of the implementation is `O(n*m)` where `n` and `m` are the
+    /// length of the text and the maximum lengths of sources words in conversion rulesets.
+    /// (i.e. brute-force).
+    fn convert_to_with(
+        &self,
+        text: &str,
+        output: &mut String,
+        shadowing_automaton: Option<&CharwiseDoubleArrayAhoCorasick<u32>>,
+        shadowing_target_words: &[String],
+        shadowed_source_words: &HashSet<String>,
+    ) {
+        let automaton = unwrap_or_return!(self.automaton.as_ref().or_else(|| {
+            output.push_str(text);
+            None
+        }));
+
+        // let mut cnt = HashMap::<usize, usize>::new();
+        let mut last = 0;
+        let mut left_match: Option<(usize, usize, &str)> = None;
+        let mut right_match: Option<(usize, usize, &str)> = None;
+
+        while last < text.len() {
+            // leftmost-longest matching
+            if left_match.is_none() || left_match.unwrap().0 < last {
+                let m = automaton.leftmost_find_iter(&text[last..]).next();
+                left_match = m.map(|m| {
+                    (
+                        last + m.start(),
+                        last + m.end(),
+                        self.target_words[m.value() as usize].as_str(),
+                    )
+                });
+            }
+            if right_match.is_none() || right_match.unwrap().0 < last {
+                right_match = shadowing_automaton.and_then(|shadowing_automaton| {
+                    shadowing_automaton
+                        .leftmost_find_iter(&text[last..])
+                        .next()
+                        .map(|m| {
+                            (
+                                last + m.start(),
+                                last + m.end(),
+                                shadowing_target_words[m.value() as usize].as_str(),
+                            )
+                        })
+                });
+            }
+
+            let (s, e, target_word) = match (left_match, right_match) {
+                (Some(a), Some(b)) if a.0 > b.0 || (a.0 == b.0 && a.1 <= b.1) => b, // shadowed: pick a word in shadowing automaton
+                (None, Some(b)) => b,                                               // ditto
+                (Some(a), _) => {
+                    // not shadowed: pick a word in original automaton
+                    if shadowed_source_words.contains(a.2) {
+                        // source word is disabled: skip one char and re-search
+                        let first_char_len = text.chars().next().unwrap().len_utf8();
+                        (
+                            last,
+                            a.0 + first_char_len,
+                            &text[last..a.0 + first_char_len],
+                        )
+                    } else {
+                        a
+                    }
+                }
+                (None, None) => {
+                    // end
+                    output.push_str(&text[last..]);
+                    break;
+                }
+            };
+            if s > last {
+                output.push_str(&text[last..s]);
+            }
+            // *cnt.entry(text[s..e].chars().count()).or_insert(0) += 1;
+            output.push_str(target_word);
+            last = e;
+        }
+    }
+
+    /// Convert the given text, parsing and applying adhoc Mediawiki conversion rules in it.
+    ///
+    /// Basic MediaWiki conversion rules like `-{FOOBAR}-` or `-{zh-hant:FOO;zh-hans:BAR}-` are
+    /// supported.
+    ///
+    /// Unlike [`convert_to_as_wikitext_extended`](Self::convert_to_as_wikitext_extended), rules
+    /// with additional flags like `{H|zh-hant:FOO;zh-hans:BAR}` that sets global rules are simply
+    /// ignored. And, it does not try to skip HTML code blocks like `<code></code>` and
+    /// `<script></script>`.
+    #[inline(always)]
+    pub fn convert_as_wikitext_basic(&self, text: &str) -> String {
+        let mut output = String::with_capacity(text.len());
+        self.convert_to_as_wikitext_basic(text, &mut output);
+        output
+    }
+
+    /// Convert the given text, parsing and applying adhoc and global MediaWiki conversion rules in
+    /// it.
+    ///
+    /// Unlike [`convert_to_as_wikitext_basic`](Self::convert_to_as_wikitext_basic), all flags
+    /// documented in [Help:高级字词转换语法](https://zh.wikipedia.org/wiki/Help:高级字词转换语法)
+    /// are supported. And it tries to skip HTML code blocks such as `<code></code>` and
+    /// `<script></script>`.
+    ///
+    /// # Limitations
     ///
     /// The internal implementation are intendedly replicating the behavior of
     /// [LanguageConverter.php](https://github.com/wikimedia/mediawiki/blob/7bf779524ab1fd8e1d74f79ea4840564d48eea4d/includes/language/LanguageConverter.php#L855)
     /// in MediaWiki. But it is not fully compliant with MediaWiki and providing NO PROTECTION over
-    /// XSS attack.
+    /// XSS attacks.
     ///
-    /// Compared to the plain `convert`, this is known to be much slower due to the inevitable
+    /// Compared to the plain `convert`, this is known to be MUCH SLOWER due to the inevitable
     /// nature of the implementation decision made by MediaWiki.
-    pub fn convert_allowing_inline_rules(&self, text: &str) -> String {
+    #[inline(always)]
+    pub fn convert_as_wikitext_extended(&self, text: &str) -> String {
+        let mut output = String::with_capacity(text.len());
+        self.convert_to_as_wikitext_extended(text, &mut output);
+        output
+    }
+
+    /// Same as [`convert_to_as_wikitext_basic`](Self::convert_to_as_wikitext_basic), except that
+    /// it takes a `&mut String` as dest
+    /// instead of returning a `String`.
+    #[inline(always)]
+    pub fn convert_to_as_wikitext_basic(&self, text: &str, output: &mut String) {
+        self.convert_to_as_wikitext(text, output, &mut None, false, false)
+    }
+
+    /// Same as [`convert_to_as_wikitext_extended`](Self::convert_to_as_wikitext_extended), except
+    /// that it takes a `&mut String` as dest instead of returning a `String`.
+    #[inline(always)]
+    pub fn convert_to_as_wikitext_extended(&self, text: &str, output: &mut String) {
+        self.convert_to_as_wikitext(text, output, &mut None, true, true)
+    }
+
+    /// The general implementation of MediaWiki syntax-aware conversion.
+    ///
+    /// Equivalent to [`convert_as_wikitext_basic`](Self::convert_as_wikitext_basic) if
+    /// `addtional_conv_lines` is set empty and both `skip_html_code_blocks` and
+    /// `apply_global_rules` are set to `false`.
+    ///
+    /// Equivalent to [`convert_as_wikitext_extended`], otherwise.
+    ///
+    /// `addtional_conv_lines` looks like:
+    /// ```text
+    /// zh-cn:天堂执法者; zh-hk:夏威夷探案; zh-tw:檀島警騎2.0;
+    /// zh-cn:史蒂芬·'史蒂夫'·麦格瑞特; zh-tw:史提夫·麥加雷; zh-hk:麥星帆;
+    /// zh-cn:丹尼尔·'丹尼/丹诺'·威廉姆斯; zh-tw:丹尼·威廉斯; zh-hk:韋丹尼;
+    /// ```
+    #[inline(always)]
+    pub fn convert_as_wikitext(
+        &self,
+        text: &str,
+        secondary_converter_builder: &mut Option<ZhConverterBuilder>,
+        skip_html_code_blocks: bool,
+        apply_global_rules: bool,
+    ) -> String {
+        let mut output = String::with_capacity(text.len());
+        self.convert_to_as_wikitext(
+            text,
+            &mut output,
+            secondary_converter_builder,
+            skip_html_code_blocks,
+            apply_global_rules,
+        );
+        output
+    }
+
+    /// Same as [`convert_as_wikitext`](Self::convert_as_wikitext), except
+    /// that it takes a `&mut String` as dest instead of returning a `String`.
+    pub fn convert_to_as_wikitext(
+        &self,
+        text: &str,
+        output: &mut String,
+        secondary_converter_builder: &mut Option<ZhConverterBuilder>,
+        skip_html_code_blocks: bool,
+        apply_global_rules: bool,
+    ) {
         // Ref: https://github.com/wikimedia/mediawiki/blob/7bf779524ab1fd8e1d74f79ea4840564d48eea4d/includes/language/LanguageConverter.php#L855
         //  and https://github.com/wikimedia/mediawiki/blob/7bf779524ab1fd8e1d74f79ea4840564d48eea4d/includes/language/LanguageConverter.php#L910
         //  and https://github.com/wikimedia/mediawiki/blob/7bf779524ab1fd8e1d74f79ea4840564d48eea4d/includes/language/LanguageConverter.php#L532
-        // TODO: this may degrade to O(n^2)
-        let p1 = Lazy::new(|| {
-            // start of rule | noHtml | noStyle | no code | no pre
-            Regex::new(r#"-\{|<script.*?>.*?</script>|<style.*?>.*?</style>|<code>.*?</code>|<pre.*?>.*?</pre>"#).unwrap()
-        });
+
+        #[allow(clippy::type_complexity)]
+        let mut convert_to: Box<dyn Fn(&str, &mut String)> =
+            Box::new(|text: &str, output: &mut String| self.convert_to(text, output));
+        if secondary_converter_builder.is_some() || apply_global_rules {
+            // build a secondary automaton from global rules specified in wikitext
+            let mut builder = secondary_converter_builder.take().unwrap_or_default();
+            if !builder.tables.is_empty() {
+                panic!("The secondary converter builder should not load conversion tables");
+            }
+            // let mut shadowing_pairs = HashMap::new();
+            let global_rules_in_page = PageRules::from_str(text).expect("infaillible");
+            for ca in global_rules_in_page.as_conv_actions() {
+                match ca.is_add() {
+                    true => builder = builder.conv_pairs(ca.as_conv().get_conv_pairs(self.variant)),
+                    false => {
+                        builder = builder.unconv_pairs(ca.as_conv().get_conv_pairs(self.variant))
+                    }
+                }
+            }
+            let ZhConverter {
+                automaton: shadowing_automaton,
+                target_words: shadowing_target_words,
+                ..
+            } = builder.build();
+            let shadowed_source_words: HashSet<String> = builder.removes.keys().cloned().collect();
+            *secondary_converter_builder = Some(builder);
+            if shadowing_automaton.is_some() || !shadowed_source_words.is_empty() {
+                convert_to = Box::new(move |text: &str, output: &mut String| {
+                    self.convert_to_with(
+                        text,
+                        output,
+                        shadowing_automaton.as_ref(),
+                        shadowing_target_words.as_slice(),
+                        &shadowed_source_words,
+                    )
+                })
+            }
+        };
+
+        // TODO: is this O(n) instead of O(n^2)?
+        // start of rule | noHtml | noStyle | no code | no pre
+        let sor_or_html = regex!(
+            r#"-\{|<script.*?>.*?</script>|<style.*?>.*?</style>|<code>.*?</code>|<pre.*?>.*?</pre>"#
+        );
+        // start of rule
+        let sor = regex!(r#"-\{"#);
+        let pat_outer = if skip_html_code_blocks {
+            sor_or_html
+        } else {
+            sor
+        };
         // TODO: we need to understand what the hell it is so that to adapt it to compatible syntax
         // 		$noHtml = '<(?:[^>=]*+(?>[^>=]*+=\s*+(?:"[^"]*"|\'[^\']*\'|[^\'">\s]*+))*+[^>=]*+>|.*+)(*SKIP)(*FAIL)';
-        let p2 = Lazy::new(|| Regex::new(r#"-\{|\}-"#).unwrap());
+        let pat_inner = regex!(r#"-\{|\}-"#);
+
         let mut pos = 0;
-        let mut converted = String::with_capacity(text.len());
         let mut pieces = vec![];
-        while let Some(m1) = p1.find_at(text, pos) {
+        while let Some(m1) = pat_outer.find_at(text, pos) {
             // convert anything before (possible) the toplevel -{
-            self.converted(&text[pos..m1.start()], &mut converted);
+            convert_to(&text[pos..m1.start()], output);
             if m1.as_str() != "-{" {
                 // not start of rule, just <foobar></foobar> to exclude
-                converted.push_str(&text[m1.start()..m1.end()]); // kept as-is
+                output.push_str(&text[m1.start()..m1.end()]); // kept as-is
                 pos = m1.end();
                 continue; // i.e. <SKIP><FAIL>
             }
             // found toplevel -{
             pos = m1.start() + 2;
             pieces.push(String::new());
-            while let Some(m2) = p2.find_at(text, pos) {
+            while let Some(m2) = pat_inner.find_at(text, pos) {
                 // let mut piece = String::from(&text[pos..m2.start()]);
                 if m2.as_str() == "-{" {
                     // if there are two many open start tag, ignore the new nested rule
                     if pieces.len() >= NESTED_RULE_MAX_DEPTH {
                         pos += 2;
                         continue;
                     }
@@ -124,23 +438,21 @@
                     pieces.last_mut().unwrap().push_str(&text[pos..m2.start()]);
                     pieces.push(String::new()); // e.g. -{ zh: AAA -{
                     pos = m2.end();
                 } else {
                     // end tag
                     let mut piece = pieces.pop().unwrap();
                     piece.push_str(&text[pos..m2.start()]);
-                    let upper = if let Some(upper) = pieces.last_mut() {
-                        upper
+                    // only take it output; mutations to global rules are ignored
+                    let r = ConvRule::from_str_infallible(&piece);
+                    if let Some(upper) = pieces.last_mut() {
+                        write!(upper, "{}", r.targeted(self.variant)).unwrap();
                     } else {
-                        &mut converted
+                        write!(output, "{}", r.targeted(self.variant)).unwrap();
                     };
-                    // only take it output; mutations to global rules are ignored
-                    ConvRule::from_str_infallible(&piece)
-                        .write_output(upper, self.variant)
-                        .unwrap();
                     // if let Ok(rule) = dbg!(ConvRule::from_str(&piece)) {
                     //     rule.write_output(upper, self.variant).unwrap();
                     // } else {
                     //     // rule is invalid
                     //     // TODO: what should we do actually? for now, we just do nothing to it
                     //     upper.push_str(&piece);
                     // }
@@ -148,24 +460,23 @@
                     if pieces.is_empty() {
                         // return to toplevel
                         break;
                     }
                 }
             }
             while let Some(piece) = pieces.pop() {
-                converted.push_str("-{");
-                converted.push_str(&piece);
+                output.push_str("-{");
+                output.push_str(&piece);
             }
             // TODO: produce convert(&text[pos..])
         }
         if pos < text.len() {
             // no more conv rules, just convert and append
-            converted.push_str(&self.convert(&text[pos..]));
+            convert_to(&text[pos..], output);
         }
-        converted
     }
 
     // TODO: inplace? we need to maintain a stack which could be at most O(n)
     //       and it requires access to underlying bytes for subtle mutations
     // pub fn convert_inplace(&self, text: &mut String) {
     //     let tbp = VecDeque::<&str>::new(); // to be pushed
     //     let mut wi = 0; // writing index
@@ -174,70 +485,91 @@
     //         while !tbp.is_empty() && s - wi >= tbp[0].len() {
     //             let raw = unsafe { text.as_bytes_mut() };
     //             raw[wi..wi + tbp[0].len()].clone_from_slice(tbp[0].as_bytes());
     //             tbp.pop_front();
     //         }
     //     }
     // }
+
+    /// Count the sum of lengths of matched source words to be substituted in the given text, in bytes.
+    pub fn count_matched(&self, text: &str) -> usize {
+        let automaton = unwrap_or_return!(self.automaton.as_ref(), 0);
+
+        automaton
+            .leftmost_find_iter(text)
+            .map(|m| m.end() - m.start())
+            .sum()
+    }
 }
 
-/// A builder that helps build a `ZhConverter`.
+/// A builder that helps build a [`ZhConverter`](ZhConverter).
 ///
 /// # Example
 /// Build a Zh2CN converter with some additional rules.
 /// ```
-/// use zhconv::{zhconv, ZhConverterBuilder, Variant, tables::ZH_HANS_CN_TABLE};
+/// use zhconv::{zhconv, ZhConverterBuilder, Variant, get_builtin_tables};
 /// // extracted from https://zh.wikipedia.org/wiki/Template:CGroup/Template:CGroup/文學.
-/// let conv_lines = r"zh-hans:三个火枪手;zh-hant:三劍客;zh-tw:三劍客;
+/// let rules = r"zh-hans:三个火枪手;zh-hant:三劍客;zh-tw:三劍客;
 ///                    zh-cn:雾都孤儿;zh-tw:孤雛淚;zh-hk:苦海孤雛;zh-sg:雾都孤儿;zh-mo:苦海孤雛;";
 /// let converter = ZhConverterBuilder::new()
 ///                     .target(Variant::ZhCN)
-///                     .table(*ZH_HANS_CN_TABLE)
-///                     .dfa(true) // dfa enabled: slower build, faster conversion
-///                     .conv_lines(conv_lines)
+///                     .tables(get_builtin_tables(Variant::ZhCN))
+///                     .conv_lines(rules.lines())
 ///                     .build();
 /// let original = "《三劍客》是亞歷山大·仲馬的作品。《孤雛淚》是查爾斯·狄更斯的作品。";
 /// assert_eq!(converter.convert(original), "《三个火枪手》是亚历山大·仲马的作品。《雾都孤儿》是查尔斯·狄更斯的作品。");
 /// assert_eq!(zhconv(original, Variant::ZhCN), "《三剑客》是亚历山大·仲马的作品。《孤雏泪》是查尔斯·狄更斯的作品。")
 #[derive(Debug, Clone, Default)]
 pub struct ZhConverterBuilder<'t> {
     target: Variant,
     /// The base conversion table
     tables: Vec<(&'t str, &'t str)>,
     /// Rules to be added, from page rules or cgroups
     adds: HashMap<String, String>,
     /// Rules to be removed, from page rules or cgroups
     removes: HashMap<String, String>, // TODO: unnecessary owned type
-    dfa: bool,
 }
 
 impl<'t> ZhConverterBuilder<'t> {
     pub fn new() -> Self {
         Default::default()
     }
 
+    /// Shorthand for `ZhConverterBuilder::new()::target(variant)`.
+    #[inline(always)]
+    pub fn targeted(variant: Variant) -> Self {
+        Self::new().target(variant)
+    }
+
     /// Set the target Chinese variant to convert to.
     ///
     /// The target variant is only useful to get proper conv pairs from
     /// [`ConvRule`](crate::rule::ConvRule)s. That is, if only tables are specified, the target
     /// variant would be useless.
     pub fn target(mut self, variant: Variant) -> Self {
         self.target = variant;
         self
     }
 
     /// Add a conversion table, which is typically those in [`tables`](crate::tables).
-    pub fn table(mut self, table: (&'t str, &'t str)) -> Self {
+    pub fn table(mut self, table: Table<'t>) -> Self {
         self.tables.push(table);
         self
     }
 
-    //  [CGroup](https://zh.wikipedia.org/wiki/Module:CGroup) (a.k.a 公共轉換組)
+    /// Add a set of conversion tables, which are typically returned by [`get_builtin_tables`](crate::get_builtin_tables).
+    pub fn tables(mut self, tables: &[Table<'t>]) -> Self {
+        self.tables.extend(tables.iter());
+        self
+    }
+
+    // /// [CGroup](https://zh.wikipedia.org/wiki/Module:CGroup) (a.k.a 公共轉換組)
+    // pub fn cgroup()
 
-    /// Add a set of rules extracted from a page.
+    /// Add a set of rules extracted from a page in wikitext.
     ///
     /// This is a helper wrapper around `page_rules`.
     #[inline(always)]
     pub fn rules_from_page(self, text: &str) -> Self {
         self.page_rules(
             &PageRules::from_str(text).expect("Page rules parsing is infallible for now"),
         )
@@ -251,140 +583,177 @@
 
     /// Add a set of rules.
     ///
     /// These rules take the higher precedence over those specified via `table`.
     fn conv_actions<'i>(mut self, conv_actions: impl IntoIterator<Item = &'i ConvAction>) -> Self {
         for conv_action in conv_actions {
             let pairs = conv_action.as_conv().get_conv_pairs(self.target);
-            if conv_action.adds() {
+            if conv_action.is_add() {
                 self.adds
-                    .extend(pairs.iter().map(|&(f, t)| (f.to_owned(), t.to_owned())));
+                    .extend(pairs.map(|(f, t)| (f.to_owned(), t.to_owned())));
             } else {
                 self.removes
-                    .extend(pairs.iter().map(|&(f, t)| (f.to_owned(), t.to_owned())));
+                    .extend(pairs.map(|(f, t)| (f.to_owned(), t.to_owned())));
             }
         }
         self
     }
 
-    /// Add a [`Conv`].
+    /// Add [`Conv`]s.
     ///
     /// For general cases, check [`add_conv_pair`](#method.add_conv_pair) which takes a plain
     /// `from -> to` pair.
-    pub fn add_conv(mut self, conv: Conv) -> Self {
-        let pairs = conv.get_conv_pairs(self.target);
-        self.adds
-            .extend(pairs.iter().map(|&(f, t)| (f.to_owned(), t.to_owned())));
+    pub fn convs(mut self, convs: impl IntoIterator<Item = impl AsRef<Conv>>) -> Self {
+        for conv in convs.into_iter() {
+            self.adds.extend(
+                conv.as_ref()
+                    .get_conv_pairs(self.target)
+                    .map(|(f, t)| (f.to_owned(), t.to_owned())),
+            )
+        }
         self
     }
 
     /// Mark a conv as removed.
-    pub fn remove_conv(mut self, conv: Conv) -> Self {
-        let pairs = conv.get_conv_pairs(self.target);
-        self.removes
-            .extend(pairs.iter().map(|&(f, t)| (f.to_owned(), t.to_owned())));
+    pub fn unconvs(mut self, convs: impl IntoIterator<Item = impl AsRef<Conv>>) -> Self {
+        for conv in convs.into_iter() {
+            self.removes.extend(
+                conv.as_ref()
+                    .get_conv_pairs(self.target)
+                    .map(|(f, t)| (f.to_owned(), t.to_owned())),
+            )
+        }
         self
     }
 
-    /// Add a single `from -> to` conversion pair.
+    /// Add `from -> to` conversion pairs.
     ///
     /// It takes the precedence over those specified via `table`. It shares the same precedence level with those specified via `cgroup`.
-    pub fn add_conv_pair(mut self, from: impl AsRef<str>, to: impl AsRef<str>) -> Self {
-        let (from, to): (&str, &str) = (from.as_ref(), to.as_ref());
-        if from.is_empty() {
-            panic!("Conv pair should have non-empty from.")
+    pub fn conv_pairs(
+        mut self,
+        pairs: impl IntoIterator<Item = (impl Into<String>, impl Into<String>)>,
+    ) -> Self {
+        for (from, to) in pairs {
+            let (from, to) = (from.into(), to.into());
+            debug_assert!(!from.is_empty(), "Conv pair should have non-empty from.");
+            if from.is_empty() {
+                continue;
+            }
+            self.adds.insert(from, to);
+        }
+        self
+    }
+
+    /// Mark conversion pairs as removed.
+    ///
+    /// Any rule with the same `from`, whether specified via `add_conv_pair`, `conv_lines` or `table`, is removed.
+    pub fn unconv_pairs(
+        mut self,
+        pairs: impl IntoIterator<Item = (impl Into<String>, impl Into<String>)>,
+    ) -> Self {
+        for (from, to) in pairs {
+            let (from, to) = (from.into(), to.into());
+            debug_assert!(!from.is_empty(), "Conv pair should have non-empty from.");
+            if from.is_empty() {
+                continue;
+            }
+            self.removes.insert(from, to);
         }
-        self.adds.insert(from.to_owned(), to.to_owned());
         self
     }
 
     /// Mark a single conversion pair as removed.
     ///
     /// Any rule with the same `from`, whether specified via `add_conv_pair`, `conv_lines` or `table`, is removed.
-    pub fn remove_conv_pair(mut self, from: impl AsRef<str>, to: impl AsRef<str>) -> Self {
+    pub fn unconv_pair(mut self, from: impl AsRef<str>, to: impl AsRef<str>) -> Self {
         self.removes
             .insert(from.as_ref().to_owned(), to.as_ref().to_owned());
         self
     }
 
     /// Add a text of conv lines.
     ///
     /// e.g.
     /// ```text
     /// zh-cn:天堂执法者; zh-hk:夏威夷探案; zh-tw:檀島警騎2.0;
     /// zh-cn:史蒂芬·'史蒂夫'·麦格瑞特; zh-tw:史提夫·麥加雷; zh-hk:麥星帆;
     /// zh-cn:丹尼尔·'丹尼/丹诺'·威廉姆斯; zh-tw:丹尼·威廉斯; zh-hk:韋丹尼;
-    /// ```
-    pub fn conv_lines(mut self, lines: &str) -> Self {
-        for line in lines.lines().map(str::trim).filter(|s| !s.is_empty()) {
-            if let Ok(conv) = Conv::from_str(line.trim()) {
+    /// ```  
+    pub fn conv_lines(mut self, lines: impl IntoIterator<Item = impl AsRef<str>>) -> Self {
+        for line in lines.into_iter() {
+            let line = line.as_ref().trim();
+            if line.is_empty() {
+                continue;
+            }
+            if let Ok(conv) = Conv::from_str(line) {
                 self.adds
-                    .extend(conv.get_conv_pairs(self.target).iter().map(|&(f, t)| {
+                    .extend(conv.get_conv_pairs(self.target).map(|(f, t)| {
                         if f.is_empty() {
                             panic!("Conv pair should have non-empty from.")
                         }
                         (f.to_owned(), t.to_owned())
                     }));
             }
         }
         self
     }
 
-    /// Set whether to activate the feature DFA of Aho-Corasick.
-    ///
-    /// With DFA enabled, it takes rougly 5x time to build the converter while the conversion
-    /// speed is < 2x faster. All built-in converters have this feature enabled for better
-    /// conversion performance. In other cases with this flag unset, the implementation would
-    /// determine by itself whether to enable it per the number of patterns.
-    pub fn dfa(mut self, enabled: bool) -> Self {
-        self.dfa = enabled;
-        self
-    }
-
     /// Do the build.
     ///
     /// It internally aggregate previously specified tables, rules and pairs, from where an
     /// automaton and a mapping are built, which are then feed into the new converter.
     pub fn build(&self) -> ZhConverter {
+        let mapping = self.build_mapping();
+        let mut target_words = vec![];
+        let automaton = if !mapping.is_empty() {
+            target_words.reserve_exact(mapping.len());
+            let sequence = mapping.into_iter();
+            Some(
+                CharwiseDoubleArrayAhoCorasickBuilder::new()
+                    .match_kind(MatchKind::LeftmostLongest)
+                    .build(sequence.map(|(f, t)| {
+                        target_words.push(t);
+                        f
+                    }))
+                    .expect("Rules feed to DAAC already filtered"),
+            )
+        } else {
+            None
+        };
+
+        ZhConverter {
+            variant: self.target,
+            automaton,
+            target_words,
+        }
+    }
+
+    /// Aggregate previously specified tables, rules and pairs to build a mapping.
+    ///
+    /// It is used by [`build`](Self::build) internally.
+    pub fn build_mapping(&self) -> HashMap<String, String> {
         let Self {
-            target,
             tables,
-            dfa,
             adds,
             removes,
+            ..
         } = self;
+        // TODO: do we need a HashMap at all?
         let mut mapping = HashMap::with_capacity(
             (tables.iter().map(|(fs, _ts)| fs.len()).sum::<usize>() + adds.len())
                 .saturating_sub(removes.len()),
         );
         mapping.extend(
             tables
                 .iter()
-                .flat_map(|(froms, tos)| {
-                    std::iter::zip(froms.trim().split('|'), tos.trim().split('|'))
-                })
-                .filter(|&(from, to)| !(from.is_empty() && to.is_empty())) // empty str will trouble AC
-                .filter(|&(from, _to)| !removes.contains_key(from))
-                .map(|(from, to)| (from.to_owned(), to.to_owned())),
+                .flat_map(|&table| expand_table(table))
+                .filter(|(from, to)| !(from.is_empty() && to.is_empty())) // empty str would trouble AC
+                .filter(|(from, _to)| !removes.contains_key(from)),
         );
         mapping.extend(
             adds.iter()
                 .filter(|(from, _to)| !removes.contains_key(from.as_str()))
                 .map(|(from, to)| (from.to_owned(), to.to_owned())),
         );
-        let sequence = mapping.keys();
-        let automaton = AhoCorasickBuilder::new()
-            .match_kind(MatchKind::LeftmostLongest)
-            .kind(if *dfa {
-                Some(AhoCorasickKind::DFA)
-            } else {
-                None
-            })
-            .build(sequence)
-            .unwrap();
-        ZhConverter {
-            variant: *target,
-            mapping,
-            automaton,
-        }
+        mapping
     }
 }
```

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/src/converters.rs` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/src/converters.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,47 @@
 //! Converters lazily built from built-in [`tables`](crate::tables).
 //!
 //! These converters are lazily built on demand with [`dfa`](crate::ZhConverterBuilder::dfa)
 //! activated for better conversion performance, and cached for later use.
 
+use daachorse::CharwiseDoubleArrayAhoCorasick;
 use lazy_static::lazy_static; // TODO: once_cell
 
-use crate::{tables::*, Variant, ZhConverter};
+use crate::{tables::*, utils::zstd_decompress, Variant, ZhConverter, ZhConverterBuilder};
 
+// FIX: Doc
+
+// More specific rules should take precedence when merging (e.g. zh-TW > zh-Hant).
+// Since the converter build process relies on HashMap::extend, latter rules overwrite the early ones.
 lazy_static! {
     #[allow(non_upper_case_globals)]
     /// Placeholding converter (`zh`/原文). Nothing will be converted with this.
-    pub static ref ZH_BLANK_CONVERTER: ZhConverter = build_converter(Variant::Zh, ("", ""));
+    pub static ref ZH_BLANK_CONVERTER: ZhConverter = ZhConverterBuilder::new().target(Variant::Zh).build();
     /// Zh2Hant converter (`zh-Hant`/繁體中文), lazily built from [`ZH_HANT_TABLE`](crate::ZH_HANT_TABLE).
-    pub static ref ZH_TO_HANT_CONVERTER: ZhConverter = build_converter(Variant::ZhHant, ZH_HANT_TABLE);
+    pub static ref ZH_TO_HANT_CONVERTER: ZhConverter = deserialize_converter(Variant::ZhHant, ZH_HANT_DAAC, [ZH_HANT_TABLE]);
     /// Zh2Hans converter (`zh-Hans`/简体中文), lazily built from [`ZH_HANS_TABLE`](crate::ZH_HANS_TABLE).
-    pub static ref ZH_TO_HANS_CONVERTER: ZhConverter = build_converter(Variant::ZhHans, ZH_HANS_TABLE);
-    /// Zh2TW converter (`zh-Hant-TW`/臺灣正體), lazily built from [`ZH_HANT_TW_TABLE`](crate::ZH_HANT_TW_TABLE).
-    pub static ref ZH_TO_TW_CONVERTER: ZhConverter = build_converter(Variant::ZhTW, *ZH_HANT_TW_TABLE);
-    /// Zh2HK converter (`zh-Hant-HK`/香港繁體), lazily built from [`ZH_HANT_HK_TABLE`](crate::ZH_HANT_HK_TABLE).
-    pub static ref ZH_TO_HK_CONVERTER: ZhConverter = build_converter(Variant::ZhHK, *ZH_HANT_HK_TABLE);
-    /// Zh2MO converter (`zh-Hant-MO`/澳門繁體), lazily built from [`ZH_HANT_MO_TABLE`](crate::ZH_HANT_MO_TABLE).
-    pub static ref ZH_TO_MO_CONVERTER: ZhConverter = build_converter(Variant::ZhMO, *ZH_HANT_MO_TABLE);
-    /// Zh2CN converter (`zh-Hans-CN`/大陆简体), lazily built from [`ZH_HANS_CN_TABLE`](crate::ZH_HANS_CN_TABLE).
-    pub static ref ZH_TO_CN_CONVERTER: ZhConverter = build_converter(Variant::ZhCN, *ZH_HANS_CN_TABLE);
-    /// Zh2SG converter (`zh-Hans-SG`/新加坡简体), lazily built from [`ZH_HANS_SG_TABLE`](crate::ZH_HANS_SG_TABLE).
-    pub static ref ZH_TO_SG_CONVERTER: ZhConverter = build_converter(Variant::ZhSG, *ZH_HANS_SG_TABLE);
-    /// Zh2MY converter (`zh-Hans-MY`/大马简体), lazily built from [`ZH_HANS_MY_TABLE`](crate::ZH_HANS_MY_TABLE).
-    pub static ref ZH_TO_MY_CONVERTER: ZhConverter = build_converter(Variant::ZhMY, *ZH_HANS_MY_TABLE);
+    pub static ref ZH_TO_HANS_CONVERTER: ZhConverter = deserialize_converter(Variant::ZhHans, ZH_HANS_DAAC, [ZH_HANS_TABLE]);
+    /// Zh2TW converter (`zh-Hant-TW`/臺灣正體), lazily built from [`ZH_HANT_TABLE`](crate::ZH_HANT_TABLE)
+    /// and [`ZH_TW_TABLE`](crate::ZH_TW_TABLE).
+    pub static ref ZH_TO_TW_CONVERTER: ZhConverter = deserialize_converter(Variant::ZhTW, ZH_HANT_TW_DAAC, [ZH_HANT_TABLE, ZH_TW_TABLE]);
+    /// Zh2HK converter (`zh-Hant-HK`/香港繁體), lazily built from [`ZH_HANT_TABLE`](crate::ZH_HANT_TABLE)
+    /// and [`ZH_HK_TABLE`](crate::ZH_HK_TABLE).
+    pub static ref ZH_TO_HK_CONVERTER: ZhConverter = deserialize_converter(Variant::ZhHK, ZH_HANT_HK_DAAC, [ZH_HANT_TABLE, ZH_HK_TABLE]);
+    /// Zh2MO converter (`zh-Hant-MO`/澳門繁體), lazily built from [`ZH_HANT_TABLE`](crate::ZH_HANT_TABLE)
+    /// and [`ZH_MO_TABLE`](crate::ZH_MO_TABLE).
+    pub static ref ZH_TO_MO_CONVERTER: ZhConverter = deserialize_converter(Variant::ZhMO, ZH_HANT_MO_DAAC, [ZH_HANT_TABLE, ZH_MO_TABLE]);
+    /// Zh2CN converter (`zh-Hans-CN`/大陆简体), lazily built from [`ZH_HANS_TABLE`](crate::ZH_HANS_TABLE)
+    /// and [`ZH_CN_TABLE`](crate::ZH_CN_TABLE).
+    pub static ref ZH_TO_CN_CONVERTER: ZhConverter = deserialize_converter(Variant::ZhCN, ZH_HANS_CN_DAAC, [ZH_HANS_TABLE, ZH_CN_TABLE]);
+    /// Zh2SG converter (`zh-Hans-SG`/新加坡简体), lazily built from [`ZH_HANS_TABLE`](crate::ZH_HANS_TABLE)
+    /// and [`ZH_SG_TABLE`](crate::ZH_SG_TABLE).
+    pub static ref ZH_TO_SG_CONVERTER: ZhConverter = deserialize_converter(Variant::ZhSG, ZH_HANS_SG_DAAC, [ZH_HANS_TABLE, ZH_SG_TABLE]);
+    /// Zh2MY converter (`zh-Hans-MY`/大马简体), lazily built from [`ZH_HANS_TABLE`](crate::ZH_HANS_TABLE)
+    /// and [`ZH_MY_TABLE`](crate::ZH_MY_TABLE).
+    pub static ref ZH_TO_MY_CONVERTER: ZhConverter = deserialize_converter(Variant::ZhMY, ZH_HANS_MY_DAAC, [ZH_HANS_TABLE, ZH_MY_TABLE]);
 }
 
 /// Get the builtin converter for a target Chinese variant.
 #[inline(always)]
 pub fn get_builtin_converter(target: Variant) -> &'static ZhConverter {
     use Variant::*;
     match target {
@@ -42,26 +53,25 @@
         ZhMO => &ZH_TO_MO_CONVERTER,
         ZhCN => &ZH_TO_CN_CONVERTER,
         ZhMY => &ZH_TO_MY_CONVERTER,
         ZhSG => &ZH_TO_SG_CONVERTER,
     }
 }
 
-/// Get the builtin conversion table for a target Chinese variant.
-///
-/// Accessing a table is only necessary when building a custom converter.
-/// Otherwise, there is [`get_builtin_converter`].
-#[inline(always)]
-pub fn get_builtin_table(target: Variant) -> (&'static str, &'static str) {
-    use Variant::*;
-    match target {
-        Zh => ("", ""),
-        ZhHant => ZH_HANT_TABLE,
-        ZhHans => ZH_HANS_TABLE,
-        ZhTW => *ZH_HANT_TW_TABLE,
-        ZhHK => *ZH_HANT_HK_TABLE,
-        ZhMO => *ZH_HANT_MO_TABLE,
-        ZhCN => *ZH_HANS_CN_TABLE,
-        ZhMY => *ZH_HANS_MY_TABLE,
-        ZhSG => *ZH_HANS_SG_TABLE,
-    }
+#[doc(hidden)]
+pub fn deserialize_converter(
+    variant: Variant,
+    daac: &[u8],
+    tables: impl IntoIterator<Item = Table<'static>>,
+) -> ZhConverter {
+    #[cfg(feature = "compress")]
+    let daac = zstd_decompress(daac);
+
+    ZhConverter::with_target_variant(
+        unsafe { CharwiseDoubleArrayAhoCorasick::deserialize_unchecked(&daac).0 },
+        tables
+            .into_iter()
+            .flat_map(|t| expand_table(t).map(|(_f, t)| t))
+            .collect(), // TODO: avoid String
+        variant,
+    )
 }
```

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/src/pagerules.rs` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/src/pagerules.rs`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/src/variant.rs` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/src/variant.rs`

 * *Files 9% similar despite different names*

```diff
@@ -17,22 +17,31 @@
 #[derive(
     Clone, Copy, Debug, PartialEq, Eq, Hash, Display, EnumString, EnumVariantNames, IntoStaticStr,
 )]
 #[strum(serialize_all = "kebab_case", ascii_case_insensitive)]
 #[derive(Default)]
 pub enum Variant {
     #[default]
+    /// Chinese (dummy variant)
     Zh,
+    /// Script: Traditional Chinese
     ZhHant,
+    /// Script: Simplified Chinese
     ZhHans,
+    /// Short for `zh-Hant-TW`, Script: Traditional Chinese, Region: Taiwan
     ZhTW,
+    /// Short for`zh-Hant-HK`, Script: Traditional Chinese, Region: Hong Kong
     ZhHK,
+    /// Short for`zh-Hant-MO`, Script: Traditional Chinese, Region: Taiwan
     ZhMO,
+    /// Short for`zh-Hans-MY`, Script: Simplified Chinese, Region: Macau
     ZhMY,
+    /// Short for`zh-Hans-SG`, Script: Simplified Chinese, Region: Singapore
     ZhSG,
+    /// Short for`zh-Hans-CN`, Script: Simplified Chinese, Region: China (mainland)
     ZhCN,
     // Unknown(String)
 }
 
 impl Variant {
     #[inline(always)]
     pub fn get_name(self) -> &'static str {
@@ -84,22 +93,23 @@
         )
         // TODO: falling back to zh finally?
         // even though the rules defined in ZhConverter.php fallbakcs to Zh,
         // tests shows that it display a error when no other more concrete variants available
     }
 
     /// Get the pairs of conversion for a target variant
-    pub fn get_conv_pairs(&self, target: Variant) -> Vec<(&str, &str)> {
+    pub fn get_conv_pairs(&self, target: Variant) -> impl Iterator<Item = (&str, &str)> {
         use Variant::*;
         // TODO: Iterator
         // MEDIAWIKI: the code of the reference implementation is too obscure, try to replicate the
         //            the same behavior based on some tests
+        let mut it = None;
         match target {
-            // based on tests, the three are only used for regional scripts as fallbacks
-            Zh | ZhHant | ZhHans => vec![],
+            // based on tests, the three are only used as fallbacks for regional scripts
+            Zh | ZhHant | ZhHans => (),
             _ => {
                 // It won't fallback to Zh finally. So Zh is only used as from?
                 let to = match_fallback!(
                     self.0,
                     target,
                     // Zh -> [ZhHans, ZhHant, ZhCN, ZhTW, ZhHK, ZhSG, ZhMO, ZhMY],
                     // ZhHans -> [ ZhCN, ZhSG, ZhMY ],
@@ -109,28 +119,27 @@
                     ZhMY -> [ ZhHans, ZhSG, ZhCN ],
                     ZhTW -> [ ZhHant, ZhHK, ZhMO ],
                     ZhHK -> [ ZhHant, ZhMO, ZhTW ],
                     ZhMO -> [ ZhHant, ZhHK, ZhTW ],
                 );
 
                 if let Some(to) = to {
-                    let mut pairs = vec![];
-                    for (_variant, from) in self.0.iter() {
-                        // when variant == target, from == to, which indicates preventing the word
-                        // from converting
-                        if !from.is_empty() {
-                            pairs.push((from.as_ref(), to));
+                    // for variant == target, from == to, it prevents the word from converting
+                    it = Some(self.0.iter().filter_map(move |(_variant, from)| {
+                        if from.is_empty() {
+                            None
+                        } else {
+                            Some((from.as_ref(), to))
                         }
-                    }
-                    pairs
-                } else {
-                    vec![]
+                    }));
                 }
             }
         }
+
+        it.into_iter().flatten()
     }
 }
 
 impl VariantMap<Vec<(String, String)>> {
     /// Get the pairs of conversion for a target variant
     pub fn get_conv_pairs(&self, target: Variant) -> &[(String, String)] {
         // MEDIAWIKI:
```

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/README.md` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/README.md`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/config-overrides.js` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/config-overrides.js`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/package.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/package.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/public/cgroups.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/public/cgroups.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/public/index.html` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/public/index.html`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/public/logo.ico` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/public/logo.ico`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/public/logo192.png` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/public/logo192.png`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/public/logo512.png` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/public/logo512.png`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/src/App.css` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/App.css`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/src/App.tsx` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/App.tsx`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/src/components/AboutDialog.tsx` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/components/AboutDialog.tsx`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/src/components/CGroupCheckbox.tsx` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/components/CGroupCheckbox.tsx`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/src/components/CGroupSelect.tsx` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/components/CGroupSelect.tsx`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/src/components/ConvertButton.tsx` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/components/ConvertButton.tsx`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/src/components/Footer.tsx` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/components/Footer.tsx`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/src/components/Header.tsx` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/components/Header.tsx`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/src/components/InputEditor.tsx` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/components/OutputEditor.tsx`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,30 @@
-import { useMemo } from "react";
-import TextField from "@material-ui/core/TextField";
-// import Paper from "@material-ui/core/Paper";
-import Typography from "@material-ui/core/Typography";
 import Box from "@material-ui/core/Box";
+import TextField from "@material-ui/core/TextField";
 
-import { countLines } from "../utils";
 import { useEditorStyles } from "./editorCommon";
+import OutputStatusLine from "./OutputStatusLine";
 
-export default function InputEditor({
-  input,
-  setInput,
-}: {
-  input: string;
-  setInput: (value: string) => void;
-}) {
+export default function OutputEditor({ output }: { output: any }) {
   const classes = useEditorStyles();
 
   return (
-    <>
+    <Box position="relative">
+      {/* for Fab positioning */}
+      {/* TODO: nowrap */}
       <TextField
         id="input"
-        label="Input / 原文"
-        placeholder="天干物燥，小心火烛。"
+        label="Output / 結果"
+        placeholder="No input"
         multiline
         fullWidth
-        autoFocus
         rows={16}
-        inputProps={{ wrap: "soft", fontSize: "1.2em" }}
-        value={input}
-        onChange={(event) => setInput(event.target.value)}
+        inputProps={{ wrap: "soft" }}
+        value={output ?? ""}
       />
       <Box className={classes.statusLineWrapper}>
-        <Typography variant="caption" color="textSecondary">
-          Lines/橫行: {useMemo(() => countLines(input), [input])}
-          <Box
-            component="span"
-            sx={{ marginLeft: "0.3em", marginRight: "0.3em" }}
-          >
-            ・
-          </Box>
-          Chars/字: {input.length}
-        </Typography>
+        <OutputStatusLine output={output} />
       </Box>
-    </>
+      {/* <WarningFab invalidLines={output?.invalid} /> */}
+    </Box>
   );
 }
```

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/src/components/OptionsControl.tsx` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/components/OptionsControl.tsx`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/src/components/OutputStatusLine.tsx` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/components/OutputStatusLine.tsx`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/src/logo.svg` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/logo.svg`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/tsconfig.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/tsconfig.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/local_dependencies/zhconv/web/yarn.lock` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/yarn.lock`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/Cargo.toml` & `zhconv_rs-0.3.0b0/Cargo.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [package]
 name = "zhconv-pyo3"
-version = "0.2.0-beta"
+version = "0.3.0-beta"
 edition = "2021"
 authors = ["Hung-I Wang <whygowe@gmail.com>"]
 license = "GPL-2.0-or-later"
 repository = "https://github.com/Gowee/zhconv-rs"
-description = "zhconv as in MediaWiki, oxidized with more efficiency 🦀"
+description = "zhconv as in MediaWiki with extra rulesets from OpenCC, oxidized with more efficiency 🦀"
 
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "zhconv_rs"
 crate-type = ["cdylib"]
 
 [dependencies]
 zhconv = { path = "local_dependencies/zhconv" }
 pyo3 = { version = "0.16", features = ["extension-module"] }
-pyo3-file = "0.5"
+pyo3-file = "0.5.0"
+
```

### Comparing `zhconv_rs-0.2.0b0/.gitignore` & `zhconv_rs-0.3.0b0/.gitignore`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/README.md` & `zhconv_rs-0.3.0b0/README.md`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/pyproject.toml` & `zhconv_rs-0.3.0b0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.2.0b0/src/lib.rs` & `zhconv_rs-0.3.0b0/src/lib.rs`

 * *Files 7% similar despite different names*

```diff
@@ -5,34 +5,34 @@
 use pyo3::exceptions::PyTypeError;
 use pyo3::prelude::*;
 use pyo3::types::PyString;
 
 use pyo3_file::PyFileLikeObject;
 
 use ::zhconv::{
-    get_builtin_table, zhconv as zhconv_plain, zhconv_mw, Variant, ZhConverter as Converter,
+    get_builtin_tables, zhconv as zhconv_plain, zhconv_mw, Variant, ZhConverter as Converter,
     ZhConverterBuilder,
 };
 
-/// zhconv(text, target[, mediawiki]) -> result
+/// zhconv(text, target[, wikitext]) -> result
 ///
 /// Convert a text to a target Chinese variant. Converters are constructed from built-in rulesets
-/// on demand and cached automatically. If `mediawiki` is `True`, inline conversion rules such as
+/// on demand and cached automatically. If `wikitext` is `True`, inline conversion rules such as
 /// `-{foo...bar}-` are activated, while converters must be rebuilt for every invocation if there
 /// are global rules. Check the project's README for more info.
 ///
 /// Supported target variants: zh, zh-Hant, zh-Hans, zh-TW, zh-HK, zh-MO, zh-CN, zh-SG, zh-MY.
 #[pyfunction]
-fn zhconv(py: Python<'_>, text: &str, target: &str, mediawiki: Option<bool>) -> PyResult<String> {
+fn zhconv(py: Python<'_>, text: &str, target: &str, wikitext: Option<bool>) -> PyResult<String> {
     py.allow_threads(move || {
         let target = Variant::from_str(target).map_err(|_e| {
             PyTypeError::new_err(format!("Unsupported target variant: {}", target))
         })?;
-        let mediawiki = mediawiki.unwrap_or(false);
-        Ok(if mediawiki {
+        let wikitext = wikitext.unwrap_or(false);
+        Ok(if wikitext {
             zhconv_mw(text, target)
         } else {
             zhconv_plain(text, target)
         })
     })
 }
 
@@ -46,44 +46,37 @@
 #[pymethods]
 impl ZhConverter {
     fn __call__(&self, py: Python<'_>, text: &str) -> String {
         py.allow_threads(move || self.0.convert(text))
     }
 }
 
-/// make_converter(base, rules, dfa = True) -> converter
+/// make_converter(base, rules) -> converter
 ///
 /// Make a converter with custom conversion rules, optionally based on a built-in ruleset
 /// specified by the `base` target variant. Rules can be an array of `(from, to)` pairs, a file
-/// path or a file-like object.
-///
-/// With DFA activated by default, the converter takes more time to build while converts more
-/// efficiently. All built-in converters used be `zhconv` have this feature enabled for better
-/// conversion performance.
+/// path or a file-like object that consists of space-seperated pairs line by line.
 ///
 /// The returned converter is a callable function of the type `ZhConverter`:
 ///
 /// converter(text) -> result
 #[pyfunction]
 fn make_converter(
     py: Python<'_>,
     base: Option<&str>,
     rules: PyObject,
-    dfa: Option<bool>,
 ) -> PyResult<ZhConverter> {
     let base = base
         .and_then(|base| base.try_into().ok())
         .unwrap_or(Variant::Zh);
     let mut builder = ZhConverterBuilder::new()
-        .dfa(dfa.unwrap_or(true))
-        .table(get_builtin_table(base));
+        .target(base)
+        .tables(get_builtin_tables(base));
     if let Ok(pairs) = rules.extract::<Vec<(String, String)>>(py) {
-        for (from, to) in pairs.into_iter() {
-            builder = builder.add_conv_pair(from, to);
-        }
+        builder = builder.conv_pairs(pairs.into_iter());
     } else {
         let mut text = String::new();
 
         if let Ok(string_ref) = rules.cast_as::<PyString>(py) {
             // path
             let path = string_ref.to_str()?;
             File::open(path)?.read_to_string(&mut text)?;
@@ -95,15 +88,15 @@
 
         for (i, line) in text.lines().map(|line| line.trim()).enumerate() {
             if line.starts_with('#') {
                 continue;
             }
             if let Some((from, to)) = line.split_once(char::is_whitespace) {
                 let to = to.trim_start_matches(char::is_whitespace);
-                builder = builder.add_conv_pair(from, to);
+                builder = builder.conv_pairs([(from, to)]);
             } else {
                 return Err(PyTypeError::new_err(format!(
                     "Invalid conversion rule at line {}: {}",
                     i + 1,
                     line
                 )));
             }
@@ -115,15 +108,15 @@
 
 /// zhconv as in MediaWiki, oxidized with much more efficiency.
 ///
 /// Convert with builtin rulesets:
 /// ```python
 /// from zhconv_rs import zhconv
 /// assert zhconv("天干物燥 小心火烛", "zh-tw") == "天乾物燥 小心火燭"
-/// assert zhconv("《-{zh-hans:三个火枪手;zh-hant:三劍客;zh-tw:三劍客}-》是亞歷山大·仲馬的作品。", "zh-cn", mediawiki=True) == "《三个火枪手》是亚历山大·仲马的作品。"
+/// assert zhconv("《-{zh-hans:三个火枪手;zh-hant:三劍客;zh-tw:三劍客}-》是亞歷山大·仲馬的作品。", "zh-cn", wikitext=True) == "《三个火枪手》是亚历山大·仲马的作品。"
 /// assert zhconv("-{H|zh-cn:雾都孤儿;zh-tw:孤雛淚;zh-hk:苦海孤雛;zh-sg:雾都孤儿;zh-mo:苦海孤雛;}-《雾都孤儿》是查尔斯·狄更斯的作品。", "zh-tw", True) == "《孤雛淚》是查爾斯·狄更斯的作品。"
 /// ```
 ///
 /// Convert with custom rules:
 /// ```python
 /// from zhconv_rs import make_converter
 /// assert make_converter(None, [("天", "地"), ("水", "火")])("甘肅天水") == "甘肅地火"
```

### Comparing `zhconv_rs-0.2.0b0/zhconv_rs.pyi` & `zhconv_rs-0.3.0b0/zhconv_rs.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Optional, Union, Literal, Sequence, Tuple, TextIO, Callable
 
+# TODO: case-insensitive literal
 ZhVariant = Union[
     Literal["zh"],  # dummy for nothing
     Literal["zh-Hant"],
     Literal["zh-Hans"],
     Literal["zh-TW"],
     Literal["zh-HK"],
     Literal["zh-MO"],
@@ -16,14 +17,14 @@
     Literal["zh-hk"],
     Literal["zh-mo"],
     Literal["zh-cn"],
     Literal["zh-sg"],
     Literal["zh-my"],
 ]
 
-def zhconv(text: str, target: ZhVariant, mediawiki: bool = False) -> str:
+def zhconv(text: str, target: ZhVariant, wikitext: bool = False) -> str:
     pass
 
 def make_converter(
     base: Optional[ZhVariant], rules: Union[Sequence[Tuple[str, str]], str, TextIO]
 ) -> Callable[[str], str]:
     pass
```

### Comparing `zhconv_rs-0.2.0b0/Cargo.lock` & `zhconv_rs-0.3.0b0/Cargo.lock`

 * *Files 8% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 checksum = "1e37cfd5e7657ada45f742d6e99ca5788580b5c529dc78faf11ece6dc702656f"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "1.0.1"
+version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "67fc08ce920c31afb70f013dcce1bfc3a3195de6a228474e45e1f145b36f8d04"
+checksum = "43f6cb1bf222025340178f382c426f13757b2960e89779dfcb319c32542a5a41"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "anyhow"
 version = "1.0.71"
@@ -56,14 +56,20 @@
 [[package]]
 name = "bytecount"
 version = "0.6.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2c676a478f63e9fa2dd5368a42f28bba0d6c560b775f38583c8bbaa7fcd67c9c"
 
 [[package]]
+name = "byteorder"
+version = "1.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "14c189c53d098945499cdfa7ecc63567cf3886b3332b312a5b4585d8d3a6a610"
+
+[[package]]
 name = "camino"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "35176a56fa5f5efe08df85cd5e68158471c2fa7057e85a5356ee4bd9787a6df9"
 dependencies = [
  "serde",
 ]
@@ -87,14 +93,23 @@
  "cargo-platform",
  "semver",
  "serde",
  "serde_json",
 ]
 
 [[package]]
+name = "cc"
+version = "1.0.79"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
+dependencies = [
+ "jobserver",
+]
+
+[[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "console_error_panic_hook"
@@ -122,14 +137,20 @@
 checksum = "1bfb12502f3fc46cca1bb51ac28df9d618d813cdc3d2f25b9fe775a34af26bb3"
 dependencies = [
  "generic-array",
  "typenum",
 ]
 
 [[package]]
+name = "daachorse"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "63b7ef7a4be509357f4804d0a22e830daddb48f19fd604e4ad32ddce04a94c36"
+
+[[package]]
 name = "digest"
 version = "0.10.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f2fb860ca6fafa5552fb6d0e816a69c8e49f0908bf524e30a90d97c85892d506"
 dependencies = [
  "block-buffer",
  "crypto-common",
@@ -214,14 +235,23 @@
 [[package]]
 name = "itoa"
 version = "1.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c8af84674fe1f223a982c933a0ee1086ac4d4052aa0fb8060c12c6ad838e754"
 
 [[package]]
+name = "jobserver"
+version = "0.1.26"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "936cfd212a0155903bcbc060e316fb6cc7cbf2e1907329391ebadc1fe0ce77c2"
+dependencies = [
+ "libc",
+]
+
+[[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
@@ -245,14 +275,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
+name = "lz4_flex"
+version = "0.10.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8b8c72594ac26bfd34f2d99dfced2edfaddfe8a476e3ff2ca0eb293d925c4f83"
+dependencies = [
+ "twox-hash",
+]
+
+[[package]]
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
 [[package]]
 name = "once_cell"
@@ -280,14 +319,20 @@
  "libc",
  "redox_syscall",
  "smallvec",
  "windows-sys",
 ]
 
 [[package]]
+name = "pkg-config"
+version = "0.3.27"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "26072860ba924cbfa98ea39c8c19b4dd6a4a25423dbdf219c1eca91aa0cf6964"
+
+[[package]]
 name = "proc-macro2"
 version = "1.0.43"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0a2ca2c61bc9f3d74d2886294ab7b9853abd9c1ad903a3ac7815c58989bb7bab"
 dependencies = [
  "unicode-ident",
 ]
@@ -419,14 +464,25 @@
 [[package]]
 name = "rustversion"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4f3208ce4d8448b3f3e7d168a73f5e0c43a61e32930de3bceeccedb388b6bf06"
 
 [[package]]
+name = "ruzstd"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ac3ffab8f9715a0d455df4bbb9d21e91135aab3cd3ca187af0cd0c3c3f868fdc"
+dependencies = [
+ "byteorder",
+ "thiserror-core",
+ "twox-hash",
+]
+
+[[package]]
 name = "ryu"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4501abdff3ae82a1c1b477a17252eb69cee9e66eb915c1abaa4f44d873df9f09"
 
 [[package]]
 name = "same-file"
@@ -512,14 +568,20 @@
 [[package]]
 name = "smallvec"
 version = "1.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2fd0db749597d91ff862fd1d55ea87f7855a744a8425a64695b6fca237d1dad1"
 
 [[package]]
+name = "static_assertions"
+version = "1.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a2eb9349b6444b326872e140eb1cf5e7c522154d69e7a0ffb0fb81c06b37543f"
+
+[[package]]
 name = "strum"
 version = "0.24.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "063e6045c0e62079840579a7e47a355ae92f60eb74daaf156fb1e84ba164e63f"
 dependencies = [
  "strum_macros",
 ]
@@ -565,14 +627,71 @@
  "libc",
  "redox_syscall",
  "remove_dir_all",
  "winapi",
 ]
 
 [[package]]
+name = "thiserror-core"
+version = "1.0.38"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0d97345f6437bb2004cd58819d8a9ef8e36cdd7661c2abc4bbde0a7c40d9f497"
+dependencies = [
+ "thiserror-core-impl",
+]
+
+[[package]]
+name = "thiserror-core-impl"
+version = "1.0.38"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "10ac1c5050e43014d16b2f94d0d2ce79e65ffdd8b38d8048f9c8f6a8a6da62ac"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn",
+]
+
+[[package]]
+name = "time"
+version = "0.3.22"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ea9e1b3cf1243ae005d9e74085d4d542f3125458f3a81af210d901dcd7411efd"
+dependencies = [
+ "itoa",
+ "serde",
+ "time-core",
+ "time-macros",
+]
+
+[[package]]
+name = "time-core"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7300fbefb4dadc1af235a9cef3737cea692a9d97e1b9cbcd4ebdae6f8868e6fb"
+
+[[package]]
+name = "time-macros"
+version = "0.2.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "372950940a5f07bf38dbe211d7283c9e6d7327df53794992d293e534c733d09b"
+dependencies = [
+ "time-core",
+]
+
+[[package]]
+name = "twox-hash"
+version = "1.6.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "97fee6b57c6a41524a810daee9286c02d7752c4253064d0b05472833a438f675"
+dependencies = [
+ "cfg-if",
+ "static_assertions",
+]
+
+[[package]]
 name = "typenum"
 version = "1.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dcf81ac59edc17cc8697ff311e8f5ef2d99fcbd9817b34cec66f90b6c3dfd987"
 
 [[package]]
 name = "unicase"
@@ -593,20 +712,21 @@
 name = "unindent"
 version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "58ee9362deb4a96cef4d437d1ad49cffc9b9e92d202b6995674e928ce684f112"
 
 [[package]]
 name = "vergen"
-version = "8.1.3"
+version = "8.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6e03272e388fb78fc79481a493424f78d77be1d55f21bcd314b5a6716e195afe"
+checksum = "8b3c89c2c7e50f33e4d35527e5bf9c11d6d132226dbbd1753f0fbe9f19ef88c6"
 dependencies = [
  "anyhow",
  "rustversion",
+ "time",
 ]
 
 [[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
@@ -748,30 +868,64 @@
 name = "windows_x86_64_msvc"
 version = "0.36.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c811ca4a8c853ef420abd8592ba53ddbbac90410fab6903b3e79972a631f7680"
 
 [[package]]
 name = "zhconv"
-version = "0.2.0-beta"
+version = "0.3.0-beta"
 dependencies = [
- "aho-corasick 1.0.1",
+ "aho-corasick 1.0.2",
  "console_error_panic_hook",
+ "daachorse",
  "hex-literal",
  "itertools",
  "lazy_static",
+ "lz4_flex",
  "once_cell",
  "regex",
+ "ruzstd",
  "sha2",
  "strum",
  "vergen",
  "wasm-bindgen",
+ "zstd",
 ]
 
 [[package]]
 name = "zhconv-pyo3"
-version = "0.2.0-beta"
+version = "0.3.0-beta"
 dependencies = [
  "pyo3",
  "pyo3-file",
  "zhconv",
 ]
+
+[[package]]
+name = "zstd"
+version = "0.12.3+zstd.1.5.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "76eea132fb024e0e13fd9c2f5d5d595d8a967aa72382ac2f9d39fcc95afd0806"
+dependencies = [
+ "zstd-safe",
+]
+
+[[package]]
+name = "zstd-safe"
+version = "6.0.5+zstd.1.5.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d56d9e60b4b1758206c238a10165fbcae3ca37b01744e394c463463f6529d23b"
+dependencies = [
+ "libc",
+ "zstd-sys",
+]
+
+[[package]]
+name = "zstd-sys"
+version = "2.0.8+zstd.1.5.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5556e6ee25d32df2586c098bbfa278803692a20d0ab9565e049480d52707ec8c"
+dependencies = [
+ "cc",
+ "libc",
+ "pkg-config",
+]
```

### Comparing `zhconv_rs-0.2.0b0/PKG-INFO` & `zhconv_rs-0.3.0b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: zhconv-rs
-Version: 0.2.0b0
+Version: 0.3.0b0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Natural Language :: Chinese (Traditional)
 Classifier: Natural Language :: Chinese (Simplified)
-Summary: zhconv as in MediaWiki, oxidized with more efficiency 🦀
+Summary: zhconv as in MediaWiki with extra rulesets from OpenCC, oxidized with more efficiency 🦀
 Author: Hung-I Wang <whygowe@gmail.com>
 Author-email: Hung-I Wang <whygowe@gmail.com>
 License: GPL-2.0-or-later
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source, https://github.com/Gowee/zhconv-rs/tree/main/pyo3
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: zhconv-rs Version: 0.2.0b0 Classifier: Programming
+Metadata-Version: 2.1 Name: zhconv-rs Version: 0.3.0b0 Classifier: Programming
 Language :: Rust Classifier: Programming Language :: Python :: Implementation
 :: CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Text Processing :: Linguistic Classifier: Natural Language
 :: Chinese (Traditional) Classifier: Natural Language :: Chinese (Simplified)
-Summary: zhconv as in MediaWiki, oxidized with more efficiency ð¦ Author:
-Hung-I Wang
+Summary: zhconv as in MediaWiki with extra rulesets from OpenCC, oxidized with
+more efficiency ð¦ Author: Hung-I Wang
 gmail.com> Author-email: Hung-I Wang
 gmail.com> License: GPL-2.0-or-later Requires-Python: >=3.7 Description-
 Content-Type: text/markdown; charset=UTF-8; variant=GFM Project-URL: Source,
 https://github.com/Gowee/zhconv-rs/tree/main/pyo3 [![CI status](https://
 github.com/Gowee/zhconv-rs/actions/workflows/main.yml/badge.svg)](https://
 github.com/Gowee/zhconv-rs/actions) [![docs.rs](https://docs.rs/zhconv/
 badge.svg)](https://docs.rs/zhconv) [![Crates.io](https://img.shields.io/
```

