# kra-tremol-g03
Integrating the Tremol-g03 controll unit for KRA automatic reconsiliation

# Setting it to work via USB

sudo chmod 0777 /dev/ttyACM0
stty -F /dev/ttyACM0 -inlcr 115200
stty -F /dev/ttyACM0 -opost -onlcr 115200
stty -F /dev/ttyACM0 -isig -icanon -iexten -echo -echoe -echok -echoctl -echoke 115200

#Connect the ZFPLabServer to the Controll unit via USB
## setting string Settings(com=/dev/ttyACM0,baud=115200,tcp=0,ip=,port=,password=)
