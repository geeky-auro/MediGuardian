# MediGuardian
MediGuardian is an advanced software tool designed to identify, analyze, and protect sensitive data that could potentially lead to the identification of individuals. It utilizes sophisticated algorithms and pattern recognition techniques to scan through vast amounts of data, searching for specific markers or formats that resemble personally identifiable information.

The primary purpose of a MediGuardian is to safeguard sensitive information such as social security numbers, driver's license numbers, credit card details, addresses, and other confidential data that, if exposed, could lead to identity theft, fraud, or privacy breaches.

The detection process involves various steps, including data classification, pattern matching, and contextual analysis. It works across multiple file formats, databases, and communication channels, employing both rule-based systems and machine learning models to recognize PII accurately.

Once potential PII is identified, the detector can take several actions, including encryption, masking, redaction, or flagging the data for further review by authorized personnel. Some advanced PII Detectors also offer real-time monitoring and alerts to notify administrators of any potential breaches or unauthorized access attempts.

Organizations across different sectors, including finance, healthcare, government, and technology, employ PII Detectors to comply with data protection regulations like GDPR, HIPAA, or CCPA. These tools play a crucial role in ensuring data privacy and security, helping organizations mitigate risks associated with mishandling sensitive information and maintaining trust with their customers and stakeholders.

## Task
Implementation Gen AI to automatically identify and safeguard personally identifiable information from being inadvertently shared with language models. 

## Data Collection and Processing
For the capstone project on implementing Gen AI to automatically identify and safeguard personally identifiable information (PII) from being shared with language models, consider the following steps:
1. Data Acquisition:
The project begins with obtaining medical reports or documents in digital
format, often in PDF or other standardized formats.
2. Reading and Extraction:
Using the PyPDF2 library, the code reads the medical reports and extracts
text from the initial pages.
This text extraction process allows the code to access and work with the
content of the medical reports programmatically.
3. Preparing for Anonymization:
The extracted text undergoes a pre-processing phase to prepare it for
anonymization.
This step involves cleaning the text and ensuring it is in a format suitable for
further analysis.
4. Anonymization Process:
The code utilizes the Presidio library, developed by Microsoft, for
anonymization purposes.
Presidio employs pattern recognition techniques to identify and mask
sensitive information such as names, addresses, and specific IDs within the
medical reports.
5. Advanced Anonymization Techniques: Various predefined recognizers and custom recognition patterns are used to
comprehensively identify and mask sensitive data.
Recognizers specialized in identifying titles, addresses, or custom-defined PII
parameters ensure a thorough anonymization process.
6. Mapping and Deanonymization:
The code maintains a mapping of anonymized data to its original form,
allowing for deanonymization if necessary.
This mapping ensures the ability to retrieve the original data from the
anonymized content when needed.
7. Enhancing Data Protection:
Incorporation of faker operators adds another layer of data security by
replacing sensitive data with realistic, yet fake, information.
This step ensures that even if original data is required for testing or
demonstration, it remains protected.
8. Conclusion:
The data collection and processing phase primarily focus on acquiring
medical reports, extracting relevant information, and anonymizing sensitive
data to protect patient privacy.
The process sets the foundation for secure and ethical handling of medical
information, ensuring compliance with data protection regulations while
enabling subsequent analysis and summarization.
