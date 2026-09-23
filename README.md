# Guide Dashboard

A single static page for Alpha School guides. Open the link, sign in with your
school email and the shared password, and you get the doom-loop and accuracy
rounds for your campus.

**There is no student data in this repository.** The page ships one encrypted
blob. The key is derived from the password in your browser
(PBKDF2-HMAC-SHA256, 310,000 iterations) and the payload is AES-256-GCM. Without
the password the file is noise — nothing to read in the HTML, in the git
history, or in a cached copy.

Do not forward the link and the password outside the guide team.
