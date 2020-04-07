# split
Used to split my Alfa AWUS036NHA USB wireless adapter to run a managed interface and a monitor interface simultaneously.

# Dependencies
- A compatible wireless adapter
    - see 'Troubleshooting'
   
- Airmon-ng

    - sudo apt install aircrack-ng

# Installation
    git clone https://github.com/mcgregol/split

    cd split
    
    sudo bash install

# Usage

    sudo bash split "current_interface" "new_interface_name" 

    ex. sudo bash split wlan0 wlan1 

# Troubleshooting

If you get an error and/or the program doesn't work, run **sudo iw list** and look under **valid interface combinations**.  If you do not see **#{ managed, P2P-client } <= 2** or **#{ AP, mesh point, P2P-GO } <= 2**, etc., your wireless adapter isn't compatible.
