ssh-agent on Bash on Ubuntu on Windows
======================================

Scripts to use to persist `ssh-agent` on Bash on Windows on Ubuntu

How To
-------

Read the blog post here

http://daveeddy.com/2017/10/18/persistent-sshagent-on-bash-on-ubuntu-on-windows/

Install
-------

Put the scripts into place

    mkdir -p ~/bin
    cd ~/bin
    wget 'https://raw.githubusercontent.com/bahamas10/windows-bash-ssh-agent/master/start-ssh-agent'
    chmod a+x ./start-ssh-agent

Create a hidden scheduled task on Windows to then start this script at login

    powershell -noprofile -windowstyle hidden -command "c:\windows\system32\bash.exe -c "~/bin/start-ssh-agent""


License
-------

MIT License
