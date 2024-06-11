# OSWAP-MOBILE-TOP-10-2024


## M1: Improper Credential Usage
### Summary
Many applications do not store credentials safely, often storing them in plain text or within the source code. This makes it easy to decompile applications and retrieve sensitive information using tools like `jadx`.

### Attack Vectors
- **Exploitability:** Easy
- Attackers can use hardcoded credentials to gain unauthorized access once identified.

### Security Weakness
- **Detectability:** Easy
- Improper credential storage can be identified through proper testing.

### Technical Impacts
- **Impact:** Severe
- Unauthorized users can access sensitive information, leading to privacy loss, fraud, etc.

### Business Impacts
- **Reputation Damage**
- **Information Theft**
- **Fraud**
- **Unauthorized Access**

### Prevention
- Avoid hardcoding credentials.
- Encrypt sensitive information properly.
- Ensure secure storage of credentials.
- Regularly update API keys and tokens.

## M2: Inadequate Supply Chain Security
### Summary
Developers often use libraries that can be easily exploited. Attackers can inject malicious code during the development phase, allowing data theft, user spying, or mobile device control.

### Attack Vectors
- **Exploitability:** Average
- Vulnerabilities in third-party libraries or during the development phase.

### Security Weakness
- **Detectability:** Difficult
- Due to lack of secure coding practices and weak testing.

### Technical Impacts
- **Impact:** Severe
- Can lead to stealing sensitive information, unauthorized access, malware infection, and system compromise.

### Business Impacts
- Financial loss
- Reputation damage
- Supply chain disturbance

### Prevention
- Secure coding practices
- Use trusted libraries and components
- Implement proper security controls

## M3: Insecure Authentication/Authorization
### Summary
Automated attacks target authentication and authorization weaknesses, allowing attackers to bypass controls or log in as legitimate users.

### Attack Vectors
- **Exploitability:** Easy
- Directly submitting requests to the backend server or logging in as legitimate users.

### Security Weakness
- **Detectability:** Average
- Testers can perform binary attacks and use POST/GET requests to backend servers.

### Technical Impacts
- **Impact:** Severe
- Over-privileged execution, unauthorized access to sensitive information, difficulty tracing attacks.

### Business Impacts
- **Reputation Damage**
- **Information Theft**
- **Fraud**
- **Unauthorized Access**

### Prevention
- Avoid “Remember Me” functionality
- Avoid 4-digit PINs
- Encrypt data stored on the client side
- Use FaceID or TouchID with additional security checks
- Backend should verify user roles and permissions

## M4: Insufficient Input/Output Validation
### Summary
Failing to validate inputs and outputs can lead to SQL injection, XSS, data corruption, and the injection of malicious code.

### Attack Vectors
- **Exploitability:** Difficult
- Can result in unauthorized access, data manipulation, and backend system compromise.

### Security Weakness
- **Detectability:** Easy
- Insufficient input/output validation and contextual validation.

### Technical Impacts
- **Impact:** Severe
- Data breaches, system compromise, code execution, reputation damage, legal issues.

### Business Impacts
- Data breaches
- System disruption
- Financial impact
- Legal consequences

### Prevention
- Proper input/output validation
- Data integrity checks
- Secure coding practices
- Comprehensive security testing

## M5: Insecure Communication
### Summary
Data transmitted between mobile apps and servers can be intercepted and modified if not properly secured.

### Attack Vectors
- **Exploitability:** Easy
- Easily monitored on local networks.

### Security Weakness
- **Detectability:** Average
- Inconsistencies in data transmission security.

### Technical Impacts
- **Impact:** Severe
- PII leaks, intercepted user credentials.

### Business Impacts
- Identity theft
- Fraud
- Reputational damage

### Prevention
- Apply SSL/TLS to transport channels
- Use certificates from trusted CA providers
- Avoid sending sensitive data over insecure channels
- Avoid plain text transmission

