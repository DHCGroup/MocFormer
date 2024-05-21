# MocFormer: A Two-Stage Pre-training-Driven Transformer for Drug-Target Interactions Prediction

The official repository of the paper [MocFormer: A Two-Stage Pre-training-Driven Transformer for Drug-Target Interactions Prediction](https://www.biorxiv.org/content/10.1101/2023.09.13.557595v3)

![image](https://github.com/rickwang28574/MocFormer/assets/87885188/f152b543-1c42-4616-82ac-e9489a53cf66)

A novel two-stage pre-trained framework (Mocformer) is proposed for drug-target interactions prediction. In the first stage, pre-trained molecule and protein models develop a comprehensive feature representation, enhancing the framework's ability to handle drug and protein diversity. This also reduces bias, improving prediction accuracy. In the second stage, a transformer with bilinear pooling and a fully connected layer enables predictions based on feature vectors.

### Installation

```bash
git clone https://github.com/rickwang28574/MocFormer.git
cd MocFormer
```
#### Install dependency

```bash
conda create -n MocFormer python==3.8.1
conda activate MocFormer
pip install -r requirements.txt
```

#### Processed Datasets
The two datasets provided below are results obtained by processing and fine-tuning small molecules and proteins using Unimol and ESM-2, respectively. The composition of the datasets includes: SMILES representations for small molecules, amino acid sequences for proteins, embeddings for small molecules, embeddings for proteins, and labels.

For DrugBank dataset

```bash
https://drive.google.com/file/d/1PsFQusALcyp2NkjFs5xw-CHhSqZpzSVr/view?usp=sharing
```

For Epigenetic-regulators dataset

```bash
Train: https://drive.google.com/file/d/1_aJX3UBZMDsi32EZz25BAW3KRvdQHsy9/view?usp=sharing
Test: https://drive.google.com/file/d/1k-Y6fBAY8U8IukxaO9Dhh4ESzYRLtIGz/view?usp=sharing
```

#### Train & Test
Please run the billnear_DrugBank_uni_esm2_3B_trans copy.ipynb notebook sequentially, and you will obtain results in the "Test" section of the file. In this Jupyter notebook, we have provided model training and testing code using the DrugBank dataset as an example. The model for the Epigenetic-regulators dataset will be very similar.

## Citation
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>@article{Zhang2023.09.13.557595,
  title={MocFormer: A Two-Stage Pre-training-Driven Transformer for Drug-Target Interactions Prediction},
  author={Yi-Lun Zhang and Wen-Tao Wang and Jia-Hui Guan and Deepak Kumar Jain and Tian-Yang Wang and Swalpa Kumar Roy},
  journal={bioRxiv},
  year={2023}
}
</code></pre><div class="zeroclipboard-container position-absolute right-0 top-0">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn js-clipboard-copy m-2 p-0 tooltipped-no-delay" data-copy-feedback="Copied!" data-tooltip-direction="w" value="@article{Zhang2023.09.13.557595,
  title={MocFormer: A Two-Stage Pre-training-Driven Transformer for Drug-Target Interactions Prediction},
  author={Yi-Lun Zhang and Wen-Tao Wang and Jia-Hui Guan and Deepak Kumar Jain and Tian-Yang Wang and Swalpa Kumar Roy},
  journal={bioRxiv},
  year={2023}
}" tabindex="0" role="button" style="display: inherit;">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon m-2">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none m-2">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>

