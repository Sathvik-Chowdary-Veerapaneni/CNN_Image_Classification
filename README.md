# Image_Classification_101
Image_Classification Model that classifies between dog and cat.

- Setting up Mac GPU usage to use the Apples GPU for training the model.
- For both tesnorflow and pytorch.
- using this article , https://www.linkedin.com/pulse/how-use-gpu-tensorflow-pytorch-libraries-macbook-pro-m2apple-kashyap/

If you got any error while installing virtual env, here the solution,
from stackoverflow, https://stackoverflow.com/questions/31133050/virtualenv-command-not-found
"So, to solve the issue, do pip uninstall virtualenv and then reinstall it with sudo pip install virtualenv (or install as root)"

check with codes using this article to ensure wether the installations weree successful or not,
https://medium.com/bluetuple-ai/how-to-enable-gpu-support-for-tensorflow-or-pytorch-on-macos-4aaaad057e74

# Steps to setup the Kaggle API to download dataset directly from kaggle to Jupyer Notebook
- First, you need to create a kaggle account and then go to your account and click on "Create New API Token" button. This will download a file called kaggle.json.
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

Now load the dataset using the following code:
```python
bash or zsh terminal : kaggle datasets download -d vishweshsalodkar/wild-animals
```
unzip file_name.zip , it will extract the file to the current directory.


Every project has to be purposeful, so here is the purpose of this project:
- I would like to identify a tiger from the images.
- A single image classifcation model that can classify wetheer the image is a tiger or not.
