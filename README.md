# HopfieldNet_rmsp
## A TensorFlow Implementation of Hopfield Network trained with RMSProp

You should have:

python2.7 or higher (`sudo apt install python2.7 python-pip`)

Jupyter Notebook (`python -m pip install --upgrade pip`, `python -m pip install jupyter`)

TensorFlow (`pip install tensorflow-gpu`)

TensorBoard (`pip install tensorboard`) (optionally)

CUDA 9.0 and cuDNN 7.0.5 (for TensorFlow support)

You can use pretrained HopfieldNet-model in folder 'models' by tf_hopfield_rmsp.ipynb or train your own by tf_train_hopfield_rmsp.ipynb

You can also use your own trained model, it will be in folder 'models' after training, dont forget to delete pretrained one.

This version of HopfieldNet use RMSProp-optimizer instead of standart Gradiend Descend and have a special loss-function that tries delete not only the nearest one parasitic memory and not every parasitic memories. Instead it takes both from these two worlds and increases energy levels only for 5 neares parasitic memories. It helps not to do everything at once and fail and at the same time not to be looking only for one parasitic memory letting other have pretty low energy.
