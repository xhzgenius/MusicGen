# MusicGen

 2025春季深度生成模型小组作业

## Usage

##### 安装所需的包

最好安装 jupyter notebook，vscode 有支持插件

```bash
pip install --upgrade transformers scipy
pip install transformers[torch]
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu128
pip install librosa
pip install --upgrade datasets
pip install peft
```

##### 运行推理（生成音乐）

直接进入 `inference.ipynb` 运行。已跑通。效果还挺不错。修改max_new_tokens可以修改生成长度。

##### 运行微调

MusicCap数据集需要下载并处理。找到了下载和处理的脚本 `download_musiccaps.ipynb` ，但是没跑通，疑似需要youtube cookie，暂时懒得搞。暂时没搞定。

找到了 MusicBench (https://huggingface.co/datasets/amaai-lab/MusicBench/tree/main) 数据集。需要下载里面的压缩文件，解压并放在 `/data` 目录。

微调代码已备，跑一遍要先读数据集（十几分钟）所以有点慢。
