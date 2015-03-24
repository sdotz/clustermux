#Clustermux
Clustermux generates parallel ssh connections with synchronized tmux panes for arbitrary sets of servers. It is useful if you need to execute commands synchronously across a large number of servers.


##Usage
###Create your inventory
inventory.yaml is where you will specify servers you'd like to connect to. See the example, and create your own. 

###Connect
Once you have an inventory, using it is simple. Make sure you are in a tmux session.

`clustermux -s myapp.prd.app`

You can also specify the inventory.yaml path

`clustetmux -i ~/myinv.yaml -s myapp.prd.app`

Specify a higher node in the yaml to get all the servers under it.

`clustermux -s myapp.prd`

###That's it!
