# Improving Allocentric Spatial Reasoning of VLMs via Perspective-conditional Prompt-based Contrastive Decoding

Code and data for "Improving Allocentric Spatial Reasoning of VLMs via Perspective-conditional Prompt-based Contrastive Decoding" (EMNLP Findings 2026).

**Perspective-Conditional Prompt-based Contrastive Decoding (PCD)**: a training-free method that leverages VLMs' capabilities while exploiting the performance gap between egocentric and allocentric spatial reasoning.


## Datasets

We evaluate on the following benchmarks. Please download each dataset from the links below and place the files under `data/` as described.

**3DSRBench** ([Link](https://huggingface.co/datasets/ccvl/3DSRBench)):
We use the `orientation_on_the_left` and `orientation_in_front_of` types.
Place the files under `data/3dsrbench/`.

**OmniSpatial** ([Link](https://huggingface.co/datasets/qizekun/OmniSpatial)):
We use the `allocentric` subset under the Perspective Taking category.
Place the files under `data/omnispatial/`.

**SpatialMQA** ([Link](https://huggingface.co/datasets/liuziyan/SpatialMQA)):
We use the `test` split.
Place the files under `data/spatialmqa/`.

**ViewSpatial-Bench** ([Link](https://huggingface.co/datasets/lidingm/ViewSpatial-Bench)):
We use the `relative_direction` subset under the Person Perspective category.
Place the files under `data/viewspatial/`.

Note that these benchmarks contain multiple files (e.g., images, annotations). 
Please download all associated files for each benchmark.

After downloading, organize the files as follows:

```
data/
├── 3dsrbench/
├── omnispatial/
├── spatialmqa/
└── viewspatial/
```


## Usage
### Evaluation
```bash
python pcd_qwen25vl.py --model_size 7B 
```

## Citation
