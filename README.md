# <span style="color: orange">SSH Configuration & Secure Remote Access Setup (PuTTY & Key Management)</span>

## <span style="color: orange">Introduction</span>

This project aims to demonstrate how to download and install PuTTY SSH client and create public and private SSH keys on Windows 11 virtual machine (VM) on UTM M1/M2/M3 in 2025.

*   **What is PuTTy?**

PuTTY is a free, open-source terminal emulator and network file transfer application, created in 1997 by Simon Tatham, that serves a client program for SSH and Telnet and it is used primarily to to log into another computer over a network or the Internet.

![image alt](https://github.com/Michaelsalaja/Network-Engineering-and-Cryptography-Lab/blob/408a0a952d2b5c106e229dd2cea9aa9b2975c703/Figure%201.png)

*   **What is SSH key?**

SSHkeys are used to identify oneself to an SSH server that uses public key cryptography and challenge-response authentication. An immediate advantage of this method over traditional password authentication is that you can be authenticated by the server without sending your password over the network. You can also use it with automation because it allows for unattended server communication.

## <span style="color: orange">Lab prerequisite</span>

*   The PuTTy Terminal should be installed

## <span style="color: orange">Putty Installation</span>

➢ Open a Web browser
➢ Google PuTTy
➢ Enter the PuTTy Official Website
➢ Download

Navigate to the official PuTTY website and download the "64-bit **ARM** version of the **MSI** ('Windows Installer').

![image alt](https://github.com/Michaelsalaja/Network-Engineering-and-Cryptography-Lab/blob/7c5eb9d013d120b5aacc85bee223da9e11e53dd1/Figure%202.png)


➤ **Run the installer**

![image alt](https://github.com/Michaelsalaja/Network-Engineering-and-Cryptography-Lab/blob/7c5eb9d013d120b5aacc85bee223da9e11e53dd1/Figure%203.png)

➤ The downloaded file will pop message indicating that this executable file may contain virus. Click okay to ren the setup Wizard


![image alt](https://github.com/Michaelsalaja/Network-Engineering-and-Cryptography-Lab/blob/7c5eb9d013d120b5aacc85bee223da9e11e53dd1/Figure%204.png)

➤ Click Next

![image alt](https://github.com/Michaelsalaja/Network-Engineering-and-Cryptography-Lab/blob/7c5eb9d013d120b5aacc85bee223da9e11e53dd1/Figure%205.png)

➤ Click next to accept the default installation path (usually C:\Program Files\PuTTY) and click Next.

![image alt](https://github.com/Michaelsalaja/Network-Engineering-and-Cryptography-Lab/blob/7c5eb9d013d120b5aacc85bee223da9e11e53dd1/Figure%206.png)

* Verify the selections to ensure that “Add Shortcut to PuTTY on the Desktop” is selected, then click “install”. The Rest of the default setting can be left unchanged.

![image alt](https://github.com/Michaelsalaja/Network-Engineering-and-Cryptography-Lab/blob/7c5eb9d013d120b5aacc85bee223da9e11e53dd1/Figure%207.png)

* Click Finish after the installation is completed. The installation only takes a minute. If installation lasts more than 5 minutes, then verify if the right package is chosen for an installation

![image alt](https://github.com/Michaelsalaja/Network-Engineering-and-Cryptography-Lab/blob/7c5eb9d013d120b5aacc85bee223da9e11e53dd1/Figure%208.png)

➤ Go the search bar and type PuTTy to ensure that is successfully installed
➤ Double click the icon

![image alt](https://github.com/Michaelsalaja/Network-Engineering-and-Cryptography-Lab/blob/7c5eb9d013d120b5aacc85bee223da9e11e53dd1/Figure%209.png)

➤ PuTTY is successfully installed on Windows 11

![image alt](https://github.com/Michaelsalaja/Network-Engineering-and-Cryptography-Lab/blob/7c5eb9d013d120b5aacc85bee223da9e11e53dd1/Figure%2010.png)

### Alternative Methods

*   Open the Command Prompt or PowerShell as an administrator
*   Type in the command <mark>`winget install PuTTy.PuTTy`</mark>
*   I refused to use this method for the learning purpose. Network Engineering and SOC are the pathways that I am heading to career wise

### Generating the SSH Keys on PuTTY

*   Type PuTTy on the Windows "Search bar", then double click PuTTygen

![image alt](https://github.com/Michaelsalaja/Network-Engineering-and-Cryptography-Lab/blob/7c5eb9d013d120b5aacc85bee223da9e11e53dd1/Figure%2011.png)

*   RSA is chosen by default. Leave it unchanged
*   Click "Generate"
*   During the generation process, move your mouse over the blank area on the PuTTY window to create some randomness. This instruction will also be shown on top the green label indicating the generation process.
*   A public and private key pair will then be generated

**Number of bits in a generated key:** 2048

*   Copy all the SShkey from the top by highlighting the text shown after the generation. This is necessary to ensure that nothing goes wrong if forget to save it.
*   Right-click the highlighted text and click copy

![image alt](https://github.com/Michaelsalaja/Network-Engineering-and-Cryptography-Lab/blob/7c5eb9d013d120b5aacc85bee223da9e11e53dd1/Figure%2013.png)

*   Otherwise, click "Save public key"
*   Choose a destination to save the file

![image alt](https://github.com/Michaelsalaja/Network-Engineering-and-Cryptography-Lab/blob/7c5eb9d013d120b5aacc85bee223da9e11e53dd1/Figure%2014.png)

*   Click "Save private key"
*   There will be a pop warning if you wish to save the private key with a passphrase

![image alt](https://github.com/Michaelsalaja/Network-Engineering-and-Cryptography-Lab/blob/7c5eb9d013d120b5aacc85bee223da9e11e53dd1/Figure%2015.png)

➤ I chose to add a passphrase to provide an extra layer of security

![image alt](https://github.com/Michaelsalaja/Network-Engineering-and-Cryptography-Lab/blob/7c5eb9d013d120b5aacc85bee223da9e11e53dd1/Figure%2016.png)

➤ Choose a destination and click "Save File" to save the key

![image alt](https://github.com/Michaelsalaja/Network-Engineering-and-Cryptography-Lab/blob/7c5eb9d013d120b5aacc85bee223da9e11e53dd1/Figure%2017.png)

Load Key:

In case you want to load your key, click on right pane and click "Load private key" from the drop down.

![image alt](https://github.com/Michaelsalaja/Network-Engineering-and-Cryptography-Lab/blob/7c5eb9d013d120b5aacc85bee223da9e11e53dd1/Figure%2018.png)

Here you can see other functions that can be configured on the PuTTyKey Generator, such as "Adding certificate to key"

![image alt](https://github.com/Michaelsalaja/Network-Engineering-and-Cryptography-Lab/blob/7c5eb9d013d120b5aacc85bee223da9e11e53dd1/Figure%2019.png)

Note

Providing a passphrase for your **SSH** key provides an extra layer of security, but it can also cause issues when you run automated scripts that require the protected key.

The ssh-agent can manage your keys. You enter the passphrase once. The ssh-agent keeps your key in its memory and pulls it up when needed. If you want the ssh-agent manage your keys, issue the following command:

eval $(ssh-agent)

After the program starts the ssh-add command to add your public key to the agent, the ssh-add utility searches for default keynames, of which id_rsa is one, and adds them to the ssh-agent. After you type your password, the "unlocked" key is stored with ssh-agent and can be used to authenticate against other servers.

root@bck1:~# ssh-add
Enter passphrase for /root/.ssh/id_rsa:
Identity added: /root/.ssh/id_rsa (/root/.ssh/id_rsa)
root@bck1:~#

Each time that you open a new terminal session, you are prompted for the key passphrase. Consider running the following commands to append your .bash_profile file so that ssh-agent starts with every bash session and adds your key.

echo ‘eval $(ssh-agent)’ >> ~/.bash_profile
echo ‘ssh-add’ >> ~/.bash_profile

<mark><font color="#E36C09">Conclusion</font></mark>

This lab projects helps equip people with the knowledge and skills to download and install **PuTTY SSH** client and create their own public and private **SSH** keys.
