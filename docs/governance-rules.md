# API Governance Rules

This document outlines the rules enforced by Spectral for API validation and governance.

## 🔍 Error Reporting & Severity Levels

Each rule is assigned a severity level:

- 🛑 **Error** → Must be fixed for API compliance.
- ⚠️ **Warning** → Recommended improvements.
- ℹ️ **Info** → General guidance.

## 🔎 Examples of Improved Error Messages

1. **Missing Contact Field in API Info**  
   - **Error Message:** `"API specifications should include a contact field."`
   - **Severity:** ⚠️ Warning  
   - **Fix:** Add a `contact` field in `info` object.

2. **Missing Tags in API Operations**  
   - **Error Message:** `"Operations should include a 'tags' field for better categorization."`
   - **Severity:** 🛑 Error  
   - **Fix:** Ensure every API operation has a `tags` field.

3. **Unused Component in API Spec**  
   - **Error Message:** `"Unused components should be removed."`
   - **Severity:** ℹ️ Info  
   - **Fix:** Remove unreferenced schemas from `components`.

---

## 📜 How to Run API Linting  
Run the following command to validate your API specifications:

```bash
npm run lint:api
