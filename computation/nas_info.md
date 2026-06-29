## Connecting instructions for macs

1. Open a finder window
2. Press ⌘+k
3. Paste in the server address smb://10.158.30.63
4. Connect
- user: tribblelab
- password: ask Carrie

When you disconnect, repeat 1&2, rest of info is stored

## ssh'ing from terminal

To ssh into the NAS from terminal, run ``ssh tribblelab@10.158.30.63`` and authenticate with same password as above. 
You will then have to cd into the correct NetBackup directory where data are stored: ``cd /var/services/NetBackup``.

## interactive browser

Using the same login information (`tribblelab` as user, specified password), you can use the [interactive browser](http://tribblenas.biology.uw.edu:5000/)
