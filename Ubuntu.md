### General

    history
    history -c
    which python
    ps -ax | grep python
    ps -e | grep ssh
    ps -ef | pgrep python
    
    searching
    find / -iname svn.so
    
    content searching
    cat filename | grep keyword
    grep -R key_string
    #find . -name "*.py" | xargs cat | grep keyword
    
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
    ps -ef | grep python | awk '{print $2}' | xargs kill -9
    
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
    rm -d dirpath
    find . -name *.pyc -exec rm -f {} \;
    find . -name find-to-pattern -exec rm -rf {} \;
    
    replace
    sed -i 's/book/books/g' filename
    grep -rl matchstring somedir/ | xargs sed -i 's/searched_text/replacement_text/g'
    find . -name "*.txt" |xargs sed -i "s/searched_text/replacement_text/g"
    find . -name "ltc_timer.py" | xargs sed -i 's/DGC_/LTC_/g'
    find . -name "ltc_timer.py" | xargs sed -i 's/dgc_/ltc_/g'
    
    print
    cat $(find . -name "ltc_timer.py")
        
    edit
    vim $(find . -name "ltc_timer.py")
    
    move/rename
    mv rpc rpc_new
    rename "s/btc/bch/g"
    
    checking info
    $ sudo apt install glances
    $ glances
    $ glances
    $ lshw
    $ lscpu
    $ lsblk
    $ df -h /
    $ df -BG
    $ du -hs ~/.ethereum
    $ du -ah /home/ee
    $ lsb_release -a
    $ uname -a
    $ cat /etc/lsb-release 
    $ lspci
    $ vmstat
    
    chk&mount disk
    $ sudo fdisk -l
    $ lsblk
    $ mkdir /mnt/sdb
    $ sudo mount /dev/sdb5 /mnt/sdb/
    
    port
    ping -p 80 google.com

    time
    $ date +%s
    
    if
    if [ -d "pro/exchange" ]
    then
      echo "pro exists"
      tar cvf pro.tar.gz pro/
      mv pro.tar.gz tmp/pro_$(date +%s).tar.gz
      rm -rf pro
    else
      echo "pro doesn't exist"
    fi
    
    alias in shell script
    shopt -s expand_aliases
    source ~/.bash_aliases

    virtualbox storage expand
    VBoxManage modifyhd win10.vdi --resize 120000
    
    compress
    zip -P bitspace -r keystore.zip keystore/
    sudo apt-get install p7zip-full
    7z -pbitspace x k.zip

    account
    sudo adduser username
    sudo deluser username
    sudo visudo
    sudo usermod -l newUsername oldUsername
    sudo usermod -d /home/newHomeDir -m newUsername
    
    port scan
    nmap -p portnumber ipaddress
    nmap -p 3306 google.com
