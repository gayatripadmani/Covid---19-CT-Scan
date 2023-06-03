# Covid---19-CT-Scan

COVID-19 Detection based on Chest X-rays and CT Scans using four Transfer Learning algorithms: VGG16, ResNet50, InceptionV3, Xception. The models were trained for 500 epochs on around 1000 Chest X-rays and around 750 CT Scan images on Google Colab GPU. After training, the accuracies acheived for the model are as follows:
<pre>
                ResNet50
CT Scans        80%      
</pre>
A Flask App was later developed wherein user can upload Chest X-rays or CT Scans and get the output of possibility of COVID infection.

The article for the project was selected and published in <b>Towards Data Science</b>:<br> 
https://towardsdatascience.com/covid-19-detector-flask-app-based-on-chest-x-rays-and-ct-scans-using-deep-learning-a0db89e1ed2a

# Dataset
The dataset for the project was gathered from two sources:
CT Scan images (750 images) were obtained from: https://drive.google.com/drive/folders/1WOeodRmv1Mw5Cswuip3nUIi6ViQWKpo_
80% of the images were used for training the models and the remaining 20% for testing

# Technical Concepts
<b>ImageNet</b> is formally a project aimed at (manually) labeling and categorizing images into almost 22,000 separate object categories for the purpose of computer vision research.<br>
More information can be found <a href="https://www.pyimagesearch.com/2017/03/20/imagenet-vggnet-resnet-inception-xception-keras/">here</a>
<br>
<br>
<b>ResNet50</b> ResNet-50 is a convolutional neural network that is 50 layers deep. You can load a pretrained version of the network trained on more than a million images from the ImageNet database. The pretrained network can classify images into 1000 object categories, such as keyboard, mouse, pencil, and many animals. Unlike traditional sequential network architectures such as AlexNet, OverFeat, and VGG, ResNet is instead a form of “exotic architecture” that relies on micro-architecture modules.<br>
More information can be found <a href="https://www.mathworks.com/help/deeplearning/ref/resnet50.html#:~:text=ResNet%2D50%20is%20a%20convolutional,%2C%20pencil%2C%20and%20many%20animals.">here</a>
<br>

## How to use Flask App
<ul>
  <li>Download repo, change to directory of repo, go to command prompt and run <b>pip install -r requirements.txt</b></li>
  <li>The dataset and models of the repository have been moved to Google Drive due to expiry of my Github LFS. So please download the zip file from <b><a href="https://drive.google.com/file/d/1dA-rdmDmCGa3xxW5KpfLJdo7M54lPcQq/view?usp=sharing">here</a></b>, extract it and replace the above data and models folder with these. Also make sure you have <b>PYTHON V 3.8.5</b>. Other versions might not be supported</li>
  <li>On command prompt, run <b>python app.py</b></li>
  <li>Open your web browser and go to <b>127.0.0.1:5000</b> to access the Flask App</li>
</ul>

## How to use Jupyter Notebooks 
<ul>
  <li>Download my repo and upload the repo folder to your <b>Google Drive</b></li>
  <li>Go to the jupyter notebooks folder in my repo, right click the notebook you want to open and select <b>Open with Google Colab</b>   </li>
  <li>Activate free <b>Google Colab GPU</b> for faster execution. Go to Runtime -> Change Runtime Type -> Hardware Accelerator -> GPU -> Save</li>
</ul>
