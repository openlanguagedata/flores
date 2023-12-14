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

| Language                           | Code       | Open issues |
|------------------------------------|------------|-------------|
| Acehnese (Arabic script)           | `ace_Arab` |
| Acehnese (Latin script)            | `ace_Latn` |
| Mesopotamian Arabic                | `acm_Arab` |
| Ta’izzi-Adeni Arabic               | `acq_Arab` |
| Tunisian Arabic                    | `aeb_Arab` |
| Afrikaans                          | `afr_Latn` |
| South Levantine Arabic             | `ajp_Arab` |
| Akan                               | `aka_Latn` |
| Tosk Albanian                      | `als_Latn` |
| Amharic                            | `amh_Ethi` |
| North Levantine Arabic             | `apc_Arab` |
| Modern Standard Arabic             | `arb_Arab` |
| Modern Standard Arabic (Romanized) | `arb_Latn` |
| Najdi Arabic                       | `ars_Arab` |
| Moroccan Arabic                    | `ary_Arab` |
| Egyptian Arabic                    | `arz_Arab` |
| Assamese                           | `asm_Beng` |
| Asturian                           | `ast_Latn` |
| Awadhi                             | `awa_Deva` |
| Central Aymara                     | `ayr_Latn` |
| South Azerbaijani                  | `azb_Arab` |
| North Azerbaijani                  | `azj_Latn` |
| Bashkir                            | `bak_Cyrl` |
| Bambara                            | `bam_Latn` |
| Balinese                           | `ban_Latn` |
| Belarusian                         | `bel_Cyrl` |
| Bemba                              | `bem_Latn` |
| Bengali                            | `ben_Beng` |
| Bhojpuri                           | `bho_Deva` |
| Banjar (Arabic script)             | `bjn_Arab` |
| Banjar (Latin script)              | `bjn_Latn` |
| Standard Tibetan                   | `bod_Tibt` |
| Bosnian                            | `bos_Latn` |
| Bodo                               | `brx_Deva` | `dev` only |
| Buginese                           | `bug_Latn` |
| Bulgarian                          | `bul_Cyrl` |
| Catalan                            | `cat_Latn` |
| Cebuano                            | `ceb_Latn` |
| Czech                              | `ces_Latn` |
| Chokwe                             | `cjk_Latn` |
| Central Kurdish                    | `ckb_Arab` | [facebookresearch/flores#50](https://github.com/facebookresearch/flores/issues/50) |
| Mandarin Chinese (Simplified)      | `cmn_Hans` |
| Mandarin Chinese (Traditional)     | `cmn_Hant` |
| Crimean Tatar                      | `crh_Latn` |
| Welsh                              | `cym_Latn` |
| Danish                             | `dan_Latn` |
| German                             | `deu_Latn` |
| Dogri                              | `dgo_Deva` | `dev` only |
| Southwestern Dinka                 | `dik_Latn` |
| Dyula                              | `dyu_Latn` |
| Dzongkha                           | `dzo_Tibt` |
| Greek                              | `ell_Grek` |
| English                            | `eng_Latn` |
| Esperanto                          | `epo_Latn` |
| Estonian                           | `est_Latn` |
| Basque                             | `eus_Latn` |
| Ewe                                | `ewe_Latn` |
| Faroese                            | `fao_Latn` |
| Fijian                             | `fij_Latn` |
| Finnish                            | `fin_Latn` |
| Fon                                | `fon_Latn` |
| French                             | `fra_Latn` |
| Friulian                           | `fur_Latn` |
| Nigerian Fulfulde                  | `fuv_Latn` |
| Scottish Gaelic                    | `gla_Latn` |
| Irish                              | `gle_Latn` |
| Galician                           | `glg_Latn` |
| Goan Konkani                       | `gom_Deva` |
| Guarani                            | `grn_Latn` |
| Gujarati                           | `guj_Gujr` |
| Haitian Creole                     | `hat_Latn` |
| Hausa                              | `hau_Latn` |
| Hebrew                             | `heb_Hebr` |
| Hindi                              | `hin_Deva` |
| Chhattisgarhi                      | `hne_Deva` |
| Croatian                           | `hrv_Latn` |
| Hungarian                          | `hun_Latn` |
| Armenian                           | `hye_Armn` |
| Igbo                               | `ibo_Latn` |
| Ilocano                            | `ilo_Latn` |
| Indonesian                         | `ind_Latn` |
| Icelandic                          | `isl_Latn` |
| Italian                            | `ita_Latn` |
| Javanese                           | `jav_Latn` |
| Japanese                           | `jpn_Jpan` |
| Kabyle                             | `kab_Latn` |
| Jingpho                            | `kac_Latn` |
| Kamba                              | `kam_Latn` |
| Kannada                            | `kan_Knda` |
| Kashmiri (Arabic script)           | `kas_Arab` |
| Kashmiri (Devanagari script)       | `kas_Deva` |
| Georgian                           | `kat_Geor` |
| Central Kanuri (Arabic script)     | `knc_Arab` |
| Central Kanuri (Latin script)      | `knc_Latn` |
| Kazakh                             | `kaz_Cyrl` |
| Kabiyè                             | `kbp_Latn` |
| Kabuverdianu                       | `kea_Latn` |
| Khmer                              | `khm_Khmr` |
| Kikuyu                             | `kik_Latn` |
| Kinyarwanda                        | `kin_Latn` |
| Kyrgyz                             | `kir_Cyrl` |
| Kimbundu                           | `kmb_Latn` |
| Northern Kurdish                   | `kmr_Latn` |
| Kikongo                            | `kon_Latn` |
| Korean                             | `kor_Hang` |
| Lao                                | `lao_Laoo` |
| Ligurian                           | `lij_Latn` |
| Filipino                           | `fil_Latn` |
| Limburgish                         | `lim_Latn` |
| Lingala                            | `lin_Latn` |
| Lithuanian                         | `lit_Latn` |
| Lombard                            | `lmo_Latn` |
| Latgalian                          | `ltg_Latn` |
| Luxembourgish                      | `ltz_Latn` |
| Luba-Kasai                         | `lua_Latn` |
| Ganda                              | `lug_Latn` |
| Luo                                | `luo_Latn` |
| Mizo                               | `lus_Latn` |
| Standard Latvian                   | `lvs_Latn` |
| Magahi                             | `mag_Deva` |
| Maithili                           | `mai_Deva` |
| Malayalam                          | `mal_Mlym` |
| Marathi                            | `mar_Deva` |
| Minangkabau (Arabic script)        | `min_Arab` |
| Minangkabau (Latin script)         | `min_Latn` |
| Macedonian                         | `mkd_Cyrl` |
| Plateau Malagasy                   | `plt_Latn` |
| Maltese                            | `mlt_Latn` |
| Meitei (Bengali script)            | `mni_Beng` |
| Meitei (Meitei script)             | `mni_Mtei` | `dev` only |
| Halh Mongolian                     | `khk_Cyrl` |
| Mossi                              | `mos_Latn` |
| Maori                              | `mri_Latn` |
| Burmese                            | `mya_Mymr` |
| Dutch                              | `nld_Latn` |
| Norwegian Nynorsk                  | `nno_Latn` |
| Norwegian Bokmål                   | `nob_Latn` |
| Nepali                             | `npi_Deva` |
| Nko                                | `nqo_Nkoo` |
| Northern Sotho                     | `nso_Latn` |
| Nuer                               | `nus_Latn` |
| Nyanja                             | `nya_Latn` |
| Occitan                            | `oci_Latn` |
| West Central Oromo                 | `gaz_Latn` |
| Odia                               | `ory_Orya` |
| Pangasinan                         | `pag_Latn` |
| Eastern Panjabi                    | `pan_Guru` |
| Papiamento                         | `pap_Latn` |
| Western Persian                    | `pes_Arab` |
| Polish                             | `pol_Latn` |
| Portuguese                         | `por_Latn` |
| Dari                               | `prs_Arab` |
| Southern Pashto                    | `pbt_Arab` |
| Ayacucho Quechua                   | `quy_Latn` |
| Romanian                           | `ron_Latn` |
| Rundi                              | `run_Latn` |
| Russian                            | `rus_Cyrl` |
| Sango                              | `sag_Latn` |
| Sanskrit                           | `san_Deva` |
| Santali                            | `sat_Olck` |
| Sicilian                           | `scn_Latn` |
| Shan                               | `shn_Mymr` |
| Sinhala                            | `sin_Sinh` |
| Slovak                             | `slk_Latn` |
| Slovenian                          | `slv_Latn` |
| Samoan                             | `smo_Latn` |
| Shona                              | `sna_Latn` |
| Sindhi (Arabic script)             | `snd_Arab` |
| Sindhi (Devanagari script)         | `snd_Deva` | `dev` only |
| Somali                             | `som_Latn` |
| Southern Sotho                     | `sot_Latn` |
| Spanish                            | `spa_Latn` |
| Sardinian                          | `srd_Latn` |
| Serbian                            | `srp_Cyrl` |
| Swati                              | `ssw_Latn` |
| Sundanese                          | `sun_Latn` |
| Swedish                            | `swe_Latn` |
| Swahili                            | `swh_Latn` |
| Silesian                           | `szl_Latn` |
| Tamil                              | `tam_Taml` |
| Tatar                              | `tat_Cyrl` |
| Telugu                             | `tel_Telu` |
| Tajik                              | `tgk_Cyrl` |
| Thai                               | `tha_Thai` |
| Tigrinya                           | `tir_Ethi` |
| Tamasheq (Latin script)            | `taq_Latn` |
| Tamasheq (Tifinagh script)         | `taq_Tfng` |
| Tok Pisin                          | `tpi_Latn` |
| Tswana                             | `tsn_Latn` |
| Tsonga                             | `tso_Latn` |
| Turkmen                            | `tuk_Latn` |
| Tumbuka                            | `tum_Latn` |
| Turkish                            | `tur_Latn` |
| Twi                                | `twi_Latn` |
| Uyghur                             | `uig_Arab` |
| Ukrainian                          | `ukr_Cyrl` |
| Umbundu                            | `umb_Latn` |
| Urdu                               | `urd_Arab` |
| Northern Uzbek                     | `uzn_Latn` |
| Venetian                           | `vec_Latn` |
| Vietnamese                         | `vie_Latn` |
| Waray                              | `war_Latn` |
| Wolof                              | `wol_Latn` |
| Xhosa                              | `xho_Latn` |
| Eastern Yiddish                    | `ydd_Hebr` |
| Yoruba                             | `yor_Latn` |
| Yue Chinese                        | `yue_Hant` | [facebookresearch/flores#61](https://github.com/facebookresearch/flores/issues/61) |
| Standard Moroccan Tamazight        | `zgh_Tfng` |
| Standard Malay                     | `zsm_Latn` |
| Zulu                               | `zul_Latn` |

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