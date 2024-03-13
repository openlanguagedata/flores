# The FLORES+ evaluation benchmark for multilingual machine translation

This repository hosts the open source FLORES+ machine translation evaluation benchmark, released under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/). This dataset was originally released by FAIR researchers at Meta under the name FLORES. Further information about these initial releases can be found in the [papers below](#citation). The data is now being managed by OLDI, the [Open Language Data Initiative](https://oldi.org). The `+` has been added to the name to disambiguate between the original datasets and this new actively developed version.

## Data

For each language, the dataset has 997 sentences for the `dev` split and 1012 sentences for the `devtest` split. The separate blind `test` set, originally developed by Meta, is not managed by OLDI and not part of this repository. 

The English sentences were sampled in equal amounts from <a href="https://en.wikinews.org/">Wikinews</a> (an international news source), <a href="https://en.wikibooks.org/wiki/Wikijunior">Wikijunior</a> (a collection of age-appropriate non-fiction books), and <a href="https://en.wikivoyage.org/">Wikivoyage</a> (a travel guide). These were then translated into other languages.

## Download the dataset

The latest version of the dataset can be downloaded in the Releases tab of this repository. It is available as a zip archive, with password `multilingual machine translation`. The data is only available in this format in order to avoid it being picked up by crawlers, which would lead to it being accidentally included in the sort of web corpora often used to train LLMs and large scale machine translation models, rendering it useless as a benchmark.

⚠️ **Please note** ⚠️:
1. Please do not re-host this data as plain text in places where it might be picked up by web crawlers.
2. If you are planning on evaluating your model with FLORES+, you should ensure its contents are not in your training data.

## Contributing

Fixes and new language contributions are most welcome. Please see the [Contribution guidelines](https://oldi.org/guidelines) for further information.

## Language coverage

|    Code    |  Variety   |                Name                 |                           Notes                            |
|------------|------------|-------------------------------------|------------------------------------------------------------|
| `ace_Arab` | `achi1257` |       Acehnese (Arabic script)      |                                                            |
| `ace_Latn` | `achi1257` |       Acehnese (Latin script)       |                                                            |
| `acm_Arab` | `meso1252` |         Mesopotamian Arabic         | [[1]](https://github.com/openlanguagedata/flores/issues/8) |
| `acq_Arab` | `taiz1242` |         Taʽizzi-Adeni Arabic        | [[1]](https://github.com/openlanguagedata/flores/issues/8) |
| `aeb_Arab` | `tuni1259` |           Tunisian Arabic           |                                                            |
| `afr_Latn` | `afri1274` |              Afrikaans              |                                                            |
| `als_Latn` | `tosk1239` |           Albanian (Tosk)           |                                                            |
| `amh_Ethi` | `amha1245` |               Amharic               |                                                            |
| `apc_Arab` | `nort3139` |       Levantine Arabic (North)      | [[1]](https://github.com/openlanguagedata/flores/issues/7) |
| `apc_Arab` | `sout3123` |       Levantine Arabic (South)      | [[1]](https://github.com/openlanguagedata/flores/issues/7) |
| `arb_Arab` | `stan1318` |        Modern Standard Arabic       |                                                            |
| `arb_Latn` | `stan1318` |  Modern Standard Arabic (Romanized) |                                                            |
| `ars_Arab` | `najd1235` |             Najdi Arabic            | [[1]](https://github.com/openlanguagedata/flores/issues/8) |
| `ary_Arab` | `moro1292` |           Moroccan Arabic           |                                                            |
| `arz_Arab` | `egyp1253` |           Egyptian Arabic           |                                                            |
| `asm_Beng` | `assa1263` |               Assamese              |                                                            |
| `ast_Latn` | `astu1245` |               Asturian              |                                                            |
| `awa_Deva` | `awad1243` |                Awadhi               |                                                            |
| `ayr_Latn` | `cent2142` |            Central Aymara           |                                                            |
| `azb_Arab` | `sout2697` |          South Azerbaijani          |                                                            |
| `azj_Latn` | `nort2697` |          North Azerbaijani          |                                                            |
| `bak_Cyrl` | `bash1264` |               Bashkir               |                                                            |
| `bam_Latn` | `bamb1269` |               Bambara               |                                                            |
| `ban_Latn` | `bali1278` |               Balinese              |                                                            |
| `bel_Cyrl` | `bela1254` |              Belarusian             |                                                            |
| `bem_Latn` | `bemb1257` |                Bemba                |                                                            |
| `ben_Beng` | `beng1280` |               Bengali               |                                                            |
| `bho_Deva` | `bhoj1244` |               Bhojpuri              |                                                            |
| `bjn_Arab` | `banj1239` |         Banjar (Jawi script)        |                                                            |
| `bjn_Latn` | `banj1239` |        Banjar (Latin script)        |                                                            |
| `bod_Tibt` | `utsa1239` |            Lhasa Tibetan            |                                                            |
| `bos_Latn` | `bosn1245` |               Bosnian               |                                                            |
| `brx_Deva` | `bodo1269` |                 Bodo                |                         `dev` only                         |
| `bug_Latn` | `bugi1244` |               Buginese              |                                                            |
| `bul_Cyrl` | `bulg1262` |              Bulgarian              |                                                            |
| `cat_Latn` | `stan1289` |               Catalan               |                                                            |
| `ceb_Latn` | `cebu1242` |               Cebuano               |                                                            |
| `ces_Latn` | `czec1258` |                Czech                |                                                            |
| `chv_Cyrl` | `chuv1255` |               Chuvash               |                         `dev` only                         |
| `cjk_Latn` | `chok1245` |                Chokwe               |                                                            |
| `ckb_Arab` | `cent1972` |           Central Kurdish           |                                                            |
| `cmn_Hans` | `beij1234` | Mandarin Chinese (Standard Beijing) |                                                            |
| `cmn_Hant` | `taib1240` |     Mandarin Chinese (Taiwanese)    |                                                            |
| `crh_Latn` | `crim1257` |            Crimean Tatar            |                                                            |
| `cym_Latn` | `wels1247` |                Welsh                |                                                            |
| `dan_Latn` | `dani1285` |                Danish               |                                                            |
| `deu_Latn` | `stan1295` |                German               |                                                            |
| `dgo_Deva` | `dogr1250` |                Dogri                |                         `dev` only                         |
| `dik_Latn` | `sout2832` |          Southwestern Dinka         |                                                            |
| `dyu_Latn` | `dyul1238` |                Dyula                |                                                            |
| `dzo_Tibt` | `dzon1239` |               Dzongkha              |                                                            |
| `ekk_Latn` | `esto1258` |               Estonian              |                                                            |
| `ell_Grek` | `mode1248` |                Greek                |                                                            |
| `eng_Latn` | `stan1293` |               English               |                                                            |
| `epo_Latn` | `espe1235` |              Esperanto              |                                                            |
| `eus_Latn` | `basq1248` |                Basque               |                                                            |
| `ewe_Latn` | `ewee1241` |                 Ewe                 |                                                            |
| `fao_Latn` | `faro1244` |               Faroese               |                                                            |
| `fij_Latn` | `fiji1243` |                Fijian               |                                                            |
| `fil_Latn` | `fili1244` |               Filipino              |                                                            |
| `fin_Latn` | `finn1318` |               Finnish               |                                                            |
| `fon_Latn` | `fonn1241` |                 Fon                 |                                                            |
| `fra_Latn` | `stan1290` |                French               |                                                            |
| `fur_Latn` | `east2271` |               Friulian              |                                                            |
| `fuv_Latn` | `nige1253` |          Nigerian Fulfulde          |                                                            |
| `gaz_Latn` | `west2721` |          West Central Oromo         |                                                            |
| `gla_Latn` | `scot1245` |           Scottish Gaelic           |                                                            |
| `gle_Latn` | `iris1253` |                Irish                |                                                            |
| `glg_Latn` | `gali1258` |               Galician              |                                                            |
| `gom_Deva` | `goan1235` |             Goan Konkani            |                                                            |
| `gug_Latn` | `para1311` |          Paraguayan Guaraní         |                                                            |
| `guj_Gujr` | `guja1252` |               Gujarati              |                                                            |
| `hat_Latn` | `hait1244` |            Haitian Creole           |                                                            |
| `hau_Latn` | `haus1257` |                Hausa                |                                                            |
| `heb_Hebr` | `hebr1245` |                Hebrew               |                                                            |
| `hin_Deva` | `hind1269` |                Hindi                |                                                            |
| `hne_Deva` | `chha1249` |            Chhattisgarhi            |                                                            |
| `hrv_Latn` | `croa1245` |               Croatian              |                                                            |
| `hun_Latn` | `hung1274` |              Hungarian              |                                                            |
| `hye_Armn` | `nucl1235` |               Armenian              |                                                            |
| `ibo_Latn` | `nucl1417` |                 Igbo                |                                                            |
| `ilo_Latn` | `ilok1237` |               Ilocano               |                                                            |
| `ind_Latn` | `indo1316` |              Indonesian             |                                                            |
| `isl_Latn` | `icel1247` |              Icelandic              |                                                            |
| `ita_Latn` | `ital1282` |               Italian               |                                                            |
| `jav_Latn` | `java1254` |               Javanese              |                                                            |
| `jpn_Jpan` | `nucl1643` |               Japanese              |                                                            |
| `kab_Latn` | `kaby1243` |                Kabyle               |                                                            |
| `kac_Latn` | `kach1280` |               Jingpho               |                                                            |
| `kam_Latn` | `kamb1297` |                Kamba                |                                                            |
| `kan_Knda` | `nucl1305` |               Kannada               |                                                            |
| `kas_Arab` | `kash1277` |       Kashmiri (Arabic script)      |                                                            |
| `kas_Deva` | `kash1277` |     Kashmiri (Devanagari script)    |                                                            |
| `kat_Geor` | `nucl1302` |               Georgian              |                                                            |
| `kaz_Cyrl` | `kaza1248` |                Kazakh               |                                                            |
| `kbp_Latn` | `kabi1261` |                Kabiyè               |                                                            |
| `kea_Latn` | `kabu1256` |             Kabuverdianu            |                                                            |
| `khk_Cyrl` | `halh1238` |            Halh Mongolian           |                                                            |
| `khm_Khmr` | `cent1989` |           Khmer (Central)           |                                                            |
| `kik_Latn` | `kiku1240` |                Kikuyu               |                                                            |
| `kin_Latn` | `kiny1244` |             Kinyarwanda             |                                                            |
| `kir_Cyrl` | `kirg1245` |                Kyrgyz               |                                                            |
| `kmb_Latn` | `kimb1241` |               Kimbundu              |                                                            |
| `kmr_Latn` | `nort2641` |           Northern Kurdish          |                                                            |
| `knc_Arab` | `cent2050` |    Central Kanuri (Arabic script)   |                                                            |
| `knc_Latn` | `cent2050` |    Central Kanuri (Latin script)    |                                                            |
| `kor_Hang` | `kore1280` |                Korean               |                                                            |
| `ktu_Latn` | `kitu1246` |             Kituba (DRC)            |                                                            |
| `lao_Laoo` | `laoo1244` |                 Lao                 |                                                            |
| `lij_Latn` | `geno1240` |          Ligurian (Genoese)         |                                                            |
| `lim_Latn` | `limb1263` |              Limburgish             |                                                            |
| `lin_Latn` | `ling1263` |               Lingala               |                                                            |
| `lit_Latn` | `lith1251` |              Lithuanian             |                                                            |
| `lmo_Latn` | `lomb1257` |               Lombard               | [[1]](https://github.com/openlanguagedata/flores/issues/5) |
| `ltg_Latn` | `east2282` |              Latgalian              |                                                            |
| `ltz_Latn` | `luxe1241` |            Luxembourgish            |                                                            |
| `lua_Latn` | `luba1249` |              Luba-Kasai             |                                                            |
| `lug_Latn` | `gand1255` |                Ganda                |                                                            |
| `luo_Latn` | `luok1236` |                 Luo                 |                                                            |
| `lus_Latn` | `lush1249` |                 Mizo                |                                                            |
| `lvs_Latn` | `stan1325` |           Standard Latvian          |                                                            |
| `mag_Deva` | `maga1260` |                Magahi               |                                                            |
| `mai_Deva` | `mait1250` |               Maithili              |                                                            |
| `mal_Mlym` | `mala1464` |              Malayalam              |                                                            |
| `mar_Deva` | `mara1378` |               Marathi               |                                                            |
| `mhr_Cyrl` | `gras1239` |             Meadow Mari             |                         `dev` only                         |
| `min_Arab` | `mina1268` |      Minangkabau (Jawi script)      |                                                            |
| `min_Latn` | `mina1268` |      Minangkabau (Latin script)     |                                                            |
| `mkd_Cyrl` | `mace1250` |              Macedonian             |                                                            |
| `mlt_Latn` | `malt1254` |               Maltese               |                                                            |
| `mni_Beng` | `mani1292` |  Meitei (Manipuri, Bengali script)  |                                                            |
| `mni_Mtei` | `mani1292` |   Meitei (Manipuri, Meitei script)  |                         `dev` only                         |
| `mos_Latn` | `moss1236` |                Mossi                |                                                            |
| `mri_Latn` | `maor1246` |                Maori                |                                                            |
| `mya_Mymr` | `nucl1310` |               Burmese               |                                                            |
| `nld_Latn` | `dutc1256` |                Dutch                |                                                            |
| `nno_Latn` | `norw1262` |          Norwegian Nynorsk          |                                                            |
| `nob_Latn` | `norw1259` |           Norwegian Bokmål          |                                                            |
| `npi_Deva` | `nepa1254` |                Nepali               |                                                            |
| `nqo_Nkoo` | `nkoa1234` |                 Nko                 |                                                            |
| `nso_Latn` | `pedi1238` |            Northern Sotho           |                                                            |
| `nus_Latn` | `nuer1246` |                 Nuer                |                                                            |
| `nya_Latn` | `nyan1308` |                Nyanja               |                                                            |
| `oci_Latn` | `occi1239` |               Occitan               |                                                            |
| `ory_Orya` | `oriy1255` |                 Odia                |                                                            |
| `pag_Latn` | `pang1290` |              Pangasinan             |                                                            |
| `pan_Guru` | `panj1256` |           Eastern Panjabi           |                                                            |
| `pap_Latn` | `papi1253` |              Papiamento             |                                                            |
| `pbt_Arab` | `sout2649` |           Southern Pashto           |                                                            |
| `pes_Arab` | `west2369` |           Western Persian           |                                                            |
| `plt_Latn` | `plat1254` |           Plateau Malagasy          |                                                            |
| `pol_Latn` | `poli1260` |                Polish               |                                                            |
| `por_Latn` | `braz1246` |        Portuguese (Brazilian)       |                                                            |
| `prs_Arab` | `dari1249` |                 Dari                |                                                            |
| `quy_Latn` | `ayac1239` |           Ayacucho Quechua          |                                                            |
| `ron_Latn` | `roma1327` |               Romanian              |                                                            |
| `run_Latn` | `rund1242` |                Rundi                |                                                            |
| `rus_Cyrl` | `russ1263` |               Russian               |                                                            |
| `sag_Latn` | `sang1328` |                Sango                |                                                            |
| `san_Deva` | `sans1269` |               Sanskrit              |                                                            |
| `sat_Olck` | `sant1410` |               Santali               |                                                            |
| `scn_Latn` | `sici1248` |               Sicilian              |                                                            |
| `shn_Mymr` | `shan1277` |                 Shan                |                                                            |
| `sin_Sinh` | `sinh1246` |               Sinhala               |                                                            |
| `slk_Latn` | `slov1269` |                Slovak               |                                                            |
| `slv_Latn` | `slov1268` |              Slovenian              |                                                            |
| `smo_Latn` | `samo1305` |                Samoan               |                                                            |
| `sna_Latn` | `shon1251` |                Shona                |                                                            |
| `snd_Arab` | `sind1272` |        Sindhi (Arabic script)       |                                                            |
| `snd_Deva` | `sind1272` |      Sindhi (Devanagari script)     |                         `dev` only                         |
| `som_Latn` | `soma1255` |                Somali               |                                                            |
| `sot_Latn` | `sout2807` |            Southern Sotho           |                                                            |
| `spa_Latn` | `amer1254` |       Spanish (Latin American)      |                                                            |
| `srd_Latn` | `sard1257` |              Sardinian              | [[1]](https://github.com/openlanguagedata/flores/issues/6) |
| `srp_Cyrl` | `serb1264` |               Serbian               |                                                            |
| `ssw_Latn` | `swat1243` |                Swati                |                                                            |
| `sun_Latn` | `sund1252` |              Sundanese              |                                                            |
| `swe_Latn` | `swed1254` |               Swedish               |                                                            |
| `swh_Latn` | `swah1253` |               Swahili               |                                                            |
| `szl_Latn` | `sile1253` |               Silesian              |                                                            |
| `tam_Taml` | `tami1289` |                Tamil                |                                                            |
| `taq_Latn` | `tama1365` |       Tamasheq (Latin script)       |                                                            |
| `taq_Tfng` | `tama1365` |      Tamasheq (Tifinagh script)     |                                                            |
| `tat_Cyrl` | `tata1255` |                Tatar                |                                                            |
| `tel_Telu` | `telu1262` |                Telugu               |                                                            |
| `tgk_Cyrl` | `taji1245` |                Tajik                |                                                            |
| `tha_Thai` | `thai1261` |                 Thai                |                                                            |
| `tir_Ethi` | `tigr1271` |               Tigrinya              |                                                            |
| `tpi_Latn` | `tokp1240` |              Tok Pisin              |                                                            |
| `tsn_Latn` | `tswa1253` |                Tswana               |                                                            |
| `tso_Latn` | `tson1249` |                Tsonga               |                                                            |
| `tuk_Latn` | `turk1304` |               Turkmen               |                                                            |
| `tum_Latn` | `tumb1250` |               Tumbuka               |                                                            |
| `tur_Latn` | `nucl1301` |               Turkish               |                                                            |
| `twi_Latn` | `akua1239` |             Akuapem Twi             |                                                            |
| `twi_Latn` | `asan1239` |              Asante Twi             |                                                            |
| `uig_Arab` | `uigh1240` |                Uyghur               |                                                            |
| `ukr_Cyrl` | `ukra1253` |              Ukrainian              |                                                            |
| `umb_Latn` | `umbu1257` |               Umbundu               |                                                            |
| `urd_Arab` | `urdu1245` |                 Urdu                |                                                            |
| `uzn_Latn` | `nort2690` |            Northern Uzbek           |                                                            |
| `vec_Latn` | `vene1259` |               Venetian              |                                                            |
| `vie_Latn` | `viet1252` |              Vietnamese             |                                                            |
| `war_Latn` | `wara1300` |                Waray                |                                                            |
| `wol_Latn` | `nucl1347` |                Wolof                |                                                            |
| `xho_Latn` | `xhos1239` |                Xhosa                |                                                            |
| `ydd_Hebr` | `east2295` |           Eastern Yiddish           |                                                            |
| `yor_Latn` | `yoru1245` |                Yoruba               |                                                            |
| `yue_Hant` | `xian1255` |  Yue Chinese (Hong Kong Cantonese)  |                                                            |
| `zgh_Tfng` | `stan1324` |     Standard Moroccan Tamazight     |                                                            |
| `zsm_Latn` | `stan1306` |            Standard Malay           |                                                            |
| `zul_Latn` | `zulu1248` |                 Zulu                |                                                            |


## Citation

This dataset is based upon FLORES-200, described in the following paper:

```bibtex
@article{nllb-22,
    title = {No Language Left Behind: Scaling Human-Centered Machine Translation},
    author = {{NLLB Team} and Costa-jussà, Marta R. and Cross, James and Çelebi, Onur and Elbayad, Maha and Heafield, Kenneth and Heffernan, Kevin and Kalbassi, Elahe and Lam, Janice and Licht, Daniel and Maillard, Jean and Sun, Anna and Wang, Skyler and Wenzek, Guillaume and Youngblood, Al and Akula, Bapi and Barrault, Loic and Mejia-Gonzalez, Gabriel and Hansanti, Prangthip and Hoffman, John and Jarrett, Semarley and Sadagopan, Kaushik Ram and Rowe, Dirk and Spruit, Shannon and Tran, Chau and Andrews, Pierre and Ayan, Necip Fazil and Bhosale, Shruti and Edunov, Sergey and Fan, Angela and Gao, Cynthia and Goswami, Vedanuj and Guzmán, Francisco and Koehn, Philipp and Mourachko, Alexandre and Ropers, Christophe and Saleem, Safiyyah and Schwenk, Holger and Wang, Jeff},
    year = {2022},
    eprint = {arXiv:1902.01382},
}
```

Other authors have since contributed to the dataset:
* N’Ko: Moussa Koulako Bala Doumbouya, Baba Mamadi Diané, Solo Farabado Cissé, Djibrila Diané, Abdoulaye Sow, Séré Moussa Doumbouya, Daouda Bangoura, Fodé Moriba Bayo, Ibrahima Sory 2. Condé, Kalo Mory Diané, Chris Piech, Christopher Manning. [Paper](https://arxiv.org/abs/2310.15612), [repository](https://github.com/common-parallel-corpora/common-parallel-corpora).
* Bodo, Dogri, Meitei (Meitei Script), Sindhi (Devanagari script), Goan Konkani: AI4Bharat, Jay Gala, Pranjal A. Chitale, Raghavan AK, Sumanth Doddapaneni, Varun Gumma, Aswanth Kumar, Janki Nawale, Anupama Sujatha, Ratish Puduppully, Vivek Raghavan, Pratyush Kumar, Mitesh M. Khapra, Raj Dabre, Anoop Kunchukuttan. [Paper](https://arxiv.org/abs/2305.16307), [repository](https://github.com/AI4Bharat/IndicTrans2).

If you use this dataset in your work, please cite the papers listed in [bibliography.bib](bibliography.bib).

## Changelog

See [CHANGELOG.md](CHANGELOG.md) for information about the latest changes.
