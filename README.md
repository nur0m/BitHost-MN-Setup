# MN-Setup Guide (Follow below Steps)

1) If --------------------------------

you want to mantain your actual bithost.conf file because have just set as masternode use:

prompt#: wget -q https://raw.githubusercontent.com/nur0m/BitHost-MN-Setup/master/bithostinstall.sh
prompt#: sudo chmod +x bithostinstall.sh
prompt#: ./bithostinstall.sh

and go to step 3

2) Else if -------------------------------------

you want install from zero with automatic config file creation for masternode use:

prompt#: wget -q https://raw.githubusercontent.com/nur0m/BitHost-MN-Setup/master/bithostinstall-create-config.sh
prompt#: sudo chmod +x bithostinstall-create-config.sh
prompt#: ./bithostinstall-config-create.sh

When prompted to Enter your bithost Masternode GEN Key.
Paste your Masternode GEN Key and press enter

3) ----------------------------------------------------------

Wait till Node is fully Synced with blockchain.
Wait until the script end.

For start the node:

prompt#: systemctl start bithost.service
prompt#: systemctl enable bithost.service

For check enter below command.
prompt#: bithost-cli getinfo

When Node Fully Synced enter below command for check masternode status.
prompt#: bithost-cli masternode status
