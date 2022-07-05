# SAS → CSV
> Convert [`.sas7bdat`](https://documentation.sas.com/doc/en/pgmsascdc/9.4_3.5/hostwin/n0sk6o15955yoen19n9ghdziqw1u.htm#n19rscz36w9ly5n1c6bhrh8o348x) to [`.csv`](https://en.wikipedia.org/wiki/Comma-separated_values) in Google Drive using Google Colab R kernel

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/woncoh1/sas2csv/blob/main/sas2csv.ipynb)

## Intro
- This notebook uses Colab's R kernel to convert `.sas7bdat` files into `.csv` files
- All `.sas7bdat` and `.csv` files are stored in Google Drive
- The `.sas7bdat` files can be moved to trash or left intact

## Character encoding
- `.sas7bdat`
    - [cp949](https://en.wikipedia.org/wiki/Unified_Hangul_Code) (default)
    - [euc-kr](https://en.wikipedia.org/wiki/Extended_Unix_Code#EUC-KR)
    - [utf-8](https://en.wikipedia.org/wiki/UTF-8)
    - [latin1](https://en.wikipedia.org/wiki/ISO/IEC_8859-1)
- `.csv`: [utf-8](https://en.wikipedia.org/wiki/UTF-8) (default)

## File permission
- Upload `.csv`: **editor** of the **main folder**
- Trash `.sas7bdat`: **owner** of the **main folder**

## Folder structure
- **Main Folder**
    - Subfolder 1
        - `.sas7bdat` 1
        - `.sas7bdat` 2
        - ...
        - `.sas7bdat` n
    - Subfolder 2
        - `.sas7bdat` 1
        - `.sas7bdat` 2
        - ...
        - `.sas7bdat` n
    - ...
    - Subfolder n
        - `.sas7bdat` 1
        - `.sas7bdat` 2
        - ...
        - `.sas7bdat` n

## TODO
- [ ] Add more character encodings
- [ ] Expand to `.sav` (SPSS) and `.dta` (Stata) files
- [ ] Improve time complexity using concurrency, parallelism or distributed computing
