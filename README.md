# InfoSec_h5


## x) Read and summarize (Some bullets per article is enough for summary) € Schneier 2015: Applied Cryptography: 10. Using Algorigthms: 10.1, 10.2, 10.3, 10.4 (from start until the start of "Dereferencing Keys" in 10.4)


### 10.1 Choosing an Algorithm

* When it comes to evaluating and choosing encryption algorithms, there are several options, including choosing a published algorithm, trusting a manufacturer or private consultant, trusting the government, or writing your own algorithm.
* Creating your own algorithm can be a solution, but it could leave room for security flaws as it has not been tested by other experts in the field.
* Trusting a single entity is problematic, so choosing a published algorithm is the most sensible option.
* It is believed that algorithms approved for export by the U.S. government can be broken by the NSA, and they may even suggest deliberate weaknesses to companies wishing to export their products.
* Relying on a company's reputation or hiring a security consultant is not a guarantee of security, since they may have limited or no knowledge of cryptography.
* To prove that the NSA can break an algorithm, it is necessary to encrypt information of great importance that is worth demonstrating that the NSA can break it.
* It is assumed that the NSA can read any message it chooses, but due to limited resources, it cannot read all messages it wants.


#### Algorithms for Export:

* Algorithms for export out of the United States must be approved by the U.S. government.
* It is widely believed that these export-approved algorithms can be broken by the NSA.
* The NSA possesses the source code for all government-approved algorithms for export.


### 10.2 Public-Key Cryptography versus Symmetric Cryptography

* The comparison of public-key cryptography and symmetric cryptography is irrelevant because they serve different purposes.
* Needham and Schroeder argued that symmetric algorithms are more efficient than public-key algorithms. However, this overlooks the security benefits of public-key cryptography.
* Whitfield Diffie suggested the adoption of a combination of systems, where public-key systems are only used for exchanging keys for symmetric cryptography.
* Symmetric cryptography is faster and better for encrypting data 
while public-key cryptography is better for key management and protocols.


### 10.3 Encrypting Communications Channels

* Encryption can take place at any layer in the OSI communications model.
* Link-by-link encryption is done at the lowest layers, and end-to-end encryption is done at higher layers.
* Link-by-link encryption encrypts everything going through a particular data link.
* End-to-end encryption selectively encrypts data until they are decrypted by the intended final recipient.

![Classes of Algorithms](1.JPG)


#### Link-by-Link Encryption:


* Link-by-link encryption is very effective, as it will encrypt all data, including the routing information and protocol information.
* This type of encryption is also called traffic-flow security since it implemented in the physical layer of the network.
* Security does not depend on any traffic management techniques. Thats why the key management is simple since only the two endpoints of the line need a common key
* The biggest problem with encryption at the physical layer is that each physical link in the network needs to be encrypted
* If the network is large, the cost may quickly become extremely high for this kind of encryption, because every node in the network must be protected
* Table 10.1 shows the process of link-by-link encryption


![Figure 10.1 Link encryption](2.JPG)


#### End-to-End Encryption:

![Figure 10.2 End-to-end encryption](3.JPG)


#### Combining the Two:



### 10.4 Encrypting Data for Storage 

![Comparing Link-by-Link and End-to-End Encryption](4.JPG)



## y) Choose a password manager. Explain: (This subtask y does not require tests with a computer if the question can be answered without them)

### What treaths does it protect against?

### What information is encrypted, what's not?

### What's the license? How would you describe license's effects or categorize it?

### Where is the data stored? If in "the cloud", which country / juristiction / which companies? If on local disk, where?

### How is the data protected?


## a) Demonstrate the use of a password manager.


## b) Encrypt and decrypt a message (you can use any tool you want, gpg is one option)


## c) Voluntary bonus: send and receive encrypted message over email.


## e) Voluntary bonus, easy: try rot13, the military grade top-secret encryption of the top-2 empire of year zero. Could double rot13 provide extra security?
