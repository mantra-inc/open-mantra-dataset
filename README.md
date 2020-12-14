# OpenMantra dataset
OpenMantra dataset is a evaluation dataset for machine translation of manga.
The dataset comprised of five Japanese manga series across different genres, including fantasy, romance, battle, mystery, and slice of life.
Original Japanese texts are translated into English and Chinese by professional translator.

This repository includes annotation json files and original images.

- images/ : Directory that includes the images of Mantra5 dataset
- annotations.json: Annotation of Mantra5 dataset
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


