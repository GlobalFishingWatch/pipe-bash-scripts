# pipe-bash-scripts
Collection of bash scripts that are mostly used in pipeline repositories.

The idea of this repository is to be used in projects that currently depends on the `pipe-tools` project but they only use the scripts that the project offers instead of the python utils.


## Repositories
The `pipe-bash-scripts` repo will be represented by `gfw-bash-pipeline` Docker Image is hosted on [Container Registry](https://gcr.io/world-fishing-827/gfw-bash-pipeline).

The full repository name for Container Registry is `gcr.io/world-fishing-827/github.com/globalfishingwatch/gfw-bash-pipeline:latest`.

## Supported tags

* `:latest`: Has the current python version (3.7) and the last Google-SDK cli that are using all the pipeline steps.
* `:latest-python3.7`: Has the current python version (3.7) and the last Google-SDK cli that are using all the pipeline steps.
* `:latest-python3.8`: Has the new python version (3.8) and the last Google-SDK cli that are using the pipeline steps that requires python3.8.
* `:latest-python3.9`: Has the new python version (3.9) and the last Google-SDK cli that are using the pipeline steps that requires python3.9.
In order to update to the latest Google-SDK cli version, trigger a build.

## Usage

To use one of the images, pull from [Container Registry](https://gcr.io/google.com/cloudsdktool/cloud-sdk) and then run the following command:
Ex using the latest image.

```
docker pull gcr.io/world-fishing-827/github.com/globalfishingwatch/gfw-bash-pipeline:latest
```

To indicate in other Dockerfile use it:
```
FROM gcr.io/world-fishing-827/github.com/globalfishingwatch/gfw-bash-pipeline:latest

