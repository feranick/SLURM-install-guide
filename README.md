1. Install packages:

sudo apt install slurm-wlm-basic-plugins slurm-wlm-basic-plugins-dev slurm-wlm-doc slurm-wlm-torque slurm-wlm slurm-client

2. Configure slurm config file, following the attached file:

sudo nano /etc/slurm-llnl/slurm.conf

3. type:

slurmd -C

and replace the final line of slurm.conf with the output

4. (Re)start slurm using the file restartslurm (attached)

In case of hangs, run the following:

sudo rm -r /var/lib/slurm-llnl/slurm*
sudo restartslurm 
