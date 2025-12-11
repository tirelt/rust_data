# Rust data

Dummy project to try Rust at tasks I would normally do in python: 🦀 >> 🐍 ??

Same excercise than [C++ data processing](https://github.com/tirelt/cpp_data_processing) which was a disaster.


## Notebook

1. Create a python `venv` with jupyter notebook (same as usual)
```Bash
python3 -m venv venv
venv/bin/activate
pip install -r requirements.txt
```

2. Installing the `evcxr_jupyter` crate 
```Bash
cargo install --locked evcxr_jupyter
```

3. Install the kernal 
```Bash
env JUPYTER_PATH=$VIRTUAL_ENV/share/jupyter/ evcxr_jupyter --install
```
Note: check that `$VIRTUAL_ENV` returns the path to the virtual env.

4. Set up VSCode 

Make sure that the Jupyter extension is installed. Open the notebook, select Jupyter Kernel and you should see the rust Kernel.
You can also use 
```Bash
jupyter kernelspec list
```
To see what kernels are available.