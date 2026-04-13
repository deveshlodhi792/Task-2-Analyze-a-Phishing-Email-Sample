Examining the Sender's Email:-
-
To identify the phishing characteristics of email, we have to start with examining the Sender's email:-
  - In the screenshot above we can see that, the email is a notification sended by the Open AI regarding Subscription.
  - We can see that the Display name of organization is OpenAI ServiceStatus but the actual domain behind display name is <mark>sage.develop@msa.hinet.net</mark>.
  - The genuine domain responsible for OpenAI service status is <mark>https://status.openai.com</mark>(reference <a href="https://help.openai.com/en/articles/11725090-verifying-communications-from-openai">website</a>).
  - It suggests that the email is compromised as it is not from authentic domain.
  - The sender here trying masquerade technique.
  - The Display name term "ServiceStatus" which is formatted improperly or typo, it also a strong indicator or potential phishing attacker.
  - All these indicators suggest that the sender is a spoof of OpenAI Service Status.




Checking Email Header:-
-

-   We have divided headers into four categories to check for discrepancies:-
    1. Authentication-related headers
    2. Sender Identity headers
    3. Routing headers
    4. Content-related headers
 
-  First we look on Authentication headers:
    + SPF (Sender Policy Framework): This protocol verifies that the sending mail server whether authorized or not.
    + DKIM (Domain Keys Identified Mail): This protocol ensures the email content has not been altered and verifies the sender's domain via cryptographic signature.
    + DMARC (Domain-based Message Authentication, Reporting & Conformance) : This protocol ties SPF and DKIM together and defines policies for handling failed authentication.
    + After analyzing using MX Toolbox header analyzer, here are the results:
      - SPF = Pass
      - DKIM = Pass
      - DMARC = Pass
  
- Sender's Identity header:
    + After analyzing the email by MX Toolbox header analyzer, these details are found :-
      - From: 


