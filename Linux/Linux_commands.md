## 10 Most Common Linux Commands 

 __xxd__ :  is a Linux command that creates a hex dump of a given file or standard input. It can also convert a hex dump back to its original binary form. 

    EX: xxd inputfile outfile 

__file__ determines the type of file 

    EX: file data.txt
    
__gzip__ compressing and decompressing files 

    EX:
        gzip file Name    --> Compressing a file 
        gzip -d fileName -- > Decompressing a file 
        
        
__tar__  combines a few files into a single file, for easy storage and distribution.

        EX: 
            tar -cvf output.tar file1.txt file2.txt file3.txt  --> combine multiple files into one tar file
            
            tar -xf output.tar    --- > to extract files from a tar file 
            
            
__ssh__    Secure Shell to connect remotely to clients or servers

         EX: 
            ssh hostName -p portNumber -i SSH_key   ----> Passing the key file to the SSH command
            
            
            
        
        
