

Run container interactively
```
sudo docker run -i -t --rm -v $PWD/:/app ecovad
```

Run inference interactively

```
# sudo docker run -i -t --rm -v $PWD/:/app ecovad python -i  anonymise_data.py  --config ./config_inference_test.yaml
sudo docker run -i -t --rm -v $PWD/:/app ecovad python -i  ./VAD_algorithms/ecovad/ecoVAD_predict.py  --config ./config_inference_test.yaml

```