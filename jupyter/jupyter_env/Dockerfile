FROM jupyter/scipy-notebook:latest


RUN pip install --upgrade pip
RUN pip install tensorflow
RUN pip install torch torchvision
RUN pip install --upgrade jupyterthemes autopep8 isort yapf
RUN pip install jupyter_contrib_nbextensions && \
    jupyter contrib nbextension install --user
# enable the Nbextensions
RUN jupyter nbextension enable autosavetime/main
RUN jupyter nbextension enable codefolding/main
RUN jupyter nbextension enable code_font_size/code_font_size
RUN jupyter nbextension enable code_prettify/code_prettify
RUN jupyter nbextension enable code_prettify/autopep8
RUN jupyter nbextension enable code_prettify/isort
RUN jupyter nbextension enable execute_time/ExecuteTime
RUN jupyter nbextension enable spellchecker/main
RUN jupyter nbextension enable scratchpad/main
RUN jupyter nbextension enable hinterland/hinterland
RUN jupyter nbextension enable varInspector/main
RUN jupyter nbextension enable highlighter/highlighter
