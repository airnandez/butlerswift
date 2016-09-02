# Tutorial on OpenStack Swift Python SDK

## Introduction

This repository contains a short tutorial for getting started using the official Python SDK for OpenStack Swift. It is written in the form of a Python 3 notebook using Continuum Analytics' [Anaconda](https://www.continuum.io/downloads).

## Setting up your testing environment
First, you need to setup your environment by executing the steps below:

**Step 1:** Create a `conda` environment for this project. We will name it `swiftenv`. You only need to create it once. The purpose of this step is to create a dedicated environmente which we will modify by installing some dependencies specific to this project. Although this step is not strictly necessary, it is convenient so not to pollute your standard Anaconda installation:

```bash
conda create --name swiftenv python=3 ipython-notebook
```

More information about `conda` environments can be found [here](http://conda.pydata.org/docs/using/envs.html).

**Step 2:** Activate the `swiftenv` environment. You need to activate the environment anytime you want to work with this notebook. You need to activate it so that the dependencies we install in the next step are installed in the appropriate environment:

```bash
source activate swiftenv
```

**Step 3:** Install the [official Swift Python client](https://pypi.python.org/pypi/python-swiftclient) into the `swiftenv` environment. You only need to install these dependencies once:

```bash
pip install python-swiftclient python-keystoneclient
```

## Using the notebook

Once your testing environment is set up you are ready to use the notebook. Clone this repository and open the notebook:

```bash
$ source activate swiftenv
$ git clone https://github.com/airnandez/butlerswift.git
$ cd butlerswift
$ ipython notebook
```

## Destroying your testing environment
Once you are done, you may want to delete the `swiftenv` environment:

```bash
conda remove --name swiftenv --all
```

## Credits

### Author
These tools were developed and are maintained by Fabio Hernandez at [IN2P3 / CNRS computing center](http://cc.in2p3.fr) (Lyon, France).

## License
Copyright 2016 Fabio Hernandez

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

[http://www.apache.org/licenses/LICENSE-2.0](http://www.apache.org/licenses/LICENSE-2.0)

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.


