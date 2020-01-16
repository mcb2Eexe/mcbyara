# mcbyara

A simple bash script to make yara scanning files simpler using the default yara rule packs. Designed and tested on Ubuntu 18.04. Has built in dependancy checking and installing (internet conneciton is required).

Provides a terminal menu system to select which rules to use when scanning files or directories. Also sets up a custom rule location and index for developing and testing custom rules

Simple download the script and place in a $PATH recognised location and give execution rights (chmmod +x mcbyara). 


Default installation path is $HOME/yara. Edit YARA_PATH variable to change default location if required.

Commands:

Single file: mcbyara -f <file>
Directory: mcbyara -d <dir>

Warning: Directory scanning is recursive so it is recommended that there are no child directories unless you wish them to be included in the scan.

To use the custom option, place your custom rule in the custom directory and then edit the custom_index.yar file to include the rule and you're good to go.
