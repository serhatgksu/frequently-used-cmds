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
    scp -r root@43.224.34.73:/home/lk /root
    
    remoting
    ssh root@10.88.88.11
    ssh -i "xxx.pem" ubuntu@ec2-52-15-211-203.us-east-2.compute.amazonaws.com
    
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
    
