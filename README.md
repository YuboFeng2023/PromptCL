
# PromptCL: Improving Event Representation via Prompt and Contrastive Learning

We are pleased to release the official implementation of our paper titled "PromptCL: Improving Event Representation via Prompt and Contrastive Learning", which was published at NLPCC 2023 and awarded **Best Student Paper**! 🎉🎉🎉"

## Dataset

Please refer to [SWCC](https://github.com/gaojun4ever/SWCC4Event)

## Quick Start

```bash
conda create -n promptcl python=3.8
conda activate promptcl
pip install -r requirements.txt
```

## Training/Testing

we run the code on Nvidia A100 80GB.

### Train

```bash
python3 main.py --do-train
```
 
### Test

Hard Similarity Task and Transitive Task:

```bash
python3 main.py --do-eval --checkpoint ./models/checkpoint.pt
```
 
MCNC Task:

```bash
python3 mcnc.py --do-eval --checkpoint ./models/checkpoint.pt
```


## Acknowledgement

The code is developed based on [SWCC](https://github.com/imgaojun/SWCC4Event). 
We appreciate all the authors who made their code public, which greatly facilitates this project. 


## Citation

```latex
@inproceedings{feng2023promptcl,
  author       = {Yubo Feng and
                  Lishuang Li and
                  Yi Xiang and
                  Xueyang Qin},
  editor       = {Fei Liu and
                  Nan Duan and
                  Qingting Xu and
                  Yu Hong},
  title        = {PromptCL: Improving Event Representation via Prompt Template and Contrastive
                  Learning},
  booktitle    = {Natural Language Processing and Chinese Computing - 12th National
                  {CCF} Conference, {NLPCC} 2023, Foshan, China, October 12-15, 2023,
                  Proceedings, Part {I}},
  series       = {Lecture Notes in Computer Science},
  volume       = {14302},
  pages        = {261--272},
  publisher    = {Springer},
  year         = {2023},
  url          = {https://doi.org/10.1007/978-3-031-44693-1\_21},
  doi          = {10.1007/978-3-031-44693-1\_21},
  timestamp    = {Wed, 11 Oct 2023 18:49:11 +0200},
  biburl       = {https://dblp.org/rec/conf/nlpcc/FengLXQ23.bib},
  bibsource    = {dblp computer science bibliography, https://dblp.org}
}
```
