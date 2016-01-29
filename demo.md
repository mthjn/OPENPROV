####Demonstration
With the exception of vanity address generation we have performed this demonstration on an inexpensive Raspberry Pi 2 computer.
For this demonstration we will be using the Open Provenance vanity address as our bitcoin signing key (1openPBE4b7hTJ5Q6oZGgaHpxG2bC2h32) and a PGP key attributed to Open Provenance (openprov@myveryown.org).  
We will use the following two bitcoin addresses for the proof of creation and genesis provenance string transactions:

**Creation Address: __1opCKbbxvesveMjTZLiBUXqxvtVGz8CQG__**

**Genesis Address: __1opGKy6dQJEjmGHc2fdRrXLX6GKsdkqqU__**

We will then transfer ownership of the object to the following addresses, to create a chain of provenance:

**Initial Purchaser: __1B1RK3FjdG4WxRMwPfG3c4tTvd58DpUr1S__**

**Subsequent Purchaser: __1B2RKXwzU2rBChZbLktELR6gL2vuu71UC9__**

The object we will work with for this demonstration is a photograph taken recently in London by Toby Connors who has kindly donated it to this project. The original raw format (.CR2) and XMP files will be PGP  encrypted and a post production (.JPG) file will be signed and can be found within the .ZIP file linked below along with the described OPENPROV.TXT and other associated files.


#####Step 1

https://myveryown.org/pgp.txt

https://myveryown.org/declaration.txt

Please see Appendices A and B  for PGP key generation and strengthening commands.  Please see Appendix C for bitcoin vanity address generation commands and Appendix D for cross signing your keys.

The following screenshots show you how to generate/verify a signature in Electrum.

https://myveryown.org/demo/screens/openprov-demo_01.jpg

https://myveryown.org/demo/screens/openprov-demo_02.jpg


#####Step 2
We then PGP encrypt the supplied .CR2 and .XMP files and sign a post production JPG copy of the photo.

https://myveryown.org/demo/london.cr2.txt

https://myveryown.org/demo/london.xmp.txt

https://myveryown.org/demo/london.jpg

https://myveryown.org/demo/london.jpg.txt

Please see Appendix E for more information on Encrypting, Signing, Verifying, Hashing and Zipping.

#####Step 3
We then create an OPENPROV.TXT file and signed it with both our PGP key and bitcoin vanity address. https://myveryown.org/demo/openprov.txt

https://myveryown.org/demo/screens/openprov-demo_03.jpg

https://myveryown.org/demo/screens/openprov-demo_04.jpg

https://myveryown.org/demo/screens/openprov-demo_05.jpg

We used the openprov.txt template file 
https://myveryown.org/template.zip


#####Step 4
Then we collate additional files: license.txt, openprov.nfo, FILE_ID.DIZ.

#####Step 5
We then hashed the data.
https://myveryown.org/demo/sha256.txt

We then made a zip of the aforementioned 11 files.
https://myveryown.org/demo/openprov.zip 

Please see Appendix E for information on zipping files.

#####Step 6
The calculated SHA256 hash of the .ZIP link in Step 5 is as follows:

*77A2BB6D9B937185B08ADA025DAB3B7A9801667288CF03BCC12E0CFAF755A88D*

#####Step 7
The bitcoin key pair generated as a result of using the SHA256 hash of our object as the private key is as follows:

Address: 1K9zXU3qoGaWYocJjPqygJrLvMcyrnaC1D

Priv Key: 5JiyWmzwnywZbk98GU8bdtfZ9o6bxBjfcuhtWVNT1wVCCh9HTFk

Pub Key: 04A4FB38F91D42B829DA25E1C9D4B182D65621DDF194ACED3C70A1105FCBC5754E003D6974088F06FE55F974E987B22B895A1FFC2496E8D519F2F4B6BC158B58E2

This key pair creates a direct representation of our object in the blockchain.

The following screen shots detail how we obtained the bitcoin address using our SHA256 hash as a private key using bitaddress.org locally. 

https://myveryown.org/demo/screens/openprov-demo_06.jpg

https://myveryown.org/demo/screens/openprov-demo_07.jpg

https://myveryown.org/demo/screens/openprov-demo_08.jpg

#####Step 8
TX A: https://blockchain.info/tx/50e30265604e888c384796675bc246f2dc9f8ed6aa9d5854bcd778765ae7feb8 

