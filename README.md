# golang
This repository is used for How to set the Gopath for golang in our system



Step 1 – Install Go on Ubuntu

1.) wget https://dl.google.com/go/go1.13.3.linux-amd64.tar.gz      
2.) sudo tar -xvf go1.13.3.linux-amd64.tar.gz         
3.) sudo mv go /usr/local        

Step 2 - Setup Go Environment      

GOROOT is the location where Go package is installed on your system.           
1.)export GOROOT=/usr/local/go           

GOPATH is the location of your work directory. For example my project directory is ~/Projects/Proj1          

1.)export GOPATH=$HOME/Projects/Proj1          
         ex---export GOPATH=$HOME/phpexploit/src         


Now set the PATH variable to access go binary system wide.     

1.)export PATH=$GOPATH/bin:$GOROOT/bin:$PATH             

go build          
go install          


All the above environments will be set for your current session only. To make it permanent add above commands in ~/.profile or ~/.bashrc file.             

Using below command you can check go version and Goroot path   

go version        
go env   



