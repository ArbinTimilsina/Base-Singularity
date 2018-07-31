# Base-Singularity

[![https://www.singularity-hub.org/static/img/hosted-singularity--hub-%23e32929.svg](https://www.singularity-hub.org/static/img/hosted-singularity--hub-%23e32929.svg)](https://singularity-hub.org/collections/1370)

Pull the container to your machine (and optionally name custom):
```
singularity pull shub://ArbinTimilsina/Base-Singularity
singularity pull --name customname.img shub://ArbinTimilsina/Base-Singularity
```

Shell into the container:
```
singularity shell shub://ArbinTimilsina/Base-Singularity
```

Run the container:
```
singularity run shub://ArbinTimilsina/Base-Singularity
```

To run the container after the build, try
```
singularity exec customname.simg bash
```

If you want to use GPUs, don't forget --nv option
```
singularity exec --nv customname.simg bash
```

## Details
* A portable Ubuntu 16.04 environment with pre-built ML/DLframeworks including scikit-learn and keras.
* Also includes ROOTv6.14.02 and the following:
* Development kit : dpkg-dev g++ gcc binutils libqt4-dev python3-dev python3-tk python3-pip
* Utility kit     : git wget emacs vim
* Basic python    : wheel zmq six pygments pyyaml cython gputil psutil humanize h5py tqdm jupyter
* ML packages     : numpy matplotlib pandas scikit-image scikit-learn Pillow opencv-python
* DL packages     : tensorflow keras

