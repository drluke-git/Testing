# Testing
This is a test of proceedure

1.  Create repository at github.com
2.  From terminal, clone repository to Arduino folder:  git clone <url>
3.  Create project in PlatformIO in the same Arduino folder
4.  From terminal:  git add -A
5.  From terminal:  git commit --message "Useful message here"
6.  From terminal:  git push
7.  From PlatformIO controls at bottom (blue bar), synchronize all changes

Once complete, any changes/additions can be sync'd using Source Control.
The following section explains:

1.  Make a change to a file and save it.
2.  Switch to Source Control tab
3.  Add a commit message
4.  Click the Check mark at the top to commit the change
5.  From PlatformIO controls at bottom (blue bar), synchronize all changes

You should be good!

But wait!  There's More...
You need to set up an SSH key pair to handle push/pull as ID/PW will no longer be supported.

1.  Download 64-bit PUTTY and all associated apps including PLINK.
2.  Use PuttyGen to make an RSA 2048 keypair.
3.  Set up a Putty session to github.com.  Don't worry.  You can't actually connect, but you will be able to accept the server key.
4.  Log into GitHub and add the Public key from Step 2 under Settings\SSH and GPG Keys
5.  Add a system variable to the Windows environment:  GIT_SSH=C:\Program Files\PuTTY\plink.exe
6.  Start Pagent (PuTTY Authentication Agent)
7.  From Pagent in system tray, click Add Key and add the Putty private PPK from Step 2.
8.  Profit!
