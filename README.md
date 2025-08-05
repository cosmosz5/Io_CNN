# Io_CNN
This repository contains a Jupyter Notebook and the models to run a CNN for deconvolving the JWST AMI data of the jovian moon Io

## Instructions 
- The Jupyter Notebook is ready to be run at Google Colab. The file just need to be copied to a Google drive ane excecute it from there.
- The models and JWST science exposures are `npz` files. The whole directory can be retrieved from the following Google Drive links: [link](https://drive.google.com/drive/folders/13g7_Dz-nrog8ZL2uM2BI6Qi46gjwzG7m?usp=share_link)
- The directory with models and data should be placed at the root directory of the user's Google drive (usually /content/drive/MyDrive/). Otherwise the paths in the Jupyter Notebook should be modified.
- It is recommended that for trainning Colab's GPU should be enabled. The GPU model selected will depend on the user's capabilities, depending on its Colab's subscription plan. 
- For the trainning process the following line should be uncocommented:

``` bash
>> train(batch_size=2048, epochs=2500)
```

- For inference, the "trainning" line in the main loop of the Jupyter Notebook should be commented and the following line should be uncommented:

``` bash
>> generate(oifilename='/content/drive/MyDrive/NN_deconv_paper/n_cube_2025_4.npz')
```
** The path to the given dataset should be modified accordingly to the user's needs.

- In case of doubts about the execution of the provided code, please contact me at: <mailto:joelsb@astro.unam.mx>

