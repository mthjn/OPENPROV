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


####Donations & Support
If you would like to donate to the Open Provenance Project our official donation address is:

**1opDUZQ9nsL1LJALBdV1dvqSMtcvNj9EC**

If you would like to give support with your abilities please get in touch via Twitter 
**@OpenProvenance**.