## M6: Inadequate Privacy Controls
### Summary
Inadequate controls on PII can lead to fraud, blackmail, and misuse of payment data.

### Attack Vectors
- **Exploitability:** Average
- Attackers can eavesdrop on networks, file systems, and logs.

### Security Weakness
- **Detectability:** Easy
- Excessive collection of PII increases attractiveness for attackers.

### Technical Impacts
- **Impact:** Minimal on system but significant privacy violations.

### Business Impacts
- Legal violations
- Financial damage
- Reputational damage
- PII theft

### Prevention
- Minimize PII processing
- Secure storage of information
- Regular security checks (static and dynamic)

## M7: Insufficient Binary Protections
### Summary
Attackers target app binaries for valuable information or to manipulate app behavior, including injecting malicious code.

### Attack Vectors
- **Exploitability:** Easy
- Reverse engineering and code tampering.

### Security Weakness
- **Detectability:** Easy
- All apps are vulnerable, especially those with hardcoded sensitive data or algorithms.

### Technical Impacts
- **Impact:** Moderate
- Reverse engineering and code manipulation.

### Business Impacts
- Misuse of API information
- Theft of algorithms or AI models
- Reputational damage

### Prevention
- Obfuscate app binaries
- Secure sensitive data
- Implement robust security checks

## M8: Security Misconfiguration
### Summary
Improper configuration of security settings and permissions can lead to unauthorized access and data breaches.

### Attack Vectors
- **Exploitability:** Difficult
- Includes improper encryption, insecure communication, and insecure storage.

### Security Weakness
- **Detectability:** Easy
- Automated scanning tools can detect misconfigurations.

### Technical Impacts
- **Impact:** Severe
- Unauthorized access to sensitive data, account hijacking, data breaches.

### Business Impacts
- Financial and data loss
- Reputation damage
- App downtime

### Prevention
- Review and secure default configurations
- Limit unnecessary permissions
- Disable backup mode
- Avoid default credentials

## M9: Insecure Data Storage
### Summary
Data stored on mobile devices can be easily accessed if not properly secured, leading to identity theft, fraud, and reputational damage.

### Attack Vectors
- **Exploitability:** Easy
- Attackers can physically access mobile devices.

### Security Weakness
- **Detectability:** Average
- File systems are often accessible and rooted/jailbroken devices can bypass protections.

### Technical Impacts
- **Impact:** Severe
- Full access to sensitive information on the device.

### Business Impacts
- Identity theft
- Fraud
- Reputation damage
- Policy violations (e.g., PCI)
- Material loss

### Prevention
- Assess and secure information assets
- Ensure proper handling of caching, backgrounding, logging, and data storage
- Encrypt sensitive information

## M10: Insufficient Cryptography
### Summary
Weak cryptography can compromise the confidentiality, integrity, and authenticity of sensitive information.

### Attack Vectors
- **Exploitability:** Average
- Exploiting weaknesses in encryption algorithms, key management, or implementation flaws.

### Security Weakness
- **Detectability:** Average
- Weak algorithms, inadequate key lengths, poor key management, flawed implementation.

### Technical Impacts
- **Impact:** Severe
- Unauthorized retrieval of sensitive information.

### Business Impacts
- Data breaches
- Loss of intellectual property
- Financial losses
- Compliance issues

### Prevention
- Use strong encryption algorithms (e.g., AES, RSA, ECC)
- Ensure sufficient key length
- Follow secure key management practices
- Implement encryption correctly
- Secure storage of encryption keys
- Employ secure transport layers (e.g., HTTPS)
- Validate and authenticate parties involved in encryption
- Regularly update security measures
- Conduct security testing
- Follow industry standards and best practices
- Use strong hash functions (e.g., SHA-256, bcrypt)
- Implement salting for password hashing
- Use Key Derivation Functions (KDFs) like PBKDF2, bcrypt, or scrypt

---

