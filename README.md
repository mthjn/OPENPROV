# OPEN PROVENANCE 
## A Peer-to-Peer Electronic Provenance System

#####https://myveryown.org

####by Steve Douglas ( steve@myveryown.net )
####Advisor: Chris Ellis ( World Crypto Network )


#####Abstract

OPEN PROVENANCE is an original idea to establish a procedure using bitcoin(1) (vanity) addresses and PGP keys as Identities, the blockchain as a universal witness to addresses derived from SHA256 hashes, which are used as digital representations of objects, for the documentation of the processes of creation. Subsequent transactions with linked hash data can then be used to transfer ownership of objects on the blockchain which in turn creates an immutable irrefutable irrevocable digital provenance.

Proof of creation and transfer of ownership can now be done digitally without the need for trusted third parties which suffer the inherent weaknesses of the trust based model.

By asserting identities and subsequently objects on the blockchain it is possible to record proof of creation and then transfer of ownership.


#####Introduction

It is assumed you will be familiar with the following technologies: bitcoin, the blockchain, multisig and OP_RETURN transactions, Pretty Good Privacy (PGP) & Public Key Cryptography, SHA256 hashes (digital fingerprinting). 

We will also be using bitcoin vanity addresses, although not for transactions but for signatures, however they are not required and regular bitcoin address will also work just as well.

For this procedure we will use the prefix "OPENPROV" e.g. *4f50454e50524f56* in HEX for all OP_RETURN transactions that include a SHA256 hash digital fingerprint.


#####Step 1

The creator generates a PGP key pair plus a bitcoin (vanity) address (key pair) and ensures appropriate backups are available.

Self-declaration - The creator is able to declare via their website that:

*All of their works will be cryptographically signed and must be transferred using the OPEN PROVENANCE procedure as documented at https://myveryown.org.*

Generation of a vanity address shows commitment to the proof of work ethos. This vanity address is not intended to be used for transactions but is used to sign addresses that will appear in the blockchain and other text.

To create an unbreakable link between your PGP Key and your Bitcoin Vanity Address:
.
* Export your PGP Public key, add your bitcoin vanity address, sign with PGP and then sign with your bitcoin vanity address e.g. 
https://myveryown.org/pgp.txt.

This ensures the two are ouroboros.

The creator then publishes their signed bitcoin vanity address and pgp public key on their website as above along with the bitcoin/pgp signed declaration e.g. https://myveryown.org/declaration.txt 


#####Step 2

The creator documents the process of creation – e.g. using digital photography, digital video or by writing something as simple a text file. As long as it’s a digital file it can be hashed (fingerprinted). If you create something you are the first person to be able to digitise it. 

The creator can choose to optionally PGP encrypt the work in progress documentation but should include an unencrypted signed digital representation of the final piece – e.g. a photo or a video or a document. 

Encryption can optionally be used to protect trade secrets or sensitive information that can later be revealed on demand by the creator or their estate, if so desired, or required to do so e.g. in court. 


#####Step 3

The creator then creates the OPENPROV.TXT file which contains the following information:

a) Open Provenance ASCII Header (Logo and address https://myveryown.org)

b) Author Name.

c) Author Contact. e.g. email address and or bitmessage address.

NOTE: This email address should match the PGP key that is being used although that does not have to contain a valid - as in functioning - email address,  bitmessage can be used to provide additional privacy e.g. when using nyms.  If you are using bitmessage you can place your address in the comment field of the PGP key.

d) Title of Work.

e) Description of work and any other relevant information.

f) If you are working with an object that is reproducible and or made in quantity, then you must document here how many legitimate copies of that object will be made available, and if it is a digital object then list its SHA256 hash.

g) It is suggested you also include Location data e.g. Postal Address, GPS co-ordinates, Altitude, IP Address. You may wish to do the online part of this procedure at a public location e.g. a hotel or other registered business establishment(2).

h) The local date and time.

i) The OPENPROV.TXT file MUST also contain the current block height (block number), its merkle root and the block hash, as demonstrated in the World Citizenship Project by Mr Chris Ellis(2).

j) This file MUST also include a signed list of the Creation and Generation bitcoin addresses that will be used to document the moment of creation on the blockchain, and to secure the genesis provenance string. These bitcoin addresses are signed by the bitcoin (vanity) address generated in Step 1.  If you are working with a digital object then we suggest the Creation Address be derived from the objects SHA256 hash.

