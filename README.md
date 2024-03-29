<!DOCTYPE html>
<html>
<!-- <style>
    head {text-align: center}
    body {background-color: powerblue;}
    th {
        text-align: center; 
        font-weight:"bold";
        font-size: 20px;
    }
    p {font-size: 20px;}
    h2 {font-weight: bold;
        font-size:30px;}
    h1 {font-weight: bold;
        font-size:50px;}
</style> -->

<body style="background-color: powerblue;">

<table>
    <th style="font-size: 30px;"><b>Table of contents</b></th>
    <tr>
        <th><a href="#C1">Introduction</a></th>
    </tr>
    <tr>
        <th><a href="#C2">Installation</a></th>
    </tr>
    <tr>
        <th><a href="#C3">Usage</a></th>
    </tr>
    <tr>
        <th><a href="#C4">Contributing</a></th>
    </tr>
    <tr>
        <th><a href="#C5">Reference</a></th>
    </tr>
</table>

<br>

<h1 style="font-weight: bold;"> HOW TO INSTALL UBUNTU VIA VAGRANT </h1>

<h2 id="C1" style="font-weight: bold;">Introduction</h2>
<hr>

<p>Vagrant is an open-source software product for building and maintaining portable virtual software development environments; e.g., for VirtualBox, KVM, Hyper-V, Docker containers, VMware, and AWS. It tries to simplify the software configuration management of virtualization in order to increase development productivity. Vagrant is written in the Ruby language, but its ecosystem supports development in a few other languages. (<a href="https://en.wikipedia.org/wiki/Vagrant_(software))" target="_blank">Wikipeadia</a>
)</p>

<h2 id="C2" style="font-weight: bold;">Installation</h2>
<hr>

<p>Initially, we create a <b>"Virtual Machine"</b> folder in your <b>File Explorer</b>.</p>

<img src="image/1.png" alt="File Explorer">

<p>Download Vagrant via this link: <a href="https://www.vagrantup.com/downloads" target="_blank">https://www.vagrantup.com/downloads</a></p>

<p>After that, we choose <q style="font-weight: bold;">Amd64</q> in the picture below:</p>

<img src="image/2.png" alt="Vagrant download picture">

<p>We need follow the wizard and then we will check whether it exists:</p>

```bash
vagrant --version
```

<img src="image/3.png" alt="Vagrant check on terminal">

<h2 id="C3" style="font-weight: bold;">Usage</h2>
<hr>

<p>Next, we initialize the <b>Vagrant</b> on the terminal console with <b>Administrators</b> permissions.</p>

```bash
vagrant init generic/ubuntu2010
```

<img src="image/4.png" alt="initialize vagrant">

<p>It will appear in your folder:</p>

<img src="image/5.png" alt="Vagrantfile">

<p>Then we install <b>VirtualBox</b> as providers:</p>

<p>Link: <a href="https://www.virtualbox.org/wiki/Downloads" target="_blank">https://www.virtualbox.org/wiki/Downloads</a></p>

<p>Then we choose "Windows hosts"</p>

<img src="image/virtualbox.png" alt="virtualbox">


<p>After installing virtualbox providers, we activate Vagrant by a command below:</p>

```bash
vagrant up --provider=virtualbox
```

<p>In this case, I have already downloaded it before. So it can be seen as a successful work.</p>

<img src="image/run.png" alt="vagrant up">

<p>Finally, we open ubuntu kernel with <b>"ssh" keyword</b>.</p>

```bash
vagrant ssh
```

<img src="image/ssh.png" alt="ssh">

<p>From here, we're able to access ubuntu kernel and do your works.</p>

<h2 id="C4" style="font-weight: bold;">Contributing</h2>
<hr>

<p>Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate</p>

<h2 id="C5" style="font-weight: bold;">References</h2>
<hr>

<a href="https://www.vagrantup.com/" target="_blank">https://www.vagrantup.com/</a>

<a href="https://app.vagrantup.com/boxes/search" target="_blank">https://app.vagrantup.com/boxes/search</a>

</body>
</html>