- If you don't want to reinstall the packages everytime you restart the kernel, simply create a python's virtual environemnt and preinstall all the packages.
    ```sh
    pip -m venv env
    ./env/Scripts/activate
    pip install -r requirements.txt
    ```
    - Using the environment requires installing the `ipykernel` package
        ```sh
        pip install ipykernel
        ipython kernel install --user --name=env
        ```
    - If you want to delete that `venv` kernel
        ```sh
        jupyter-kernelspec uninstall venv
        ```