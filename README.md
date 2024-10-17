# README


This repository provides pre-trained n-gram language models for Chinese text, including 3-grams, 4-grams, and 5-grams. These models can be integrated into applications such as Optical Character Recognition (OCR) systems, especially for handwritten Chinese character recognition (HCTR).

## Introduction

Available models:

1. 3-grams
2. 4-grams
3. 5-grams

Each model is available in ARPA and binary formats for integration.

## 3-grams Model

### Download instruction

To download the 3-grams ARPA model:

```
mkdir 3-grams-arpa-temp
gh release download m3-grams-arpa -D 3-grams-arpa-temp -R pratamov/ZH-TW_LM
cat 3-grams-arpa-temp/* | gunzip > 3-grams.arpa
rm -rf 3-grams-arpa-temp
```


To download the 3-grams binary model:

```
mkdir 3-grams-bin-temp
gh release download m3-grams-bin -D 3-grams-bin-temp -R pratamov/ZH-TW_LM
cat 3-grams-bin-temp/* | gunzip > 3-grams.bin
rm -rf 3-grams-bin-temp
```

### How to Use

Suppose already provided a visual OCR model of [HCTR](https://github.com/intel/handwritten-chinese-ocr-samples/tree/main), integrate the model with the following parameter:

```
-dm beam-search --skip-search --kenlm-path 3-grams.arpa
```

## 4-grams Model

### Download instruction

To download the 4-grams ARPA model:

```
mkdir 4-grams-arpa-temp
gh release download m4-grams-arpa -D 4-grams-arpa-temp -R pratamov/ZH-TW_LM
cat 4-grams-arpa-temp/* | gunzip > 4-grams.arpa
rm -rf 4-grams-arpa-temp
```


To download the 4-grams binary model:

```
mkdir 4-grams-bin-temp
gh release download m4-grams-bin -D 4-grams-bin-temp -R pratamov/ZH-TW_LM
cat 4-grams-bin-temp/* | gunzip > 4-grams.bin
rm -rf 4-grams-bin-temp
```

### How to Use

Suppose already provided a visual OCR model of [HCTR](https://github.com/intel/handwritten-chinese-ocr-samples/tree/main), integrate the model with the following parameter:

```
-dm beam-search --skip-search --kenlm-path 4-grams.arpa
```


## 5-grams Model

### Download instruction

To download the 5-grams ARPA model:

```
mkdir 5-grams-arpa-temp
gh release download m5-grams-arpa -D 5-grams-arpa-temp -R pratamov/ZH-TW_LM
cat 5-grams-arpa-temp/* | gunzip > 5-grams.arpa
rm -rf 5-grams-arpa-temp
```


To download the 3-grams binary model:

```
mkdir 5-grams-bin-temp
gh release download m5-grams-bin -D 5-grams-bin-temp -R pratamov/ZH-TW_LM
cat 5-grams-bin-temp/* | gunzip > 5-grams.bin
rm -rf 5-grams-bin-temp
```

### How to Use

Suppose already provided a visual OCR model of [HCTR](https://github.com/intel/handwritten-chinese-ocr-samples/tree/main), integrate the model with the following parameter:

```
-dm beam-search --skip-search --kenlm-path 5-grams.arpa
```

