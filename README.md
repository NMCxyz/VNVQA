# VQA

## 📑 Table of Contents
1. [Prerequisites](#Prerequisites)
2. [Dataset](#Dataset)
3. [Data Transformation](#Data-Transformation)
4. [Training and Validation](#Training-and-Validation)
5. [Testing](#Testing)
6. [Pretrained Models](#Pretrained-models)
7. [Recommendations](#Recommendations)

## 🛠️ Prerequisites

### Requirements

You should first install some necessary packages.

```bash
    pip install -r requirements.txt
```

## 📊 Dataset
- The dataset used is OpenViVQA.

You can also obtain the dataset from Hugging Face:

```bash
from datasets import load_dataset
dataset = load_dataset("uitnlp/OpenViVQA-dataset")
```

## 🔄 Data Transformation
Run the data_transform.ipynb notebook to transform and preprocess the training, validation, and test sets:

## 🏋️ Training and Validation
The following script will start training with the default hyperparameters in mcan.yaml:

```bash
python3 main.py --config mcan.yaml
```
## 🧪 Testing
To test the model, modify the configuration to use the test dataset. Update mcan.yaml with the test img.
Then run the following command:

``` bash
python3 main.py --config mcan.yaml
```
## 📦 Pretrained Models
I use two pretrained models, ViT (Vision Transformer) and PhoBERT.

##💡 Recommendations
I recommend using Google Colab for running this project, as it provides free access to GPU resources, making it easier to clone the repository and run experiments.


## 📚 References

- MCAN Paper: [Deep Modular Co-Attention Networks for Visual Question Answering](https://openaccess.thecvf.com/content_CVPR_2019/html/Yu_Deep_Modular_Co-Attention_Networks_for_Visual_Question_Answering_CVPR_2019_paper.html)
- Original MCAN Implementation: [GitHub Repository](https://github.com/MILVLG/mcan-vqa)
- OpenViVQA Paper: [Open-source Vietnamese Visual Question Answering](https://aclanthology.org/2021.paclic-1.72/)
