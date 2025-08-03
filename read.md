🔒 Patch for vm2 Sandbox Escape Vulnerabilities
This repository includes a manual patch for the following critical vulnerabilities in vm2:

GHSA-cchq-frgv-rjh5 – Sandbox escape via Proxy handler

GHSA-g644-9gfx-q4q4 – Async function bypass despite allowAsync: false

🛠 How to Apply the Patch
⚠️ This is a manual patch. It will override part of the vm2 source code in your node_modules.

Install vm2 (if not already installed):

npm install vm2
Open the following file:

node_modules/vm2/lib/setup-sandbox.js
Replace its entire contents with the patched version provided here
(or paste the contents you find in patched-setup-sandbox.js from this repository).

✅ Save the file. Your vm2 sandbox is now protected against the known escape techniques.
