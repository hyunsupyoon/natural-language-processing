# natural-language-processing
Resources for "Natural Language Processing" [Coursera course](https://www.coursera.org/learn/language-processing).

## Setup with Mac OS (Reference : docker/Dockerfile)
1. install Starspace
    1. install boost
        ```
        brew install boost
        ```
    1. install Starspace
        ```
        git clone https://github.com/facebookresearch/Starspace.git
        cd Starspace        
        make
        ```
1. setup pyenv
    ```
    pyenv virtualenv 3.6.1
    pyenv local 3.6.1
    pyenv virtualenv nlp 
    pyenv local nlp
    ```
    
1. install python package
    ```
    pip install --upgrade pip
    pip install -r docker/requirements.txt
    ```

1. install Jupyter
    ```
    jupyter nbextension enable --py --sys-prefix widgetsnbextension
    jupyter contrib nbextension install
    jupyter nbextension enable codefolding/main
    echo "jupyter notebook --no-browser --allow-root" >> /usr/local/bin/run_notebook && chmod +x /usr/local/bin/run_notebook
    ```
