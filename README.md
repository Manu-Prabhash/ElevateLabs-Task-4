# ElevateLabs-Task-4
I use Kali Linux and the UFW was not installed in my OS. so i used '''sudo apt install ufw -y''', which helped me install ufw.
'''sudo ufw enable''' for activating firewall
'''sudo ufw status numbered''' for seeing active rules.
'''sudo ufw deny in proto tcp to any port 23''' we use this inorder to block incoming traffic to TCP port 23(telnet)
'''sudo ufw allow 22/tcp''' to make sure SSH stays allowed
and finally '''sudo ufw delete deny in proto tcp to any port 23''' to return back to original state.
So the firewalls  inspect packets and decide whether to allow them or deny them based on the protocols used.
