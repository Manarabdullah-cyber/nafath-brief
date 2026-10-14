Version: NAFATH-V3

Your track: Cybersecurity

Overview
A dependable public-service AI assistant relies on six interconnected technological domains. Software engineering uses versioning rules to help developers release updates safely. Artificial intelligence applies Retrieval-Augmented Generation (RAG) to retrieve relevant information before generating responses. Mobile security protects data transmission between applications and servers. Networking supports communication through IPv4 and IPv6 as connected devices increase. Cybersecurity protects the assistant against threats that could compromise its reliability. Data protection practices help ensure that conversation records are handled responsibly and users’ privacy is protected. Together, these disciplines help make the service secure, scalable, and trustworthy. The cybersecurity topic focuses on prompt injection, a threat that can manipulate an AI assistant’s behavior, and methods to reduce this risk.

Software
Semantic Versioning (SemVer) employs a MAJOR.MINOR.PATCH structure to communicate software changes. The MAJOR version is incremented when a change introduces incompatibility with the public API. The MINOR version is incremented when new functionality is added without breaking existing compatibility. The PATCH version is incremented when backward-compatible bug fixes are released. Following these guidelines helps developers and API consumers understand the impact of updates and manage dependencies more safely.

Resource: Semantic Versioning 2.0.0 - https://semver.org/spec/v2.0.0.html

AI
Retrieval-Augmented Generation (RAG) combines information retrieval with artificial intelligence language models to improve response quality. The system retrieves relevant information from a trusted knowledge source and provides it as context to the model before generating a response. This approach can reduce inaccurate answers by grounding responses in supporting evidence rather than relying solely on the model’s pre-trained knowledge. However, RAG cannot eliminate errors completely, so both retrieved information and generated responses should be evaluated and verified.

Resource: Retrieval-Augmented Generation (RAG) - https://youtu.be/v4s5eU2tfd4?si=owK3yYJzDPvjACER

Mobile
App Transport Security (ATS) is an iOS security feature that requires network connections to meet specified security standards, including HTTPS with appropriate Transport Layer Security (TLS) settings. When an application attempts to connect to a plain HTTP endpoint without an applicable exception, ATS generally blocks the connection. Developers should prioritize HTTPS endpoints and avoid unnecessary ATS exceptions to reduce the risk of exposing data transmitted between the application and its server.

Resource: Preventing Insecure Network Connections - https://developer.apple.com/documentation/security/preventing-insecure-network-connections

Networking
IPv4 and IPv6 are versions of the Internet Protocol that allow devices to communicate across networks. IPv4 uses 32-bit addresses, while IPv6 uses 128-bit addresses and provides a much larger address space. IPv6 helps address the shortage of available IPv4 addresses as connected devices and online services grow. However, IPv4 remains widely used, so many networks support both protocols.

Resource: IPv4 and IPv6 Addressing - https://www.cloudflare.com/learning/dns/glossary/what-is-my-ip-address/


Cybersecurity
Prompt injection occurs when malicious instructions try to make an AI system ignore its intended rules or produce unsafe responses. Direct prompt injection comes from user input, while indirect prompt injection can be hidden in external content, such as websites or documents. Mitigations include separating trusted instructions from untrusted content, limiting tool permissions, and checking sensitive actions. These defenses reduce risk but cannot guarantee complete protection.

Resource: Prompt Injection - https://genai.owasp.org/llmrisk/llm01-prompt-injection/

Data
Anonymization and pseudonymization are different ways to protect personal data. Anonymization removes identifying information so that a person cannot reasonably be identified. Pseudonymization replaces direct identifiers with values such as codes, but additional information may still reveal the person’s identity. Therefore, pseudonymized data generally remains personal data and needs protection, while properly anonymized data may no longer fall under personal-data rules, depending on the applicable law.

Resource: What is personal data? - https://commission.europa.eu/law/law-topic/data-protection/data-protection-explained_en

My Track: Misconception
A common misconception is that prompt injection vulnerabilities can be completely prevented by using clearly defined system instructions. In practice, malicious instructions may come directly from user input or indirectly from external sources, such as websites and documents. An AI model may struggle to distinguish trusted instructions from untrusted content. Developers should therefore apply defense in depth by separating instructions from retrieved content, limiting tool permissions, and validating sensitive actions. These measures can reduce the likelihood and impact of attacks, but they cannot guarantee complete protection. OWASP discusses this vulnerability in its “Prompt Injection” guidance.

Resource: Prompt Injection - https://genai.owasp.org/llmrisk/llm01-prompt-injection/

Open Question
How can public-service AI assistants provide useful responses while protecting citizens from malicious inputs, unreliable external information, and privacy risks?
