<h1>PIX3L PLOTT3R Web Interface</h1>

The ev3 printer now has a web interface where you can type text and draw!

This has been tested using Firefox on Ubuntu.



*   Prerequisites (Ubuntu):
*   
        sudo apt-get update
        sudo apt-get upgrade
        sudo apt-get install apache2 sshpass

*   The ev3dev version should be the latest. To upgrade:

        sudo apt-get dist-upgrade


*   Download this folder (Ubuntu):
*   
        git clone https://github.com/droidsrobotics/ev3dev.git
        cd ev3dev/PIX3L\ PLOTT3R/server
        cp home_ubuntu/* ~/
        sudo cp -r www_ubuntu/* /var/www/html/

*   Download this folder (EV3):
<br><code>        git clone https://github.com/droidsrobotics/ev3dev.git
</code><br><code>        cd ev3dev/PIX3L\ PLOTT3R/server
</code><br><code>        cp ev3_home/* ~/
</code>

You will need to replace <code>192.168.43.22</code> in printer.py with the ev3's ip address
You will also need to replace <code>robot</code> and <code>maker</code> in printer.(py)/(sh) with your ev3 username and password.
(printer.py is on the Ubuntu computer and printer.sh is on the ev3)
*   Run Code (Ubuntu):
  
        cd ~/
        python printer.pybr
        Go to http://localhost/ in Firefox

Note: If you do not want to use your own server (apache2) use this url: http://www.droidsrobotics.org/ev3dev/PIX3L%20PLOTT3R/server/www_ubuntu/