TX B: As we are working with a digital object e.g. a .JPG we are going to use part of the suggested enhancement and place its SHA256 hash prefixed with OPENPROV into the input transaction of the object key pair, e.g. 

4f50454e50524f56AAF0AE08EB31243C05A1A785C302CC4BC7A384E02F8A12FF7DA17BD33414F10B

We use coinb.in locally to 

Create 

https://myveryown.org/demo/screens/openprov-demo_09.jpg

https://myveryown.org/demo/screens/openprov-demo_10.jpg

https://myveryown.org/demo/screens/openprov-demo_11.jpg

Sign 

https://myveryown.org/demo/screens/openprov-demo_12.jpg

https://myveryown.org/demo/screens/openprov-demo_13.jpg

Verify 

https://myveryown.org/demo/screens/openprov-demo_14.jpg

https://myveryown.org/demo/screens/openprov-demo_15.jpg

Broadcast the transaction as shown.

https://myveryown.org/demo/screens/openprov-demo_16.jpg

http://coinsecrets.org/?to=393451.000036

https://blockchain.info/tx/110d97d1c56191f8592e34c28fe6f56baa21d582271467031b065e0e8c334acf?show_adv=true 

If you were working with a physical object then a standard P2PKH transaction would be sufficient.

TX C: The OP_RETURN transaction data in the output transaction and all subsequent transactions is then as follows: 

*4f50454e50524f5677A2BB6D9B937185B08ADA025DAB3B7A9801667288CF03BCC12E0CFAF755A88D*

Then again using coinb.in to create, sign, verify and broadcast the transaction.

https://myveryown.org/demo/screens/openprov-demo_17.jpg

https://myveryown.org/demo/screens/openprov-demo_18.jpg

https://myveryown.org/demo/screens/openprov-demo_19.jpg

https://myveryown.org/demo/screens/openprov-demo_20.jpg

https://myveryown.org/demo/screens/openprov-demo_21.jpg

https://myveryown.org/demo/screens/openprov-demo_22.jpg

https://myveryown.org/demo/screens/openprov-demo_23.jpg

https://myveryown.org/demo/screens/openprov-demo_24.jpg

http://coinsecrets.org/?to=393454.000004 

https://blockchain.info/tx/8fd1b973d42a87323defd2c8d2cead6ddf3d3e5397f816a934746d63371c50ed?show_adv=true 

#####Step 9
We use bitaddress locally to obtain public keys from the private keys we wish to use in the multisig.

https://myveryown.org/demo/screens/openprov-demo_25.jpg 

Then using coinb.in locally create a multisig address and redeem script.

https://myveryown.org/demo/screens/openprov-demo_26.jpg 

Please see Appendix F for the keys used to create the multisig so you are able to verify the process.

#####Step 10

The multisig address is then funded from the Genesis key and this transaction includes the same OP_RETURN data as Step 8 TX C e.g.

*4f50454e50524f5677A2BB6D9B937185B08ADA025DAB3B7A9801667288CF03BCC12E0CFAF755A88D*

We use coinb.in locally to create, sign and broadcast the transaction.

https://myveryown.org/demo/screens/openprov-demo_27.jpg

https://myveryown.org/demo/screens/openprov-demo_28.jpg 

https://myveryown.org/demo/screens/openprov-demo_29.jpg 

https://myveryown.org/demo/screens/openprov-demo_30.jpg

https://myveryown.org/demo/screens/openprov-demo_31.jpg

http://coinsecrets.org/?to=393456.000010

https://blockchain.info/tx/44fa1f4f1ecc0d92260c4acccc870ff16de307da1ce0fea7ef45432135ea4011?show_adv=true 

#####Step 11
https://blockchain.info/tx/4b6e5af733b072a2188675c5c4c7998b7138f21d0b49bb7999ed304c5bbaf0ea 

#####Step 12
Usiing coinb.in locally we create, sign, verify and broadcast the first transaction.

https://myveryown.org/demo/screens/openprov-demo_32.jpg 

https://myveryown.org/demo/screens/openprov-demo_33.jpg 

https://myveryown.org/demo/screens/openprov-demo_34.jpg 

https://myveryown.org/demo/screens/openprov-demo_35.jpg 

