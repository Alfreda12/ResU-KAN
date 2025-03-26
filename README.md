# ResU-KAN

### Training ResU-KAN

You can simply train ResU-KAN on a single GPU by specifing the dataset name ```--dataset``` and input size ```--input_size```.

```bash
python train.py --arch ResUKAN --dataset ${dataset} --input_w ${input_size} --input_h ${input_size} --name ${dataset}_ResUKAN  --data_dir [YOUR_DATA_DIR]
```

For example, train ResU-KAN with the resolution of 256x256 with a single GPU on the BUSI dataset in the ```inputs``` dir:

```bash
python train.py --arch ResUKAN --dataset busi --input_w 256 --input_h 256 --name busi_ResUKAN  --data_dir ./inputs
```

### Evaluating ResU-KAN

You can evaluate ResU-KAN using the following code

```bash
python val.py --name ${dataset}_ResUKAN --output_dir [YOUR_OUTPUT_DIR] 
```

For example

```bash
python val.py --name busi_ResUKAN --output_dir outputs
```

