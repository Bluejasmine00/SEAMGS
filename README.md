
## Installation
### Prerequisites
- Python3
- PyTorch-0.4.+
- [OpenMPI-3.1.+](https://www.open-mpi.org/software/ompi/v3.1/)
- [Horovod-0.14.+](https://github.com/horovod/horovod)

### Quick Start
```
git clone https://github.com/HKBU-HPML/OMGS-SGD.git
cd SEAMGS
pip install -r requirements.txt
dnn=resnet20 nworkers=4 ./horovod_mpi.sh
```
Assume that you have 4 GPUs on four nodes and everything works well, you will see that there are 4 workers running at a single node training the ResNet-20 model with the Cifar-10 data set using the SEAMGS algorithm.

## Referred Models
- Deep speech: [https://github.com/SeanNaren/deepspeech.pytorch](https://github.com/SeanNaren/deepspeech.pytorch)
- PyTorch examples: [https://github.com/pytorch/examples](https://github.com/pytorch/examples)
