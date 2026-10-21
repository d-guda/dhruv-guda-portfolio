# Assessment Limitations and Control Review

The risk register preserves early proposed controls, including wording that needs refinement. The review below identifies conceptual limitations and recommended corrections; no company controls were implemented.

| Entry or area | Problem | Recommended correction |
| --- | --- | --- |
| ID 1: phones | Confusing passcode encryption wording | Describe device encryption, strong local unlock protection, managed access, and revocation separately. |
| ID 2: badges | Proposal refers to lost laptops | Correct the asset reference to badges and explain rapid access revocation. |
| ID 3: IP storage | An ordinary stored hash alone does not establish trustworthy integrity | Explain who protects the expected hash; use an authenticated integrity mechanism where required. |
| ID 4: source code | Claims a firewall can be virtually unbreakable; relies on MAC addresses | Remove the absolute claim. Explain identity-based access, least privilege, release approval, and network controls as layered proposals. MAC filtering is not proof of user identity. |
| IDs 5–6: identity and customer records | Describes password encryption alongside other data | Distinguish password hashing from encryption of recoverable sensitive data. See [OWASP password-storage guidance](https://cheatsheetseries.owasp.org/cheatsheets/Password_Storage_Cheat_Sheet.html). |
| ID 6: customer records | Unmarked servers do not establish security | State actual access, encryption, monitoring, and data-retention controls instead. |
| ID 7: backups | Recovery intervals and retention are asserted without justification | Connect them to explicit recovery objectives and restoration tests. |
| All owners and costs | Every asset is assigned to CEO; costs lack calculation support | Label as assumptions and refine operational ownership and estimate basis. |
| Target scores | Six entries remain above their target upper bounds | Explain additional treatment, acceptance, or revised targets; do not claim all targets were met. |
| Original scale | Ranges overlap at 12 and are awkward for integer products | Define mutually exclusive integer bands before assigning risk-category labels. The CSV keeps numeric scores and makes no new band assignments. |
| Sources | CurseForge URL has a trailing `/!!!`; filing note has no direct link | Verify a replacement or archived URL while retaining original provenance. |

Read the proposal column alongside this critique. Suggested corrections are not implemented controls or evidence that risk was reduced.
