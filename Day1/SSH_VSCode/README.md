# VSCode

<p align="center">
    <img src="Visual_Studio_Code.webp" alt="VSCode">
    <img src="https://code.visualstudio.com/assets/home/home-screenshot-mac.png" alt="VSCode">
</p>
Visual Studio Code is the recommended IDE for MAIA. It is a powerful and versatile tool that can be used for a wide range of programming languages. It is also a great tool for remote development. In this tutorial series, we will show you how to use VSCode to remotely develop Python code on MAIA.

To install VSCode, go to the [VSCode website](https://code.visualstudio.com/) and download the installer for your operating system. Once you have installed VSCode, you can open it by searching for `Visual Studio Code` in your applications menu.


## VSCode Extensions
First, we will install some extensions that will make our lives easier when developing Python code on MAIA. To install an extension, click on the `Extensions` icon on the left-hand side of the window. Then, search for the extension you want to install and click the `Install` button.

The extensions we recommend are:
- Python
- GitLens
- GitHub Repositories
- Jupyter
- Remote - SSH
- Remote Development
- YAML [Optional]
- GitHub Copilot [Optional]

## Local and Remote Development

Local development is when you write and run code on your local machine. Remote development is when you write and run code on a remote machine. In this tutorial series, we will show you how to use VSCode to remotely develop Python code on MAIA.

First let's write a simple Python script to test our setup. Create a new file by clicking on the `New File` icon on the left-hand side of the window. Then, copy and paste the following code into the new file:

```python
print("Hello, World!")
```

and a second file with the following code:

```python
import numpy as np

array = np.random.randn(10)
print(np.mean(array))
print(np.std(array))
```

This may or may not execute depending on your local Python setup. And here is where the power of remote development comes in. We can run this code on MAIA without having to install Python on our local machine.
To do this, we will use the `Remote - SSH` extension. Click on the `Remote Explorer` icon on the left-hand side of the window. Then, click on the `+` icon to add a new SSH connection. Enter the SSH information that you can retrieve from your MAIA Namespace page, under the **Remote Desktops** tab.

IMPORTANT STEP!


MAIA SSH connection ONLY works with an SSH key ( so password authentication is disabled). If you don't have an SSH key, you can generate one by following the instructions available on your MAIA Workspace **Welcome** page and then download the private key to your local machine.

AFTER  you have downloaded the private key, you can add it to your SSH agent by running the following command in your terminal:

```bash
ssh-add /path/to/your/private/key
```

## Remote Jupyter Notebooks


## Remote Python Scripts

## Remote Debugger
