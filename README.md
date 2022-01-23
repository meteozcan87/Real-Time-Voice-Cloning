# This is the documentary of the challenge of running a Ptyhon Repo from GitHub
Click [here](https://github.com/meteozcan87/Real-Time-Voice-Cloning) to see the source of repository. I forked it into my own GitHub

I also added the sample voices that I created in order to run the code and output files.

---
# Setup

## Install Requirements
1. Both Windows and Linux are supported. A GPU is recommended for training and for inference speed, but is not mandatory.

    ### **I run the code by using Windows and Nvidia GTX 860M graphics card.**

2. Python 3.7 is recommended. Python 3.5 or greater should work, but you'll probably have to tweak the dependencies' versions. I recommend setting up a virtual environment using `venv`, but this is optional.
    ### **I created an environment by using anaconda with Pyton 3.7.**
    ```bash
    conda create -n real-time-voice-cloning python=3.7
    ```
    ![alt text][anaconda-env]

[anaconda-env]: ./anaconda-env.png "1"

3. Install [ffmpeg](https://ffmpeg.org/download.html#get-packages). This is necessary for reading audio files.
    ### **ffmeg library was not included in requirements. Therefore I installed it:**
    
    ```bash
    pip install ffmpeg
    ```

4. Install [PyTorch](https://pytorch.org/get-started/locally/). Pick the latest stable version, your operating system, your package manager (pip by default) and finally pick any of the proposed CUDA versions if you have a GPU, otherwise pick CPU. Run the given command.

    ### **I have found out that when you enter the command on PIP to intall pytorch, it also includes the right version of CUDA Toolkit and install it. Thus, I used this command:**
    ```bash
    pip install -c pytorch pytorch
    ```

5. Install the remaining requirements with `pip install -r requirements.txt`
    
    ### **By using "Open Terminal" in my environent in Anaconda, first I set my root folder of my repository. Then I entered the comment as shown above in order to install the required dependencies**

    ```bash
    pip install -r requirements.txt
    ```
    
    ![alt text][repo-terminal]

[repo-terminal]: ./repo-terminal.png "2"


6. (Optional) Download Pretrained Models
Pretrained models are now downloaded automatically. If this doesn't work for you, you can manually download them [here](https://github.com/CorentinJ/Real-Time-Voice-Cloning/wiki/Pretrained-models).
    
### **As it is written above, it did not work automatically. Therefore I downloaded the pretrained model files and saved the files in my repository**

![alt text][pretrained-models]

[pretrained-models]: ./pretrained-models.png "3"

7. (Optional) Test Configuration
Before you download any dataset, you can begin by testing your configuration with:

`python demo_cli.py`

If all tests pass, you're good to go.
### **I run this command in order to test my configuration**

```bash
python demo_cli.py
```
See the screen recording video file "running-demo.mp4"

---
# Run

## Launch the Toolbox
You can then try the toolbox:

`python demo_toolbox.py -d <datasets_root>`  
or  
`python demo_toolbox.py`  
### **After testing the system, I was ready to run the code**

```bash
python demo_toolbox.py
```
See the screen recording video file "running-code.mp4"
See the screen recording video file "creating-outputs.mp4"