k) This text file should also specify that the transfer of ownership should always be carried out over the blockchain using the OPENPROV procedure described at https://myveryown.org and the transfer must include a copy of the object .ZIP/GIT file that is used in this process, if the object .ZIP/GIT file is not made public.  If the object e.g. ZIP is to be made public we suggest you publish it on IPFS(3).

IMPORTANT: This OPENPROV.TXT file is then signed with your PGP Key and bitcoin vanity address.

A blank OPENPROV.TXT template file is available from https://myveryown.org/template.zip


#####Step 4 

We suggest you include the ‘openprov.nfo’ information file plus a ‘license.txt’ file specifying legalese regarding ownership, licensing, transfer rights, etc. 

Another piece of data you could include is a 360° panoramic photo of your location and additionally a screenshot from a GPS enabled smartphone running software that is able to show on screen the stars even during daylight hours.  We are aware it is very difficult to prove a point of presence (your location), but the combination of the public location and the photos described at the time/block height declared helps to prove it as best as is possible at this time.


#####Step 5

The creator then collates all of the information from Steps 1, 2, 3 and 4 and encrypts/signs/hashes as appropriate. 

The creator then creates a single .ZIP file containing all the (encrypted) data plus the signatures and hashes.

Alternatively the creator could: 

* Create a GIT of the data include signatures and hashes within the GIT
* Publish the object on IPFS(3). 


#####Step 6

The creator then calculates the SHA256 hash of the object (.ZIP or GIT) created in Step 5 or if publishing using IPFS notes the address, as IPFS uses SHA256 hashes for addresses.


#####Step 7

The creator is of course free to place the SHA256 of the object in an OP_RETURN transaction using proofofexistance.com(4), however that process does not facilitate the subsequent transfer of the object on the blockchain.   

Another way to use the SHA256 hash of the object obtained in Step 6 would be to employ it as a private key and to then broadcast transactions to and from this bitcoin Object key pair, using the pre-signed Creation and Genesis addresses (key pairs) declared in Step 3 item j.


#####Step 8

TX A: The creator first funds the Object Creation address with enough bitcoin to cover the transaction fees that will be used to secure the moment of creation of the object on the blockchain, generate the genesis OPENPROV provenance proof of creation / ownership and finally facilitate subsequent blockchain transfer.

TX B: An initial (input) transaction made to the Object key pair obtained in Step 7 from the key funded in TX A above which causes the Object's public bitcoin address to be placed in the blockchain, and locks the moment of creation between the confirmation block and the block number noted in the OPENPROV.TXT file in Step 3.

TX C: A second (output) transaction is then broadcast from the Object key pair obtained in Step 7 including an OP_RETURN prefixed with OPENPROV and containing the SHA256 hash data, which reveals the brain wallet seed used to create the Object key pair, that was used to document the objects creation and to transfer ownership of it on the blockchain to the signed Genesis address as specified in the OPENPROV.TXT file in Step 3.

Subsequent transactions to the Object key pair are not required and are not advised, although the key pair will later be used as part of a multisig when transferring ownership.


#####Step 9

The creator (owner) is then able to transfer ownership of the object, now secured on the blockchain, at any time by using a 3 of 3 multisig transaction,  that also includes an OP_RETURN prefixed with OPENPROV and containing the SHA256 hash data in the input and output.

* Key 1 of 3 is the Genesis key that contains as an input the output from the second transaction above (or the key with the output from a previous transfer as a result of Step 12 below).
* Key 2 of 3 is the Object key derived from the SHA256 hash. 
* Key 3 of 3 is the Buyer's signing key.

Buyer and seller agree on price and method of transfer / delivery etc. Buyer and seller combine bitcoin public keys to create a multisig address and redeem script.  The buyer and seller also provide each other with the receiving addresses they would like to use for the outputs.

#####Step 10

The creator (owner/seller) then funds the agreed multi-sig with the nominal amount of bitcoin from the key pair that received the most recent OPENPROV prefixed OP_RETURN containing the SHA256 hash data. In effect transferring ownership to the multi-sig.  This funding transaction must include an OP_RETURN prefixed with OPENPROV and containing the SHA256 hash data.  E.g. in the first instance this will be from the Genesis key pair.


#####Step 11

