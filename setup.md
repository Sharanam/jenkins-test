# Jenkins Installation

Jenkins Installation Ubuntu Linux Server is pretty easy. You may follow the cmds below on the VM to install it:

```bash

sudo apt update

sudo apt install openjdk-11-jdk -y

```

Check the java version now: java -version

Add the repository key to the system:

```bash
wget -q -O - https://pkg.jenkins.io/debian-stable/jenkins.io.key | sudo apt-key add -
```

Append the Debian package repository address to the server’s sources.list:

```bash
sudo sh -c 'echo deb http://pkg.jenkins.io/debian-stable binary/ > /etc/apt/sources.list.d/jenkins.list'
```

Run update:

```bash
sudo apt update
```

Install jenkins now:

```bash
sudo apt install jenkins -y

```

Installation is done!!

Check jenkins is running:

```bash
sudo systemctl status jenkins
```

Enable the Jenkins service to start at boot with the command:

```bash
sudo systemctl enable jenkins
```

You can start the Jenkins service with the command:

```bash
sudo systemctl start jenkins
```

Alternatively you can also use this official installation info:

<https://www.jenkins.io/doc/book/installing/linux/#debianubuntu>

## Optional Ref

<https://youtu.be/YJVNh6kTur4>
