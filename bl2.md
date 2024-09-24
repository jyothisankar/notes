### Decrypt bl2 encrypted file

Whenever there are errors in bootloader then an encrypted message is given in the SE logs because disk wouldn't have been available.
That file can be decrypted using the following steps

Step-1: Goto the directory where key rings are present
zFAB-Source/src/zaci_sw/zaci_vendor_keys/zaci_gpg/vendor_keys_debug/atov

Step-2: Identify which key to be used
For this scenario we used `secring.gpg`

Step-3: Import the keyring
gpg --import secring.gpg  # To import a keyring

Step-4: To see the keys available in the key ring
gpg --list -keys # To list the keys available in a keyring

Step-5: Decrypt the key
gpg -d <file.enc> # To decrypt the file
