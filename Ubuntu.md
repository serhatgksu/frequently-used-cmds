### General

    history
    history -c
    which python
    ps -ax | grep python
    ps -e | grep ssh
    find / -iname svn.so
    
    systemctl status httpd.service
    journalctl -xe
    
    porting
    $ netstat -apn | grep 3690
    $ netstat -plunt
    $ sudo nmap -PN -p port_number -sN remote_host
    $ sudo nmap -p port_number remote_host
    $ sudo nmap -n remote_host
    
    processing
    kill -9 10203
    pkill svnserve
    
    compressing
    tar -xvf a.tar.gz
    tar -cvf sv.tar.gz /home/username/sv
    
    copying
    scp -i xxxx.pem ubuntu@x.x.x.x:/home/ubuntu/data/vac/vacd .
    ssh -x -oForwardAgent=no -oPermitLocalCommand=no -oClearAllForwardings=yes -i xxx.pem -l ubuntu -- x.x.x.x scp -f /home/ubuntu/data/vac/vacd
    
    remoting
    ssh root@x.x.x.x
    ssh -i "xxx.pem" ubuntu@ec2-x-x-x-x.us-east-2.compute.amazonaws.com
    scp -i vachain_for_test.pem ubuntu@x.x.x.x:/home/ubuntu/data/vac/vacd .
    
    background running
    meld&
    
    permanent running
    nohup python server.py &
    nohup geth console > /dev/null 2>&1 &
    
    checking info
    $ sudo apt install glances
    $ glances
    $ glances
    $ lshw
    $ lscpu
    $ lsblk
    $ df -h /
    $ du -hs ~/.ethereum
    $ du -ah /home/ee
    $ lsb_release -a
    $ lspci
    $ vmstat
    
