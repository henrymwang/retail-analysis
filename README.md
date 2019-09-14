# Retail Analysis

This repo contains scripts to visualize and model retail data.

## Install Dependencies

This project was developed in Python 3.7.1

1. Create a new virtual environment

```
$ python3 -m venv venv
```

2. Activate the virtual environment

```
$ source venv/bin/activate
```

3. Install required dependencies from `requirements.txt`

```
(venv) $ pip install -r requirements.txt
```

## Running this notebook

1. Activate virtual environment

```
$ source venv/bin/activate
```

2. Create a kernel using this virtual environment (this way the notebook uses the
  installed dependencies from this environment, instead of the system-level environment)

```
(venv) $ ipython kernel install --user -name=retail-analysis
```

3. Start the Jupyter Notebook and make sure the kernel is `retail-analysis`

```
(venv) $ jupyter notebook
```


## Contributing

This project uses `pip-tools` for dependency management. To add a new dependency:

1. Ensure your virtual environment has been activated and install the dependency

```
(venv) $ pip install my_dependency
```

2. Add your new dependency to `requirements.in` (*note* only top-level dependencies go in this file)

```
(venv) $ pip freeze | grep my_dependency
```

3. Re-compile your dependencies

```
(venv) $ pip-compile --annotate requirements.in
```
