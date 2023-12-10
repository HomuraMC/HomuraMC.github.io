---
layout: default
title: Build a server
lang: en-US
---
# Build a server
This guide will allow you to build a Minecraft server using HomuraMC.
## system requirement
### Supported Versions
<table class="table table-striped">
	<tr>
		<th scope="col">Minecraft Version</th>
		<th scope="col"></th>
	</tr>
	<tr>
		<td>~1.16.3</td>
		<td>×</td>
	</tr>
	<tr>
		<td>1.16.4 / 1.16.5</td>
		<td>◯</td>
	</tr>
	<tr>
		<td>1.17~</td>
		<td>×</td>
	</tr>
	<tr>
		<td>Bedrock Edition</td>
		<td>×</td>
	</tr>
</table>

We plan to support all versions in stages.

### Supported OS
<table class="table table-striped">
	<tr>
		<th scope="col">OS</th>
		<th scope="col"></th>
	</tr>
	<tr>
		<td>Windows</td>
		<td>△<a href="#sys-ok-1"><small>*1</small></a></td>
	</tr>
	<tr>
		<td>Mac</td>
		<td>△<a href="#sys-ok-2"><small>*2</small></a></td>
	</tr>
	<tr>
		<td>Linux</td>
		<td>◯</td>
	</tr>
</table>

<a id="sys-ok-1"></a><small>*1 It can be run by using WSL. So it only works on Windows 10 / Windows 11.</small><br>
<a id="sys-ok-2"></a><small>*2 Not confirmed to work.</small>

### Required Specs
<table class="table table-striped">
	<tr>
		<th scope="col">Specs</th>
		<th scope="col"></th>
	</tr>
	<tr>
		<td>CPU</td>
		<td>1GHz</td>
	</tr>
	<tr>
		<td>RAM</td>
		<td>2GB</td>
	</tr>
	<tr>
		<td>storage</td>
		<td>512MB</td>
	</tr>
</table>

### Recommended Specs
<table class="table table-striped">
	<tr>
		<th scope="col">Specs</th>
		<th scope="col"></th>
	</tr>
	<tr>
		<td>CPU</td>
		<td>2.5GHz</td>
	</tr>
	<tr>
		<td>RAM</td>
		<td>4GB</td>
	</tr>
	<tr>
		<td>storage</td>
		<td>1024MB</td>
	</tr>
</table>

## Building the server
### Installing Python
For Windows, from [here](https://www.python.org/downloads/windows/),  
For Mac, go to [here](https://www.python.org/downloads/macos/),  
For Ubuntu, go to [here](https://www.python.jp/install/ubuntu/index.html),  
For other Linux platforms, download Python from [here](https://www.python.jp/install/centos/index.html)  
Download and install Python from [here]() for Ubuntu and [here]() for other Linux.  
If you are able to install it, proceed to the next step.

### Installing Git
Download and install Git from [here](https://git-scm.com/downloads).  
If you are able to install it, go to the next step.

### Building and constructing HomuraMC environment
First, run this command in a folder of your choice.
```
git clone https://github.com/HomuraMC/Homura.git
```
Next, create a Python virtual environment. (Recommended)
```
python3 -m venv homura
```
Once you have created the virtual environment, access Python in the virtual environment using the following command.
```
cd . /homura/scripts/Activate
```
Next, use pip to install the libraries required by Homura.  
```
python3 -m pip install -r requirements.txt
```
After installation, you can start the server by running the following command.  
```
python3 main.py
```
Congratulations, you have successfully built HomuraMC! If you have made it this far without any errors, you have successfully built HomuraMC!
  
<div style="display: flex;">
	<div class="maeato">
		<b>back</b><br>
		<a href="/docs/en-us/">Main Page</a>
	</div>

	<div class="maeato">
		<b>next</b><br>
		<a href="/docs/en-us/config/">Config</a>
	</div>
</div>