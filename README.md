# Image_Classification_101
This project aims to build a multi-classification image model for practice and hands-on experience.

## Setting up Mac GPU usage

To utilize the Apple GPU for training the model with TensorFlow and PyTorch, follow the steps mentioned in this article: [How to Use GPU with TensorFlow and PyTorch Libraries on MacBook Pro M2Apple](https://www.linkedin.com/pulse/how-use-gpu-tensorflow-pytorch-libraries-macbook-pro-m2apple-kashyap/)

If you encounter any errors while installing virtualenv, you can refer to this solution from Stack Overflow: [Virtualenv Command Not Found](https://stackoverflow.com/questions/31133050/virtualenv-command-not-found)

To verify the successful installation, you can check the codes provided in this article: [How to Enable GPU Support for TensorFlow or PyTorch on macOS](https://medium.com/bluetuple-ai/how-to-enable-gpu-support-for-tensorflow-or-pytorch-on-macos-4aaaad057e74)

## Steps to setup the Kaggle API to download dataset directly from kaggle to Project Terminal
- First, you need to create a kaggle account -> your account -> "Create New API Token" -> download's a file kaggle.json.
- Then, you need to move this file to the .kaggle directory in your home directory. If this directory does not exist, you can create it by running the following command in your terminal:
```bash
mkdir ~/.kaggle
```
- Then, you need to move the kaggle.json file to the .kaggle directory by running the following command in your terminal:
```bash
mv ~/Downloads/kaggle.json ~/.kaggle
```
- Finally, you need to change the permissions of the kaggle.json file so that only you can read and write to it by running the following command in your terminal:
```bash
chmod 600 ~/.kaggle/kaggle.json
```
- Now, you should be able to use the kaggle API to download datasets directly from kaggle to your Jupyter Notebook.

Now download the dataset using the following code in the terminal:
```
    kaggle datasets download -d vishweshsalodkar/wild-animals
```

To extract the zip file, use the following command in the terminal:
``` 
    unzip file_name.zip 

```


# Test Images
I have downloaded 5 diffrent classes of images from the internet to test the model. The images are as follows:
``` 
    Test_Images
        - Lion
        - Cheetah
        - Jaguar
        - Tiger
        - Leopard
```
