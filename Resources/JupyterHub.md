# JupyterHub

[JupyterHub](https://jupyter.org/hub) is a powerful program that allows companies, classrooms or research labs to share computational hardware and run _notebook_ based code concurrently. [Jupyter's](https://jupyter.org/index.html) goal is to provide interactive computing software for different programming languages. JupyterHub allows multiple users to take advantage of a single server by separating user processes and programs. 

We foresee much of our development to be done through JupyterHub as it is simple to use, scalable and functions well for multiple use cases.

_Last Update_: Friday, December 18th, 2020

## Table of Contents
- [Setup Guide](#setup-guide)
  - [Initializing an SSH Tunnel](#initializing-an-ssh-tunnel)
  - [Opening JupyterHub in your Browser](#opening-jupyterhub-in-your-browser)
- [Running](#running)
- [Support](#support)
- [See Also](#see-also)

## Setup Guide

JupyterHub (and Jupyter in general) has a server based design. A server is responsible for running the actual code, and a client (typically visualized in a browser) can write code for the server to run. On our workstation, there is a always running server setup. This is nice, as you will never need to launch the server yourself. So, JupyterHub is essentially setup already.

### Initializing an SSH Tunnel

For you to be able to visualize JupyterHub in your browser, your computer needs to know that there is a JupyterHub instance running on the workstation. This can be done through something called an SSH Tunnel. Please see [this](https://github.com/WisconsinAutonomous/wa-resources/blob/master/Resources/SSH.md) readme for information about SSH and SSH Tunneling.

Jupyter is run on port `8000`, so you must forward that port to your own computer. In theory, you can map `8000` to any port you'd like, but we'll leave it at `8000` for simplicity. Your command may look something like this:
```bash
ssh -L 8000:localhost:8000 -J <cae username>@best-tux.cae.wisc.edu <cae username>@carproject-06.engr.wisc.edu
```

### Opening JupyterHub in your Browser

Your computer should now have access to the JupyterHub server. To open up Jupyter, go to a browser and type in `localhost:8000/jupyter`. This should open a webpage with a login prompt. Login with your cae credentials.

## Running

`TODO`

## Support

Contact [Aaron Young](aryoung5@wisc.edu) for any questions or concerns regarding the contents of this repository.

## See Also

Stay up to date with our technical info by following our [blog](https://www.wisconsinautonomous.org/blog).

Follow us on [Facebook](https://www.facebook.com/wisconsinautonomous/), [Instagram](https://www.instagram.com/wisconsinautonomous/), and [LinkedIn](https://www.linkedin.com/company/wisconsin-autonomous/about/)!

<img src="https://github.com/WisconsinAutonomous/wa-resources/blob/master/Images/WA.png" alt="Wisconsin Autonomous Logo" height="100px">  <img src="https://github.com/WisconsinAutonomous/wa-resources/blob/master/Images/UWCrest.png" alt="University of Wisconsin - Madison Crest" height="100px" align="right">
