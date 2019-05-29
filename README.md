# Earthquake Animator

## Development Build

1. In the root of this repo, create  virtual environment ([guide](https://packaging.python.org/guides/installing-using-pip-and-virtualenv/))
    ```
    python -m venv env
    ```

2. Activate the environment

    Windows
    ```
    env\Scripts\activate
    ```

    macOS and Linux
    ```
    source env/bin/activate
    ```

3. Install requirements
    ```
    python -m pip install --upgrade pip
    pip install -r requirements.txt
    pip install -r requirements_dev.txt
    ```

4. Create a `.env` in the root directory of this repo with the following info. **This file is not version controlled**. This is where we place secret credentials.
    ```
    FLASK_APP=app:APP
    FLASK_ENV="development"
    ```

5. Run the server in development
    ```
    flask run
    ```

6. _Optional:_ Create an ipython kernel to use Jupyter Notebook with this environment. After calling `jupyter notebook`, you'll need to select this kernel in the interface (see [documentation](https://ipython.readthedocs.io/en/stable/install/kernel_install.html)).
    ```
    ipython kernel install --user --name=earthquakes-env
    ```