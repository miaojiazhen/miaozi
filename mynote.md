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