The buyer then funds the multisig address with the agreed purchase price plus a different yet still nominal amount of bitcoin to compensate the seller for the bitcoin they have provided, and to also cover transaction fees and to ensure there is also a residual amount of bitcoin for the output transaction, which secures the object on the blockchain, and facilitates a subsequent transaction which can be used to transfer ownership.


#####Step 12

Two output transactions are then broadcast to the network as follows: 

TX 1 The agreed sale value plus a nominal amount of bitcoin is sent to the creator (owner/seller) and the change sent back to the multisig.

TX 2 The residual bitcoin is sent to the buyer along with an OPENPROV prefixed OP_RETURN including the object SHA256 hash.


####Enhancements

It is possible when working with digital objects to use the SHA256 of the object as the creation address (private key) which would provide further blockchain transparency and make identification of the provenance easier.  It is advised to then also include an  OP_RETURN when funding the Object address (Step 8 TX B) that is prefixed with OPENPROV and contains the SHA256 of the digital file. 

It is possible to use master public keys (XPUB’s) instead of the Creation and Genesis addresses in the OPENPROV.txt file so that when producing a number of copies of an object, each one can have a unique Creation and Genesis address.

If your object is a result of a collaboration then we suggest using multisig for the Creation and Genesis addresses.


###Conclusion

Subsequent transfers are performed by repeating Steps 9 through 12 inclusive, creating a new multisig each time from the current owner key / the object key / buyer key and using the nominal input/output with corresponding OPENPROV prefixed OP_RETURN SHA256 hash tracer data as described above to ensure a continuous fully linked set of transactions on the blockchain.

Proof of ownership of an object is demonstrated by being able to sign on demand using the private key that controls the most recent transacted nominal amount of bitcoin that also includes the SHA256 hash data, which can be linked back to the original creator through all previous owners via the linked transactions on the blockchain.

Previous owners are locked out of ownership claims due to subsequent transactions on the blockchain even though they may have a copy of the Object key (.ZIP/GIT file) and thieves are unable to provide the private key that controls the nominal amount of bitcoin even if they have the object and the .ZIP/GIT file.

The transactions being on the blockchain is the universe then bearing independent witness to this transfer of ownership in an irrefutable immutable and irrevocable fashion.

The transfers of the object being recorded on the blockchain automatically creates a public digital provenance of ownership that also records value at each transfer and transcends time as it will always be available to all if you know what to look for yet does not leak identity beyond the creator.

You can see within the blockchain the address most recently and legitimately associated with the SHA256 hash of an object as a result of it being transferred from its own unique address to subsequent address as a result of the transactions described above plus you are therefore able to track an object to its current owner as well as back to its creator as specified in its OPENPROV.TXT file.


###Future Work

We are seeking help promoting the use of this procedure for the benefit of all as it becomes valuable when in distributed and widespread use.

We believe this procedure can be used to help with rights management and ownership issues in the digital age however we need help and funding to develop tools for the end user.  

We are working on a custom block explorer to show in realtime OPENPROV object transactions and provide custom SHA256 search facilities.  We will also create the ability for people to claim ownership of these objects in the blockchain using bitcoin text message signing.  Ideally we would like to create an app that would facilitate the documentation of the creation and transfer of objects.

We believe the JSON data exchange format is useful and would like to create an openprov.js file that can be written/read by API’s.

We also believe Namecoin may have potential applications when it comes to identity and object data. 

We are aware that address reuse is discouraged and each time a transaction is broadcast more information is revealed, so to retain as much operational security as is possible while still transmitting multiple transactions, we suggest the two multisig output transactions are broadcast as close to simultaneously as is possible and include sufficient fees to ensure they are mined in a timely fashion.  We would ideally like to upgrade the procedure in such a way that would cause Step 12 to become atomic.

###Demonstration
Please see the demonstration file in this repo.

###References

* 1) https://bitcoin.org/bitcoin.pdf Satoshi Nakamoto Bitcoin White Paper.
* 2) https://github.com/MrChrisJ/World-Citizenship by Mr Chris Ellis.
* 3) https://gitbub.com/ipfs a new hypermedia distribution protocol.
* 4) https://www.proofofexistence.com DOCPROOF prefixed SHA256 hash OP_RETURN transactions.

###Donations & Support
If you would like to donate to the Open Provenance Project our official donation address is:
**1opDUZQ9nsL1LJALBdV1dvqSMtcvNj9EC**

If you would like to give support with your abilities please get in touch via Twitter 
**@OpenProvenance**.
