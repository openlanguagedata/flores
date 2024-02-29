# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

In particular:

1. Any updates to pre-existing files shall entail a major version bump.
2. The inclusion of a new language, without changes to other pre-existing data, shall only entail a minor version bump.

It follows from the above that benchmark scores across different releases of FLORES+ with the same major version number are comparable.


## [2.0-rc.1] – 2024-02-29

### Added

- Added `nqo_Nkoo` from <https://github.com/common-parallel-corpora/common-parallel-corpora>.
- Added the `dev` splits for `brx_Deva`, `dgo_Deva`, `mni_Mtei`, `snd_Deva`, `gom_Deva` from <https://github.com/ai4bharat/IndicTrans2>.
- Added the `dev` split for `mhr_Cyrl`. Many thanks to Andrey Chemyshev @fu-lab.
- Added the `dev` split for `chv_Cyrl`. Many thanks to @AlAntonov.

### Changed

- Relabeled `zho_Hans` to `cmn_Hans` after confirming the data is in Standard Beijing Mandarin.
- Relabeled `zho_Hant` to `cmn_Hant` after confirming the data is in Taiwanese Mandarin.
- Relabeled `tgl_Latn` to `fil_Latn` after confirming the data is in Filipino.
- Relabeled `tzm_Tfng` to `zgh_Tfng` after additional quality assessment revealed the data was in Standard Moroccan Tamazight. Many thanks to @MedAymenF for pointing out the issues with the original FLORES-200 data.
- Updated `lij_Latn` after additional quality assessment. Data has undergone minor spelling and syntactic fixes.
- Updated `ckb_Arab` to replace usage of the non-standard `ك` character and improve the translation quality. Many thanks to @Sarchia for pointing out the issues with the original FLORES-200 data.
- Updated `yue_Hant` to better conform to Honk Kong Cantonese. Thanks to the users who reported issues in [facebookresearch/flores#61](https://github.com/facebookresearch/flores/issues/61).
- Updated several datasets due to a small number of translations (typically 1-2 sentences per dataset) having been overwritten by other sentences. The issue was reported in [facebookresearch/flores#62](https://github.com/facebookresearch/flores/issues/62) and [facebookresearch/flores#67](https://github.com/facebookresearch/flores/issues/67) – many thanks to @sotwi and @kargaranamir! Affected dev sets: `ary_Arab`, `azb_Arab`, `ban_Latn`, `bod_Tibt`, `bos_Latn`, `bug_Latn`, `crh_Latn`, `dik_Latn`, `dyu_Latn`, `dzo_Tibt`, `fao_Latn`, `hat_Latn`, `jav_Latn`, `kam_Latn`, `kas_Deva`, `kaz_Cyrl`, `kbp_Latn`, `lim_Latn`, `lin_Latn`, `lit_Latn`, `lus_Latn`, `npi_Deva`, `run_Latn`, `san_Deva`, `sat_Olck`, `spa_Latn`, `ssw_Latn`, `sun_Latn`, `szl_Latn`, `taq_Tfng`, `urd_Arab`, `ydd_Hebr`. Affected devtest sets: `ary_Arab`, `bam_Latn`, `bod_Tibt`, `dyu_Latn`, `gla_Latn`, `grn_Latn`, `hat_Latn`, `hne_Deva`, `kam_Latn`, `kaz_Cyrl`, `kik_Latn`, `lin_Latn`, `lit_Latn`, `lua_Latn`, `min_Arab`, `min_Latn`, `npi_Deva`, `run_Latn`, `san_Deva`, `smo_Latn`, `spa_Latn`, `szl_Latn`, `taq_Tfng`, `tgk_Cyrl`, `uig_Arab`, `urd_Arab`, `ydd_Hebr`.

## 1.0 - 2023-10-24

Initial release. This is the exact same data that was released under the name `FLORES-200` by [NLLB Team et al. (2022)](https://arxiv.org/abs/2207.04672). It can be downloaded from <https://tinyurl.com/flores200dataset>.