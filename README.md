# MLperf-Easy
Rapid execution of MLperf tests

MLperf has a comprehensive testbed for various models and frameworks. This recipe presents a quick setup for CPU-based testing with different frameworks and models.

The first thing to do is clone the MLperf inference repo.
```
mkdir mlcommons && cd mlcommons/
git clone --recurse-submodules https://github.com/mlcommons/inference.git --depth 1
```

Create the directory for the models.
```
mkdir models && cd models/
mkdir tf onnx
cd tf/
wget -q https://zenodo.org/record/2535873/files/resnet50_v1.pb
wget -q https://zenodo.org/record/2269307/files/mobilenet_v1_1.0_224.tgz # descomprimir
cd ../onnx
wget -q https://zenodo.org/record/4735647/files/resnet50_v1.onnx
wget -q https://zenodo.org/record/4735651/files/mobilenet_v1_1.0_224.onnx
```

