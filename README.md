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
You can check data list ```somethingv2/*.txt```

### Human3.6M
I provided two datasets, both processed and unprocessed.

Unprocessed
```bash
cd human36m/human36m_unprocessed
python build_clip_dataset.py
python make_list.py
```
You can check data list ```human36m/human36m_unprocessed/*.txt```

or you can directly check the processed data in ```human36m/human36m_processed```

### YouTubeDriving
```bash
cd youtubedriving
python make_list.py
```
You can check data list ```youtubedriving/*.txt```
