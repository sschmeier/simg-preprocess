[![https://www.singularity-hub.org/static/img/hosted-singularity--hub-%23e32929.svg](https://www.singularity-hub.org/static/img/hosted-singularity--hub-%23e32929.svg)](https://singularity-hub.org/collections/2394)


# Singularity config for simg-preprocess container

A [Singularity Hub](https://www.singularity-hub.org/) definition for preprocess workflow.

If [Singularity](https://sylabs.io/docs/) is installed locally, the container can be build (needs root access) locally like this:

```bash
sudo singularity build simg-preprocess.simg Singularity
```

The container can alos be downloaded from [Singularity Hub](https://www.singularity-hub.org/) without root access to the local machine like this:

```bash
singularity pull --name "simg-preprocess.sif" sschmeier/simg-preprocess:201911
```

Then, it can be used, e.g.:

```bash
singularity exec simg-preprocess.sif fastp --version

# to bind directory not in $HOME
singularity exec --bind /mnt/disk1/seb simg-preprocess.sif fastp --version
```
