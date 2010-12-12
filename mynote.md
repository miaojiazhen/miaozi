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

