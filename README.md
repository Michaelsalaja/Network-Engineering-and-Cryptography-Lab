# <span style="color: orange">PuTTy Installation and SSH Keys Generation</span>

## <span style="color: orange">Introduction</span>

This project aims to demonstrate how to download and install PuTTY SSH client and create public and private SSH keys on Windows 11 virtual machine (VM) on UTM M1/M2/M3 in 2025.

*   **What is PuTTy?**

PuTTY is a free, open-source terminal emulator and network file transfer application, created in 1997 by Simon Tatham, that serves a client program for SSH and Telnet and it is used primarily to to log into another computer over a network or the Internet.

![PuTTY icon showing two computers connected by a lightning bolt](image)

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

![Screenshot of the PuTTY download page in a web browser, with the 64-bit Arm installer highlighted.](image)

# Download PuTTY: latest release (0.83)

Home | FAQ | Feedback | Licence | Updates | Mirrors | Keys | Links | Team
Download: **Stable** · Snapshot Docs | Privacy | Changes | Wishlist

This page contains download links for the latest released version of PuTTY. Currently this is 0.83, released on 2025-02-08.

When new releases come out, this page will update to contain the latest, so this is a good page to bookmark or link to. Alternatively, here is a permanent link to the 0.83 release.

Release versions of PuTTY are versions we think are reasonably likely to work well. However, they are often not the most up-to-date version of the code available. If you have a problem with this release, then it might be worth trying out the development snapshots, to see if the problem has already been fixed in those versions.

## Package files

You probably want one of these. They include versions of all the PuTTY utilities (except the new and slightly experimental Windows pterm).

(You probably want the 64-bit x86 version. The 32-bit version is only for backward compatibility with very old PCs / versions of Windows.)

We also publish the latest PuTTY installers for all Windows architectures as a free-of-charge download at the Microsoft Store; they usually take a few days to appear there after we release them.

**MSI ('Windows Installer')**
*   64-bit x86: putty-64bit-0.83-installer.msi (signature)
*   <mark>64-bit Arm: putty-arm64-0.83-installer.msi (signature)</mark>
*   32-bit x86: putty-0.83-installer.msi (signature)

**Unix source archive**
*   .tar.gz: putty-0.83.tar.gz (signature)

## Alternative binary files

The installer packages above will provide versions of all of these (except PuTTYtel and pterm), but you can download standalone binaries one by one if you prefer.

(You probably want the 64-bit x86 version. The 32-bit version is only for backward compatibility with very old PCs / versions of Windows.)

**putty.exe (the SSH and Telnet client itself)**
*   64-bit x86: putty.exe (signature)
*   64-bit Arm: putty.exe (signature)
*   32-bit x86: putty.exe (signature)

---

➤ **Run the installer**

![Screenshot showing the browser download manager with the completed download of putty-arm64-0.83-installer.msi.](image)

➤ There will a pop message indicating that this executable file may contain virus. Click okay to ren the setup Wizard

www.chiark.greenend.org.uk/~sgtatham/putty/latest.html

# Download PuTTY: latest release (0.83)

Home | FAQ | Feedback | Licence | Updates | Mirrors | Keys | Links | Team
Download: **Stable** · Snapshot Docs | Privacy | Changes | Wishlist

This page contains download links for the latest released version of PuTTY. Currently this is 0.83, released on 2025-02-08.

When new releases come out, this page will update to contain the latest, so this is a good page to bookmark or link to. Alternatively, here is a permanent link to the 0.83 release.

Release versions of PuTTY are versions we think are reasonably likely to work well. However, they are often not the most up-to-date version of the code available. If you have a problem with this release, then it might be worth trying out the development snapshots, to see if the problem has already been fixed in those versions.

<div style="border: 1px solid black; padding: 10px; border-radius: 10px;">

### Package files

You probably want one of these. They include versions of all the PuTTY utilities (except the new and slightly experimental Windows pterm).

(You probably want the 64-bit x86 version. The 32-bit version is only for backwards compatibility with very old hardware.)

We also publish the latest PuTTY installers for all Windows architectures as a combined installer, which we update shortly after we release them.

