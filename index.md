This is a working demo tackling an onboarding workflow problem in real estate accounting: manually reconciling and entering a prior management company’s financials into the firm’s accounting software during property onboarding. Built on Base44.

## The Problem

Financial analysts onboarding new properties face a significant efficiency bottleneck during the financial data transfer process. Currently, the process requires an analyst to spend **2-3 hours per property** on manual reconciliation, often involving a tedious "side-by-side" workflow—viewing the prior management firm’s trial balance (in Excel or PDF view) on one screen while manually inputting data into the new firm’s accounting system on the other.

### Core Challenges:

* **GL Code Discrepancies:** The primary issue is that legacy GL codes from prior agents rarely align with the new firm’s Chart of Accounts.

* **Manual Entry:** Analysts must manually map each legacy GL code to the corresponding internal code, calculate totals, and perform line-by-line data entry. Then, the analyst will post the journal entry to capture the property's financial data. This is the first set of financial information posted on the new firm's books.
 
* **Operational Risk:** This repetitive, manual process is not only time-consuming but also creates a high risk of human error, potentially delaying month-end close and reducing the analyst's ability to focus on higher-value financial review.

## The Solution
A data mapping tool that takes a trial balance CSV from the prior management firm and produces an import-ready file journal entry for the new firm’s accounting software.

## The Workflow
1. **Upload:** Analyst uploads the prior firm's trial balance CSV.
2. **AI Matching:** The tool matches each source GL against the firm's chart of accounts, assigning a confidence score to each suggestion.
3. **Review:** The analyst reviews each row, confirms suggestions, overrides with a different target GL, or flags rows for manual decision.
4. **Validation:** High-confidence matches are bulk-confirmed; the tool validates that total source dollars equal total mapped dollars before allowing finalization.
5. **Export:** Upon confirmation, the tool exports a CSV in the target software's format and shows a journal entry preview. 

![Workflow Step 1](Workflow%20Step%201.png)

![Workflow Step 2](Workflow%20Step%202.png)

![Workflow Step 3](Workflow%20Step%203.png)

![Workflow Step 4](Workflow%20Step%204_.png)

## Out of Scope
1. Data accuracy of previous firm’s financials 
2. Multi-period imports (one trail balance per upload)
3. Non 1:1 matches