https://myveryown.org/demo/screens/openprov-demo_36.jpg 

https://myveryown.org/demo/screens/openprov-demo_37.jpg 

https://myveryown.org/demo/screens/openprov-demo_38.jpg 

https://myveryown.org/demo/screens/openprov-demo_39.jpg 

https://myveryown.org/demo/screens/openprov-demo_40.jpg 

https://blockchain.info/tx/83c432b5955752c56fc83a2e3b5ab9ea55e334c438bd57ca01db3860865409b7

Then we create, sign and broadcast the second transaction which includes the OP_RETURN data found in Steps 8 TX C and Step 10.

*4f50454e50524f5677A2BB6D9B937185B08ADA025DAB3B7A9801667288CF03BCC12E0CFAF755A88D*

https://myveryown.org/demo/screens/openprov-demo_41.jpg

https://myveryown.org/demo/screens/openprov-demo_42.jpg

https://myveryown.org/demo/screens/openprov-demo_43.jpg

https://myveryown.org/demo/screens/openprov-demo_44.jpg

https://myveryown.org/demo/screens/openprov-demo_45.jpg

https://myveryown.org/demo/screens/openprov-demo_46.jpg

https://myveryown.org/demo/screens/openprov-demo_47.jpg

http://coinsecrets.org/?to=393559.000001

https://blockchain.info/tx/948b4313c1e76102e0e7b6a721bdd5d6826976a61daf6bbbdb735960c4b2a1a5?show_adv=true 

#####A Subsequent Transfer
We then finally performed a second transfer of ownership by repeating Steps 9 through 12 inclusive as detailed in the transactions associated with the following address

https://blockchain.info/address/3JDkXDcc4AqzP1sUChTyte33RGCBVjqECm

The OP_RETURN data can be seen here

http://coinsecrets.org/?to=393566.000021

http://coinsecrets.org/?to=393574.000001

#####Software

https://github.com/samr7/vanitygen used to brute force bitcoin vanity addresses.

https://www.gnupg.org used to create PGP keys and binary file signatures.

https://bitaddress.org used to obtain public keys and addresses from private keys.

https://coinb.in used to create multisig and OP_RETURN transactions.

http://coinsecrets.org used to view OP_RETURN transaction data in the blockchain.

https://electrum.org used to generate bitcoin message signatures.

https://blockchain.info used to obtain blockchain block data.

https://blockr.io used to cross check blockchain data.

https://www.branah.com/ascii-converter used to convert ASCII to HEX.

#####Raspberry Pi 2 - Additional Software Setup
Ensure your raspbian installation is up to date.

pi@raspberrypi ~ $ **sudo apt-get update**

pi@raspberrypi ~ $ **sudo apt-get upgrade -y**

Then install additional software.

Electrum Bitcoin Wallet

First Install dependencies:

pi@raspberrypi ~ $ **sudo apt-get install python-qt4 python-pip**

Then install the application

pi@raspberrypi ~ $ **sudo pip install https://download.electrum.org/2.5.4/Electrum-2.5.4.tar.gz**

Iceweasel Browser

pi@raspberrypi ~ $ **sudo apt-get install iceweasel**

ZIP Compression Tools

pi@raspberrypi ~ $ **sudo apt-get install zip**


#####Appendix A - Generating a PGP Key
Please note it takes time to generate a 4096 bit key on the Raspberry Pi 2.  You will need to create entropy so we suggest you open a second SSH session to the pi and run some commands.  

Make sure to pick a long and unique passphrase. If your key gets stolen, this passphrase is the only thing protecting it!

The following commands are used: (Commands/Options are displayed in bold)

````
pi@raspberrypi ~ $ gpg --gen-key
gpg (GnuPG) 1.4.18; Copyright (C) 2014 Free Software Foundation, Inc.
This is free software: you are free to change and redistribute it.
There is NO WARRANTY, to the extent permitted by law.

