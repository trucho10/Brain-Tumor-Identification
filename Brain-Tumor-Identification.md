# Brain Tumor Identification on Brainy Pi

![Brain Tumor Identification](https://content.instructables.com/FW1/6PGN/LK40PV6Z/FW16PGNLK40PV6Z.jpg?auto=webp&frame=1&width=1024&fit=bounds&md=86ee9d4012a4fc708d16cdb9a9f70d15)

Brain Tumor Identification using CNN aims to use a convolutional neural network model to detect tumors in brain MRI images. Using this model, a new brain MRI image can be analyzed to find out if it has a tumor.

In this project, we implemented a brain tumor identification model on [Brainy Pi](https://brainypi.com/).

Since this project exploits two different models for a classification task (the VGG16 model and the MobileNetV2 model), results can be reported more confidently. This is because each model serves as a second opinion on the predictions made by the other. In the case of brain MRI images where both models report the same (either tumorous or non-tumorous) observation, it becomes more compelling to believe. On the other hand, in a few instances where the models disagree, additional opinions can be obtained from domain experts before any final conclusion is reached. This makes the project versatile and fit for actual use to classify Brain MRI images as tumorous or non-tumorous.

## Supplies
![Brain Tumor Identification1](https://content.instructables.com/F2B/QO4Y/LK40PUVP/F2BQO4YLK40PUVP.jpg?auto=webp&frame=1&width=1024&fit=bounds)
- Brainy Pi
- UNIX OS Terminal

## Step 1: Remote Connection to Brainy Pi
![Brain Tumor Identification2](https://content.instructables.com/FVU/62BH/LK40PUZ5/FVU62BHLK40PUZ5.png?auto=webp&frame=1&width=1024&fit=bounds&md=5045e488ba8ecd0c526eb624ebce4225)

Log in to a remote Brainy Pi: In the Terminal or Command Prompt, use the following command to initiate the SSH connection:

```
ssh -X pi@auth.iotiot.in -p 65530
```

After establishing the connection, enter the password when prompted. Type "yes" to continue.

Once the correct password has been entered, a connection to the remote Brainy Pi's command-line interface is established.

## Step 2: Cloning the Git Repository

Next is to clone the project's repository:

```
git clone https://gitlab.iotiot.in/interns-projects/brain-tumor-identification.git
```

Navigate to the project's directory using the command:

```
cd jay-patankar/brain-tumor-identification/demo
```

## Step 3: Run Model Inference Program

![Brain Tumor Identification3](https://content.instructables.com/FVX/7SEB/LK40PV43/FVX7SEBLK40PV43.png?auto=webp&frame=1&width=1024&fit=bounds&md=c29377d1afe8f07cc875e7b4fa6652c2)

In the directory where the Inference.py file is located, run the following command:
```
python3 Inference.py
```

Finally, the output is the result of model inference to identify whether there is a brain tumor or not.

> Note: Install dependencies: Install any additional dependencies or libraries required by the application on the Brainy Pi.