**MSI ('Windows Installer')**
*   64-bit x86: putty-64bit-0.83-installer.msi (signature)
*   64-bit Arm: putty-arm64-0.83-installer.msi (signature)
*   32-bit x86: putty-0.83-installer.msi (signature)

**Unix source archive**
*   .tar.gz: putty-0.83.tar.gz (signature)

</div>

![A browser security warning dialog box titled "Open Executable File?" with the message: "'putty-arm64-0.83-installer.msi' is an executable file. Executable files may contain viruses or other malicious code that could harm your computer. Use caution when opening this file. Are you sure you want to launch 'putty-arm64-0.83-installer.msi'?" with OK and Cancel buttons.](image)

➤ Click Next

![The PuTTY release 0.83 (64-bit Arm) Setup Wizard window. On the left is a blue sidebar with various computer-related icons (network, terminal, key, computer). On the right, the text reads: "Welcome to the PuTTY release 0.83 (64-bit Arm) Setup Wizard. The Setup Wizard will install PuTTY release 0.83 (64-bit Arm) on your computer. Click Next to continue or Cancel to exit the Setup Wizard." At the bottom are Back, Next, and Cancel buttons.](image)

➤ Click next to accept the default installation path (usually C:\Program Files\PuTTY) and click Next.

![PuTTY release 0.83 (64-bit Arm) Setup window showing Destination Folder selection. The path is set to C:\Program Files\PuTTY\.](image)

Ø Verify the selections to ensure that “Add Shortcut to PuTTY on the Desktop” is selected, then click “install”. The Rest of the default setting can be left unchanged.

![PuTTY release 0.83 (64-bit Arm) Setup window showing Product Features. "Add shortcut to PuTTY on the Desktop" is highlighted.](image)

Ø Click Finish after the installation is completed. The installation only takes a minute. If installation lasts more than 5 minutes, then verify if the right package is chosen for an installation

![Screenshot of the PuTTY release 0.83 (64-bit Arm) Setup Wizard showing the completion screen with a Finish button.](image)

➤ Go the search bar and type PuTTy to ensure that is successfully installed
➤ Double click the icon

![Screenshot of the Windows 11 search menu showing PuTTY as the best match after installation.](image)

➤ PuTTY is successfully installed on Windows 11

![PuTTY Configuration window showing session settings, host name, port, and connection type options.](image)

### Alternative Methods

*   Open the Command Prompt or PowerShell as an administrator
*   Type in the command <mark>`winget install PuTTy.PuTTy`</mark>
*   I refused to use this method for the learning purpose. Network Engineering and SOC are the pathways that I am heading to career wise

### Generating the SSH Keys on PuTTY

*   Type PuTTy on the Windows "Search bar", then double click PuTTygen

![Screenshot of PuTTY Key Generator window showing no key loaded.](image)

*   RSA is chosen by default. Leave it unchanged
*   Click "Generate"
*   During the generation process, move your mouse over the blank area on the PuTTY window to create some randomness. This instruction will also be shown on top the green label indicating the generation process.
*   A public and private key pair will then be generated

![Screenshot of PuTTY Key Generator window showing a generated RSA key.](image)

**PuTTY Key Generator**

**Key**
**Public key for pasting into OpenSSH authorized_keys file:**
```
ssh-rsa
AAAAB3NzaC1yc2EAAAADAQABAAABAQCoo4FCj4C40vNpF5I7Hq43AsMAHINYozG5e/evLV7qnGgOCH5V09
YnhH0C7c7royR5JRbB2ml8fqSMBBd6f0LQ9bCO94EadO/JHCZ/uwjcyL3ApxyyaSNJCh1SnlGvcxoLPbRLVyzbM
w0yhGJoOwTe/KKaNExM5u2B8GQUXJGVKRQIbSV1AWNMApKkvUqmQxCholbYsdpcKQlO7hRMeE5xRhT2al
KH0TfzjWKUNB4IFR01C9VzgV+rtfYvGXy38g0UqeNjoW23TmB
```