gpg: directory `/home/pi/.gnupg' created
gpg: new configuration file `/home/pi/.gnupg/gpg.conf' created
gpg: WARNING: options in `/home/pi/.gnupg/gpg.conf' are not yet active during this run
gpg: keyring `/home/pi/.gnupg/secring.gpg' created
gpg: keyring `/home/pi/.gnupg/pubring.gpg' created
Please select what kind of key you want:
  (1) RSA and RSA (default)
  (2) DSA and Elgamal
  (3) DSA (sign only)
  (4) RSA (sign only)
Your selection? 1
RSA keys may be between 1024 and 4096 bits long.
What keysize do you want? (2048) 4096
Requested keysize is 4096 bits
Please specify how long the key should be valid.
            0 = key does not expire
         <n>  = key expires in n days
         <n>w = key expires in n weeks
         <n>m = key expires in n months
         <n>y = key expires in n years
Key is valid for? (0) 0
Key does not expire at all
Is this correct? (y/N) y

You need a user ID to identify your key; the software constructs the user ID
from the Real Name, Comment and Email Address in this form:
        "Heinrich Heine (Der Dichter) <heinrichh@duesseldorf.de>"

Real name: Open Provenance
Email address: openprov@myveryown.org
Comment:
You selected this USER-ID:
        "Open Provenance <openprov@myveryown.org>"

Change (N)ame, (C)omment, (E)mail or (O)kay/(Q)uit? o

You need a Passphrase to protect your secret key.

We need to generate a lot of random bytes. It is a good idea to perform
some other action (type on the keyboard, move the mouse, utilize the
disks) during the prime generation; this gives the random number
generator a better chance to gain enough entropy.

Not enough random bytes available.  Please do some other work to give
the OS a chance to collect more entropy! (Need 278 more bytes)
...............................+++++

gpg: /home/pi/.gnupg/trustdb.gpg: trustdb created
gpg: key F7CEF9F2 marked as ultimately trusted
public and secret key created and signed.
gpg: checking the trustdb
gpg: 3 marginal(s) needed, 1 complete(s) needed, PGP trust model
gpg: depth: 0  valid:   1  signed:   0  trust: 0-, 0q, 0n, 0m, 0f, 1u
pub   4096R/F7CEF9F2 2016-01-12
         Key fingerprint = C619 01FB 88D1 FF96 80B7  EFC1 6642 D6FD F7CE F9F2
uid                      Open Provenance <openprov@myveryown.org>
sub   4096R/7B35B358 2016-01-12
pi@raspberrypi ~ $
````

#####Appendix B - Strengthen the PGP Key
To improve the security of your signatures we set our key to prefer stronger hashes using the following commands: (Commands/Options are displayed in bold)

````
pi@raspberrypi ~ $ gpg --edit-key openprov@myveryown.org
gpg (GnuPG) 1.4.18; Copyright (C) 2014 Free Software Foundation, Inc.
This is free software: you are free to change and redistribute it.
There is NO WARRANTY, to the extent permitted by law.

Secret key is available.

pub  4096R/F7CEF9F2  created: 2016-01-12  expires: never           usage: SC
                        trust: ultimate          validity: ultimate
sub  4096R/7B35B358  created: 2016-01-12  expires: never           usage: E
[ultimate] (1). Open Provenance <openprov@myveryown.org>

gpg> setpref SHA512 SHA384 SHA256 SHA224 AES256 AES192 AES CAST5 ZLIB BZIP2 ZIP Uncompressed

Set preference list to:
        Cipher: AES256, AES192, AES, CAST5, 3DES
        Digest: SHA512, SHA384, SHA256, SHA224, SHA1
        Compression: ZLIB, BZIP2, ZIP, Uncompressed
        Features: MDC, Keyserver no-modify
Really update the preferences? (y/N) y

pub  4096R/F7CEF9F2  created: 2016-01-12  expires: never           usage: SC
                        trust: ultimate          validity: ultimate
sub  4096R/7B35B358  created: 2016-01-12  expires: never           usage: E
[ultimate] (1). Open Provenance <openprov@myveryown.org>

gpg> save
pi@raspberrypi ~ $
````

You are then able to export the keys for backup using the following commands:

To obtain your public key in text format use:
````
pi@raspberrypi ~ $ gpg --export -a openprov@myveryown.org > pgppublic.txt
````

To obtain your private key in text format use:
````
pi@raspberrypi ~ $ gpg --export-secret-key -a openprov@myveryown.org > pgpsecret.txt
````

#####Appendix C - Generating Vanity Bitcoin Addresses and Private Keys
As great as the Raspberry Pi 2 is, it is not really suited to brute forcing bitcoin vanity addresses.  We suggest you use a more powerful computer for this task.  

Vanitygen is available in a few flavours, there are 32 and 64 bit versions, as well as an OCL optimised version, use the best you can for maximum speed.

The exact command you will use will depend on the version you are using - here are some examples:

For the 32bit .exe the command to generate our vanity address would be as follows
````
c:\vanitygen> vanitygen 1openP
````
For the 64bit .exe the command to generate our vanity address would be as follows
````
c:\vanitygen> vanitygen64 1openP
````
For the OCL .exe the command to generate our vanity address would be as follows
````
c:\vanitygen> oclvanitygen -D 0:0 1openP
````
The -D switch is used to specify the GPU to use which in our case is 0:0.  If you do not specify which GPU to use it will show you a list of available options.

The expected output would read something like
````
Difficulty: 15318045009

[3.42 Mkey/s][total 50331648][Prob 0.3%][50% in 51.5min]
````

Once the search is complete you will see something like.  
````

Pattern: 1openP

Address:1openPBE4b7hTJ5Q6oZGgaHpxG2bC2h32

Priv Key: **************************************************
````

######Please note:  

We have replaced the private key in the above example with asterisks for security reasons.

Even with a GPU it may take some time depending on how many keys per second you are able to generate to find an address that matches your search.

#####Appendix D - Cross Signing your Bitcoin Vanity Address and PGP Key
To cross sign your PGP Key with your bitcoin vanity address, first export your PGP Public key into a file e.g.

pi@raspberrypi ~ $ **gpg --export -a openprov@myveryown.org > pgp.txt**

Then add to the top of the file your bitcoin address e.g. “Bitcoin Address: 1XXXXXXXXXXXXXXXXXXXX”

pi@raspberrypi ~ $ **nano pgp.txt**

(add your bitcoin address to the top of the file)

Press ctrl+x to exit nano, answer y to save the changes.

Then sign the file with PGP e.g.
pi@raspberrypi ~ $ **gpg --clearsign --digest-algo SHA256 pgp.txt**
This will result in a pgp.txt.asc file that contains the PGP signed, copy of your public key and bitcoin address.  Delete the pgp.txt and rename pgp.txt.asc to pgp.txt

pi@raspberrypi ~ $ **rm pgp.txt**

pi@raspberrypi ~ $ **mv pgp.txt.asc pgp.txt**

Then copy the contents of this file into the Electrum message signing dialog and click sign.  

Update the pgp.txt file with the bitcoin signature as shown and save the file.  

#####Appendix E - Encrypting, Signing, Verifying, Hashing and Zipping
Where applicable you will need to replace the email address and files names as appropriate with your own.  To encrypt data use the following commands: (Commands/Options are displayed in bold)

pi@raspberrypi ~ $ **gpg -e -a -r openprov@myveryown.org london.cr2**

This will result in a london.cr2.asc file which is a ciphertext which we rename to .txt

pi@raspberrypi ~ $ **mv london.cr2.asc london.cr2.txt**

In this case we also wish to remove the unencrypted file from this folder

pi@raspberrypi ~ $ **rm london.cr2**

We repeated the above for the london.xmp file we were also supplied.

To sign binary data use the following commands:

pi@raspberrypi ~ $ **gpg --detach-sign -a --digest-algo SHA256 london.jpg**


This will result in a london.jpg.asc signature file which we rename to .txt

pi@raspberrypi ~ $ **mv london.jpg.asc london.jpg.txt**

To sign text data use the following commands:

pi@raspberrypi ~ $ **gpg --clearsign --digest-algo SHA256 declaration.txt**

This will result in a declaration.txt.asc file which we rename to .txt

pi@raspberrypi ~ $ **rm declaration.txt**

pi@raspberrypi ~ $ **mv declaration.txt.asc declaration.txt**

To hash all files in a folder to a single text file use the following command:

pi@raspberrypi ~ $ **gpg  --print-md SHA256 *.* >> sha256.txt**

This will result in the SHA256 hash of all collated input files being added to the sha256.txt file.

To verify a signature use the following commands:

pi@raspberrypi ~ $ **gpg --verify pgp.txt**

pi@raspberrypi ~ $ **gpg --verify london.jpg.txt london.jpg**

To ZIP all files in a folder use the following command:

pi@raspberrypi ~ $ **zip openprov.zip *.***

#####Appendix F - Demonstration Addresses, Keys, Scripts and Transactions

These are the addresses, public and private keys that were used in the demonstration, and have been provided to enable you to verify our work. From this data you will be able to re- create the multi-sig addresses as seen in the demonstration transactions.

Generation Address and Public Key
1opGKy6dQJEjmGHc2fdRrXLX6GKsdkqqU

*049A782F3BD262BFAC401F7A65C9B8C29FD6B8D2DAC9E1CF94EA5BEDA33EA438198D2C09DE5B445CF7452037DB4E36BDFC8079F29548A344B9858358CD4488F814*

Object Address, Private and Public Key

Address: 1K9zXU3qoGaWYocJjPqygJrLvMcyrnaC1D

Priv Key: 5JiyWmzwnywZbk98GU8bdtfZ9o6bxBjfcuhtWVNT1wVCCh9HTFk

*04A4FB38F91D42B829DA25E1C9D4B182D65621DDF194ACED3C70A1105FCBC5754E003D6974088F06FE55F974E987B22B895A1FFC2496E8D519F2F4B6BC158B58E2*

Buyer 1 Signing Key
*047DCE5334632679DB1395A590077B32ECD43DD9A65C52CDF476937F57B7B20B4268B6E604B615968380F8EE1FC7C04493D9848F496184FF208E34E450CE99653A*

Multisig 1 Address and Redeem Script

Genesis Key, Object Key and Buyer 1 Signing Key

**3L64kHSvfPiNMkyxCKwsrWkQ5S8VMZEk1S**

*5341049a782f3bd262bfac401f7a65c9b8c29fd6b8d2dac9e1cf94ea5beda33ea438198d2c09de5b445cf7452037db4e36bdfc8079f29548a344b9858358cd4488f8144104a4fb38f91d42b829da25e1c9d4b182d65621ddf194aced3c70a1105fcbc5754e003d6974088f06fe55f974e987b22b895a1ffc2496e8d519f2f4b6bc158b58e241047dce5334632679db1395a590077b32ecd43dd9a65c52cdf476937f57b7b20b4268b6e604b615968380f8ee1fc7c04493d9848f496184ff208e34e450ce99653a53ae*

######Step 12 TX 1 Unsigned
*0100000002eaf0ba5b4c30ed9979bb490b1df238718b99c7c4c5758618a272b033f75a6e4b01000000c95341049a782f3bd262bfac401f7a65c9b8c29fd6b8d2dac9e1cf94ea5beda33ea438198d2c09de5b445cf7452037db4e36bdfc8079f29548a344b9858358cd4488f8144104a4fb38f91d42b829da25e1c9d4b182d65621ddf194aced3c70a1105fcbc5754e003d6974088f06fe55f974e987b22b895a1ffc2496e8d519f2f4b6bc158b58e241047dce5334632679db1395a590077b32ecd43dd9a65c52cdf476937f57b7b20b4268b6e604b615968380f8ee1fc7c04493d9848f496184ff208e34e450ce99653a53aeffffffff1140ea35214345efa7fee01cda07e36df10f87cccc4a0c26920dcc1e4f1ffa4400000000c95341049a782f3bd262bfac401f7a65c9b8c29fd6b8d2dac9e1cf94ea5beda33ea438198d2c09de5b445cf7452037db4e36bdfc8079f29548a344b9858358cd4488f8144104a4fb38f91d42b829da25e1c9d4b182d65621ddf194aced3c70a1105fcbc5754e003d6974088f06fe55f974e987b22b895a1ffc2496e8d519f2f4b6bc158b58e241047dce5334632679db1395a590077b32ecd43dd9a65c52cdf476937f57b7b20b4268b6e604b615968380f8ee1fc7c04493d9848f496184ff208e34e450ce99653a53aeffffffff02a0860100000000001976a914729f9a6f6b94295ca4b564faa6cb20ae33d3f1d388aca86100000000000017a914c9ce3016b24e17d3421a584716f4aabf99fa31d68700000000*

######Step 12 TX 2 Unsigned
*0100000001b70954866038db01ca57bd38c434e355eab95a3b2e3ac86fc5525795b532c48301000000c95341049a782f3bd262bfac401f7a65c9b8c29fd6b8d2dac9e1cf94ea5beda33ea438198d2c09de5b445cf7452037db4e36bdfc8079f29548a344b9858358cd4488f8144104a4fb38f91d42b829da25e1c9d4b182d65621ddf194aced3c70a1105fcbc5754e003d6974088f06fe55f974e987b22b895a1ffc2496e8d519f2f4b6bc158b58e241047dce5334632679db1395a590077b32ecd43dd9a65c52cdf476937f57b7b20b4268b6e604b615968380f8ee1fc7c04493d9848f496184ff208e34e450ce99653a53aeffffffff02983a0000000000001976a9146dc58d39001af38f575119bfd85f09f06263db5288ac00000000000000002a6a284f50454e50524f5677a2bb6d9b937185b08ada025dab3b7a9801667288cf03bcc12e0cfaf755a88d00000000*

######Step 12 TX 2 Signed
*0100000001b70954866038db01ca57bd38c434e355eab95a3b2e3ac86fc5525795b532c48301000000fda401004730440220622b1a51131d37a0ff41be52b68bfd6d3073f3d0f59ce569149433207feeb2bb02207afd9f9c4ba09b0f05d68b5407577b946d5fd975fb8207089036a3c8120fe86a01473044022079a32a52de254ea30b754599c3fba3765ca137b0003259fce63c3448cd16329402202a56eb3aec89e8de94294780881a3f8af2d120f41d93fa2d7ba942f12eba91eb0147304402201bdfd7fe450c121437d209d5256ba4e1731509847c9bf2a10e521032f070df7502206f75ce448f778ca2efe96f9c6deae046f88f83fd013762828a6a422adf39fc2c014cc95341049a782f3bd262bfac401f7a65c9b8c29fd6b8d2dac9e1cf94ea5beda33ea438198d2c09de5b445cf7452037db4e36bdfc8079f29548a344b9858358cd4488f8144104a4fb38f91d42b829da25e1c9d4b182d65621ddf194aced3c70a1105fcbc5754e003d6974088f06fe55f974e987b22b895a1ffc2496e8d519f2f4b6bc158b58e241047dce5334632679db1395a590077b32ecd43dd9a65c52cdf476937f57b7b20b4268b6e604b615968380f8ee1fc7c04493d9848f496184ff208e34e450ce99653a53aeffffffff02983a0000000000001976a9146dc58d39001af38f575119bfd85f09f06263db5288ac00000000000000002a6a284f50454e50524f5677a2bb6d9b937185b08ada025dab3b7a9801667288cf03bcc12e0cfaf755a88d00000000*

Buyer 1 Receiving Address and Public Key

1B1RK3FjdG4WxRMwPfG3c4tTvd58DpUr1S

*045BE4A3305E201F917C9A7514D7B747F5B18DA9B7AEFB603DB37DC3981436216EF134556F91B58F2FDFD55442404B231C85AA9CB7D889FCA4C3C0A1316BD5A2DC*

Buyer 2 Signing Key

*049994BE3450927A9DECE42AFC902B56E8EBABAA3BA49F269109E89BD4D954CEFAC470A68E833EC7B94BE20969E4B4E700FA833981717CE35D66DCF6DD50C63FAC*

Multisig 2 Address and Redeem Script


Buyer 1 Receiving Key, Object Key and Buyer 2 Signing Key

**3JDkXDcc4AqzP1sUChTyte33RGCBVjqECm**

*5341045be4a3305e201f917c9a7514d7b747f5b18da9b7aefb603db37dc3981436216ef134556f91b58f2fdfd55442404b231c85aa9cb7d889fca4c3c0a1316bd5a2dc4104a4fb38f91d42b829da25e1c9d4b182d65621ddf194aced3c70a1105fcbc5754e003d6974088f06fe55f974e987b22b895a1ffc2496e8d519f2f4b6bc158b58e241049994be3450927a9dece42afc902b56e8ebabaa3ba49f269109e89bd4d954cefac470a68e833ec7b94be20969e4b4e700fa833981717ce35d66dcf6dd50c63fac53ae*

#####E&OE
Errors and omissions excepted

####Donations & Support
If you would like to donate to the Open Provenance Project our official donation address is:

**1opDUZQ9nsL1LJALBdV1dvqSMtcvNj9EC**

If you would like to give support with your abilities please get in touch via Twitter 
**@OpenProvenance**.
