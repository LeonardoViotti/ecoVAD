

Run container interactively
```
sudo docker run -i -t --rm -v $PWD/:/app ecovad
```

Run inference interactively

```
# sudo docker run -i -t --rm -v $PWD/:/app ecovad python -i  anonymise_data.py  --config ./config_inference_test.yaml
sudo docker run -i -t --rm -v $PWD/:/app ecovad python -i  ./VAD_algorithms/ecovad/ecoVAD_predict.py  --config ./config_inference_test.yaml

```

Requirements:

```
conda create -n vad python=3.9
conda activate vad

pip3 install torch torchvision torchaudio

# Other libraries
pip install opensoundscape==0.8.0
pip install pydub


```