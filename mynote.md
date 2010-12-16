# How to make bash
    vim markdown.sh
        #!/bin/bash
        markdown file.md > file.html
        firefox file.html &
    chmod +x file.sh
    mv file.sh /bin      //became system command

#command
## %s                substitute
    %s /****/substitute content/g
    %s /****/substitute content/gc    //zhugequeren 
    %s /\/home\/hushengjie/miao/g     //example
## which 
    which file.sh        //look over file path
    --'xp'--to exchange two char
    --'rc'--change the char in front of the cursor to 'c'
## firefox
    '/' to start search
    __ctrl+g__  find next
    __ctrl+c+l__   change URL
    __ctrl+r__     refresh
    __ctrl+k__     to google
# creat a tar ball
    tar zcvf toy.tgz toy
    tar zxvf toy.tgz
# stop a process by force
    ps aux|grep firefox
    kill -9 [the process number of firefox]
    or we can kill by name
    killall firefox
# about bash
    #!/bin/bash
    for file in a b c d;
    do
        echo $file            //bash is very sensitive to space
    done
## "a.c"->"a"
    #!/bin/bash
    WOKDIR=$1
    CD $WOKDIR
    for file in `ls`;
    do
        f=`echo $file|awk -F'.' '{ print $1 }'`
        mv $file $f
    done;
## How to usage 'if' in bash
    test -f hello.h           
    echo $?                     //if have a hello.h ,put out 0

    #!/bin/bash
    if [ -f a ]
    then
        mv a a.c
    fi
    
