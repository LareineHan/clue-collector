# Clue Collector v0.1
Local-first defensive phishing URL artifact collector.

Core rule: **common infrastructure is context, not a clue.** Mailgun/Mandrill/SendGrid/DocuSign/SharePoint/Google Drive/Safe Links usage alone is never promoted as sender linkage.

Current build:
- multiple URLs
- provider recognition
- recursive percent decoding
- embedded/downstream domain extraction
- SharePoint tenant / OneDrive namespace extraction
- Google Drive/Docs resource ID extraction
- campaign/account/tenant-like named parameter candidates
- recipient/token/timestamp noise suppression
- browser-local history + repeated-artifact comparison
- no external API

Important: repeated artifacts are correlation evidence, not proof of common ownership/operator. Opaque tokens are not labeled sender IDs without supported semantics.

Open index.html directly or deploy as a static site.
