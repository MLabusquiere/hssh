#SSH env Handler

SSH env Handler is a Bash Tool to handle environement composed with several host
using command line.


##Functionality 

- Transform a csv file to a ssh config file 
- Switch between different config file (each representig a env for example) 
- Print a ssh config file in a human readable format 

##Usage 

./hssh print (<env>)
./hssh switch <env>
./hssh parse <env_name> <file|-> <suffix_QUALIFIED_NAME> 
	     [ -f -u <default_username> -q <hostname_end> ]
./hssh help|-h|--help

print  : print the 'env' or list all env name
switch : will switch the current env to 'env' 
parse  : will parse the csv and create a new 
	 config file with the name 'env' 
	 -f : override an existing env
	 -u : add to all Host a default username
	 -q : add at the arg at the end of the hostname
csv format : aliases;hostname;username

##Dev

Tests exist :
./hssh test
