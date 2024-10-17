# Born2BeRoot
Preliminary tests
Git repo cloned successfully.

General instructions
Git repo contains a signature.txt file.

Check the signature against the students “.vdi” file, make sure it’s identical. 

Clone VM || create a snapshot && open VM.


Mandatory Part (Questions for the student)

How does a virtual machine work and what is its purpose?

The basic differences between CentOS and Debian?

Their choice of operating system?
If CentOS: what SELinux and DNF are.
If Debian: the difference between aptitude, apt and what APPArmor is.

During the defense, a script must display all information every 10 minutes. 
Its operation will be checked in detail later.

All explanations are satisfactory (else evaluation stops here).

Simple setup

Ensure that the machine does not have a graphical environment at launch.

Connect to VM as a created user (which isn’t a root)

Ensure the password follows the required policy (2 days min, 7, 30 days max).

sudo chage -l username

Evaluator checks UFW service is started.
sudo ufw status			//look for status: active

Evaluator checks SSH service is started.
sudo systemctl status ssh

Evaluator checks the chosen operating system (Debian or CentOS).
lsb_release -a || cat /etc/os-release
