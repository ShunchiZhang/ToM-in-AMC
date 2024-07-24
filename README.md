# Few-Shot Character Understanding in Movies as an Assessment to Meta-Learning of Theory-of-Mind

<p align="center">
    <a href="https://proceedings.mlr.press/v235/yu24n.html">Paper</a> |
    <a href="https://shunchizhang.github.io/tom-in-amc">Project Page</a> |
    <a href="https://icml.cc/virtual/2024/poster/33732">ICML Poster</a>
</p>

## :film_strip: Dataset: ToM-in-AMC

Please download the data from [Google Drive](https://drive.google.com/drive/folders/1y9_zP4zOaP_WPntYQuXJXOdtv72POGg_?usp=sharing).

```sh
gdown --folder 1y9_zP4zOaP_WPntYQuXJXOdtv72POGg_ -O data
# SHA256: 551a726269cf9d6149d32b7712230111ddd4f43ac8ea461edd9456c8527711ad
```

and run [`dataset_overview.ipynb`](/dataset_overview.ipynb) for details.

The dataset consists of ∼1,000 parsed movie scripts from [IMSDb](https://imsdb.com), each corresponding to a few-shot character understanding task.

## :robot: Models

Our dataset evaluate the machines’ ToM in two settings:
- **Transductive setting**: meta-model predicts with all characters’ previous acts as examples
- **Inductive setting**: meta-model predicts with a mental model of characters generated by all characters’ previous acts

  > :bulb: This setting is more stringent and has advantages in emphasizing the effects of various ToM dimensions, improving explanability and mitigating shortcuts.

### Inductive Setting: ToMPro

[To Be Cleaned] See [`/tompro`](/tompro).

### Transductive Setting: In-Context Learning

[To Be Cleaned] See [`/icl`](/icl).

## :pencil: Citation

```bibtex
@inproceedings{yu2024few,
  title = {Few-Shot Character Understanding in Movies as an Assessment to Meta-Learning of Theory-of-Mind},
  author = {Yu, Mo and Wang, Qiujing and Zhang, Shunchi and Sang, Yisi and Pu, Kangsheng and Wei, Zekai and Wang, Han and Xu, Liyan and Li, Jing and Yu, Yue and Zhou, Jie},
  booktitle = {Proceedings of the 41st International Conference on Machine Learning},
  year = {2024}
}
```
