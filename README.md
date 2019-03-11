# MN-Setup Guide (Follow below Steps)

1) If --------------------------------
you want to mantain your actual bithost.conf file because have just set as masternode use:

> wget -q https://raw.githubusercontent.com/nur0m/BitHost-MN-Setup/master/bithostinstall.sh
> sudo chmod +x bithostinstall.sh
> ./bithostinstall.sh

and go to step 3

2) Else if -------------------------------------
you want install from zero with automatic config file creation for masternode use:

> wget -q https://raw.githubusercontent.com/nur0m/BitHost-MN-Setup/master/bithostinstall-create-config.sh
> sudo chmod +x bithostinstall-create-config.sh
> ./bithostinstall-config-create.sh

When prompted to Enter your bithost Masternode GEN Key.
Paste your Masternode GEN Key and press enter

3) ----------------------------------------------------------

Wait till Node is fully Synced with blockchain.
Wait until the script end.

For start the node:

> systemctl start bithost.service
> systemctl enable bithost.service

For check enter below command.
> bithost-cli getinfo

When Node Fully Synced enter below command for check masternode status.
> bithost-cli masternode status
