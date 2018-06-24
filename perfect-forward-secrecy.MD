## What is perfect forward secrecy?
In cryptography, forward secrecy (FS), also known as perfect forward secrecy (PFS), is a feature of specific key agreement protocols that gives assurances **your session keys will not be compromised even if the private key of the server is compromised.**\
Forward secrecy protects past sessions against future compromises of secret keys or passwords. **By generating a unique session key for every session** a user initiates, even the compromise of a single session key will not affect any data other than that exchanged in the specific session protected by that particular key. 
Forward secrecy further protects data on the transport layer of a network that uses common SSL/TLS protocols, including OpenSSL




You canuse these new security features with AWS ELB:

### Perfect Forward Secrecy 
is a feature that provides additional safeguards against the eavesdropping of encrypted data, through the use of a unique random session key. This prevents the decoding of captured data, even if the secret long-term key is compromised.

### Server Order Preference
lets you configure the load balancer to enforce cipher ordering, providing more control over the level of security used by clients to connect with your load balancer.

### Predefined Security Policy 
simplifies the configuration of your load balancer by providing a recommended cipher suite that adheres to AWS security best practices. The policy includes the latest security protocols (TLS 1.1 and 1.2), enables Server Order Preference, and offers high security ciphers such as those used for Elliptic Curve signatures and key exchanges.
You can configure these new features with the AWS Management Console, API, or Command Line Interface (CLI).
## References
https://en.wikipedia.org/wiki/Forward_secrecy

https://docs.aws.amazon.com/elasticloadbalancing/latest/classic/elb-ssl-security-policy.html
