
# PromptCL: Improving Event Representation via Prompt and Contrastive Learning

We are pleased to release the official implementation of our paper titled "PromptCL: Improving Event Representation via Prompt and Contrastive Learning," which was published at NLPCC 2023! 🎉🎉🎉

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
  title={PromptCL: Improving Event Representation via Prompt and Contrastive Learning},
  author={Feng, Yubo and Li, Lishuang and Xiang, Yi and Qin, Xueyang},
  booktitle={CCF International Conference on Natural Language Processing and Chinese Computing},
  year={2023},
  organization={Springer}
}
```
