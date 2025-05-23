# Generating_Video_Data

```
Hanzhe Liang
modified: 23 May
```

😊 This library contains some common data for training video generation models. Regardless of which data you need, the following steps:
```bash
mkdir data
cd data
```
Next, go to my cloud database [link](https://huggingface.co/datasets/HanzheL/Generating_Video_Data/blob/main/README.md) and download the data you want into the folder```data/```.
Once you've downloaded the data you need, we've found preprocessing steps from its official implementation, which you can follow to process the data.
For memory requirements, we provide the files as single zip files, you need to extract the file named data_name.rar with the unzip command: ```unrar x data_name.rar```

----

### Something Something V2
Please check the data path.
```bash
cd somethingv2
python extract_frames.py
python process_somethingv2.py
```
You can check data list ```somethingv2/*.txt```. You need cite:
```bibtex
@inproceedings{goyal2017something,
  title={The" something something" video database for learning and evaluating visual common sense},
  author={Goyal, Raghav and Ebrahimi Kahou, Samira and Michalski, Vincent and Materzynska, Joanna and Westphal, Susanne and Kim, Heuna and Haenel, Valentin and Fruend, Ingo and Yianilos, Peter and Mueller-Freitag, Moritz and others},
  booktitle={Proceedings of the IEEE international conference on computer vision},
  pages={5842--5850},
  year={2017}
}
```

### Human3.6M
I provided processed datasets.

```bash
cd human36m
python build_clip_dataset.py
python make_list.py
```
You can check data list ```human36m/*.txt```. You need cite:
```bibtex
@article{h36m_pami,
 author = {Ionescu, Catalin and Papava, Dragos and Olaru, Vlad and Sminchisescu, Cristian},
 title = {Human3.6M: Large Scale Datasets and Predictive Methods for 3D Human Sensing in Natural Environments},
 journal = {IEEE Transactions on Pattern Analysis and Machine Intelligence},
 publisher = {IEEE Computer Society},
 year = {2014}
} 
```

### YouTubeDriving
```bash
cd youtubedriving
python make_list.py
```
You can check data list ```youtubedriving/*.txt```. You need cite:
```bibtex
@article{zhang2022learning,
  title={Learning to Drive by Watching YouTube videos: Action-Conditioned Contrastive Policy Pretraining},
  author={Zhang, Qihang and Peng, Zhenghao and Zhou, Bolei},
  journal={European Conference on Computer Vision (ECCV)},
  year={2022}
}
```
