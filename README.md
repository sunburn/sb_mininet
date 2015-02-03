# sunburn

## Quick Start Dev Environment

1.  Download and install Vagrant.
2.  Download and install Virtualbox.
3.  Download and install XQuartz (if no other X11 client).
4.  Clone this repo and run as follows:

```
git clone http://github.com/sunburn/sb_mininet
vagrant up
vagrant ssh
sudo python mininet/examples/miniedit.py --topo=tree,3
```

If all goes to plan you should see the MiniEdit GUI pop up in an X11 window.  
Move the switches (the squares with the OpenFlow logos on them) around and see 
the network that this has built for you.  

## Using the Mininet GUI

1. Run the network by clicking `Run` in the bottom left corner.
2. Log into a host and run some linux (i.e. `ping 10.0.0.4`) commands by right clicking on a host.