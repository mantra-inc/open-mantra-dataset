# OpenMantra dataset
Dataset introduced in the paper "Towards Fully Automated Manga Translation" presented in AAAI21 ([arXiv link](https://arxiv.org/abs/2012.14271))

by Ryota Hinami, Shonosuke Ishiwatari, Kazuhiko Yasuda, Yusuke Matsui


## Introduction
OpenMantra dataset is an evaluation dataset for machine translation of manga.
The dataset comprised of five Japanese manga series across different genres, including fantasy, romance, battle, mystery, and slice of life.
Original Japanese texts are translated into English and Chinese by professional translators.


## Data
This repository includes annotated JSON files and the original images.

- images/ : Directory that includes the images of OpenMantra dataset
- annotations.json: Annotation of OpenMantra dataset
```
[
  {
    "book_title": "tojime_no_siora", # Book title
    "pages": [ # Pages of each book
      {
        "page_index": 1, # Page number
        "image_paths": { # Image paths
          "ja": "images/tojime_no_siora/ja/000.jpg",
        },
        "text": [ # Annotation of speech bubbles that include bounding box, Japanese texts, and translated texts
          {
            "x": 82,
            "y": 952,
            "w": 668,
            "h": 107,
            "text_ja": "綴じ眼のシオラ",
            "text_en": "bound eye siora",
            "text_zh": "縫眼的希奧拉"
          },
          ...
```


## Citation
When you use OpenMantra dataset, please cite the following paper:

```
@article{hinami_aaai_2021,
    author={Ryota Hinami and Shonosuke Ishiwatari and Kazuhiko Yasuda and Yusuke Matsui},
    title={Towards Fully Automated Manga Translation},
    booktitle={Proceedings of the AAAI Conference on Artificial Intelligence},
    year={2021}
}
```

## Contact
For any question, please fill an issue or use the contact form of our company. 
[Contact](https://docs.google.com/forms/d/e/1FAIpQLScn2JHjJOgBrpiT3Lo0mOZO9-kHxwJmCRRnf8eW7K0HjDhrgg/viewform)