**Key fingerprint:** ssh-rsa 2048 SHA256:eXeyqLvd/Sg51tBO9/k5Ov0cqPtgSIHKZQt//6836YI
**Key comment:** rsa-key-20260131
**Key passphrase:**     
**Confirm passphrase:**     

**Actions**
**Generate a public/private key pair**: [Generate]
**Load an existing private key file**: [Load]
**Save the generated key**: [Save public key] [Save private key]

**Parameters**
**Type of key to generate:**
*   RSA [x]
*   DSA [ ]
*   ECDSA [ ]
*   EdDSA [ ]
*   SSH-1 (RSA) [ ]

**Number of bits in a generated key:** 2048

*   Copy all the SShkey from the top by highlighting the text shown after the generation. This is necessary to ensure that nothing goes wrong if forget to save it.
*   Right-click the highlighted text and click copy

![Screenshot of the PuTTY Key Generator window showing a generated RSA key. The public key text is highlighted in blue, and a right-click context menu is open with the 'Copy' option visible.](image)

*   Otherwise, click "Save public key"
*   Choose a destination to save the file

![Screenshot of a file explorer window titled "Save public key as:" showing the selection of a folder named "SSH Keys" and the file name "SSH_PublicKeys" being entered.](image)

*   Click "Save private key"
*   There will be a pop warning if you wish to save the private key with a passphrase

![Screenshot of the PuTTY Key Generator interface showing a generated public key, key fingerprint, and a "PuTTYgen Warning" dialog box asking "Are you sure you want to save this key without a passphrase to protect it?" with "Yes" and "No" options.](image)

**PuTTY Key Generator**

**Key**
*   **Public key for pasting into OpenSSH authorized_keys file:**
    `ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQCoo4FCj4C40vNpF5I7Hq43AsMAHINYozG5e/evLV7qnGgOCH5V09YnhH0C7c7royR5JRbB2ml8fgSMBBd6f0LQ9bCO94EadO/JHCZ/uwjcyL3ApxyyaSNJCh1SnlGvcxoLPbRLVyzbMwOyhGJoOwTe/KKaNExM5u2B8GQUXJGVKRQlbSV1AWNMApKkvUgmQxCholbYsdpcKQIO7hRMeE5xRhT2alKH0TfzjWKUNB4IFR01C9VzgV+tfYvGXy38g0UqeNjoW23TmB`
*   **Key fingerprint:** `ssh-rsa 2048 SHA256:eXeyqLvd/Sg51tBO9/k5OvOcqRtgSIHKZQt//6836YI`
*   **Key comment:** `rsa-key-20260131`
*   **Key passphrase:**     
*   **Confirm passphrase:**     

**Actions**
*   Generate a public/private key pair
*   Load an existing private key file
*   Save the generated key: [Save public key] [Save private key]

**Parameters**
*   **Type of key to generate:**
    *   RSA [x]
    *   DSA [ ]
    *   ECDSA [ ]
    *   EdDSA [ ]
*   **Number of bits in a generated key:** 2048

➤ I chose to add a passphrase to provide an extra layer of security

![Screenshot of PuTTY Key Generator window showing a generated RSA key. Red boxes highlight the "Key passphrase" and "Confirm passphrase" fields, both filled with dots.](image)

➤ Choose a destination and click "Save File" to save the key

![Screenshot of a Windows "Save private key as:" dialog box. The file path is set to "Documents > SSH Keys". The file name is entered as "SSH_PrivateKey" and the file type is "PuTTY Private Key Files (*.ppk)". Red boxes highlight the file path, the Downloads folder in the sidebar, and the File name field.](image)

Load Key:

In case you want to load your key, click on right pane and click "Load private key" from the drop down.

![PuTTY Key Generator window showing the File menu with 'Load private key' selected.](image)

Here you can see other functions that can be configured on the PuTTyKey Generator, such as "Adding certificate to key"

![PuTTY Key Generator window showing the Conversions menu with various options including 'Add certificate to key', 'SSH-2 RSA key', and prime generation settings.](image)

Note

Providing a passphrase for your **SSH** key provides an extra layer of security, but it can also cause issues when you are run automated scripts that require the protected key.

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
