### General

    history
    history -c
    which python
    ps -ax | grep python
    ps -e | grep ssh
    
    searching
    find / -iname svn.so
    
    content searching
    cat filename | grep keyword
    
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
    unzip
    
    copying
    chmod 400 x.x.x.x.pem
    scp -i x.x.x.x.pem ./interface/rpc.tar.gz ubuntu@ec2-x-x-x-x.ap-northeast-2.compute.amazonaws.com:~/
    scp -i x.x.x.x.pem -r ./interface/rpc ubuntu@ec2-x-x-x-x.ap-northeast-2.compute.amazonaws.com:~/
    
    remoting
    ssh root@x.x.x.x
    ssh -i "xxx.pem" ubuntu@ec2-x-x-x-x.us-east-2.compute.amazonaws.com
    
    background running
    meld&
    
    permanent running
    nohup spyder
    nohup python server.py &
    nohup python server.py > ./log.out 2>&1 &
    nohup geth console > /dev/null 2>&1 &
    
    account
    sudo adduser username
    sudo passwd username
    
    environment variable
    alias surf='find / -name'
    export name=smith
    $ vim ~/.bashrc
    $ source ~/.bashrc
    
    removing file/dir
    rm -rf dirpath
    
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
    
