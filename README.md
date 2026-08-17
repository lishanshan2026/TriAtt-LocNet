# TriAtt-LocNet

TriAtt-LocNet is a remote sensing image change detection model based on a LocNet backbone with Triplet Attention.

## Requirements

```bash
pip install -r requirements.txt
```

## Dataset

Set the dataset path in `metadata.json`:

```json
{
  "dataset_dir": "../CDD/Real/subset/"
}
```

The expected dataset structure follows the CDD change detection format used by the dataloader.

## Training

```bash
python train.py
```

## Evaluation and visualization

After training, place the generated model weights under `weights/`, then run:

```bash
python eval.py
python visualization.py
```

## Notes

This repository only contains source code. Pretrained weights, checkpoints, logs, temporary files, and experiment records are not included.
