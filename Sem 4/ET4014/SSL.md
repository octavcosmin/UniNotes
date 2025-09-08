HTTP uses plaintext, which means that whoever captures packets can read them.
Meanwhile, **HTTPS** uses SSL/TLS encryption using a certificate.

SSL (Secure Sockets Layer) relies on public key cryptography.

## How SSL Works
1. An SSL Certificate must be obtained.
	1. XYZ creates a CSR (certificate signing request) and a private key is created.
	2. 