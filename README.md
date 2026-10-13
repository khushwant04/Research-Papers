# AI & ML Research Papers Dataset

A collection of 1,296 AI and machine learning research papers in PDF form, published on Hugging Face. This repository holds only the dataset card. The PDFs are hosted at [huggingface.co/datasets/khushwant04/Research-Papers](https://huggingface.co/datasets/khushwant04/Research-Papers).

## Summary

| | |
| --- | --- |
| Papers | 1,296 |
| Format | PDF files, packed in a single `research-papers.tar` archive |
| Topics | Machine learning, deep learning, NLP, computer vision, reinforcement learning and related AI areas |
| Hosted on | Hugging Face Datasets |

## Download

```bash
curl -L -o research-papers.tar \
  "https://huggingface.co/datasets/khushwant04/Research-Papers/resolve/main/research-papers.tar?download=true"
tar -xf research-papers.tar
```

Or from Python:

```python
from huggingface_hub import hf_hub_download

path = hf_hub_download(
    repo_id="khushwant04/Research-Papers",
    filename="research-papers.tar",
    repo_type="dataset",
)
```

## Possible uses

- Building a retrieval / RAG corpus over ML literature
- Topic modelling and trend analysis
- Summarisation and text-classification experiments
- Paper recommendation

Only the PDFs are included. Metadata such as authors, venues or citation counts is not, so you have to extract it yourself, for example with a PDF parser such as GROBID.

## License and terms

The papers are the work of their original authors and keep their original licenses. Check each paper's terms before redistributing it. The [LICENSE](LICENSE) file in this repository (MIT) covers the repository contents, i.e. this card.

## Related

- [Paper-Scraper](https://github.com/khushwant04/Paper-Scraper): a Scrapy spider that downloads paper PDFs grouped by task.

## Citation

```bibtex
@misc{sanwalot2024researchpapers,
  title        = {AI \& Machine Learning Research Papers Dataset},
  author       = {Sanwalot, Khushwant},
  year         = {2024},
  publisher    = {Hugging Face},
  howpublished = {\url{https://huggingface.co/datasets/khushwant04/Research-Papers}}
}
```
