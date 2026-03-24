# User Workflow Journey Documentation: Parent Fund Allocation & Management for Youth Account

## Experience Mindset

**Primary User:** Parent or Guardian
**Experience:** Allocating and managing funds for a youth account, including setting spending limits and monitoring activity. This experience encompasses:
- Account overview & dashboard
- Fund transfer/allocation
- Spending limit management
- Viewing youth spending activity
- Handling errors (e.g., insufficient funds)

---

## Scenarios & Workflow Variations

### Scenario 1: Access Youth Account Dashboard
**Context:** Parent is logged into the banking web app, wants to review youth account status.

#### Variation 1A: Direct Navigation from Main Dashboard
- Parent clicks "Youth Account" from main navigation.
- Youth account dashboard loads.

#### Variation 1B: Quick Access Widget
- Parent sees a "Youth Account" widget on main dashboard.
- Clicks widget to access youth account dashboard directly.

**User Goal:** Quickly access youth account summary and recent activity.
**Business Goal:** Increase engagement with youth account features, reinforce transparency and control.

**Screens:**
1.0 Main Dashboard
2.0 Youth Account Dashboard

---

### Scenario 2: Allocate Funds to Youth Account
**Context:** Parent wants to add money to the youth account from their primary account.

#### Variation 2A: Modal-based Transfer
- Parent selects "Add Funds" from dashboard.
- Modal opens for transfer details.
- Confirmation step in modal.

#### Variation 2B: Dedicated Transfer Page
- Parent selects "Add Funds" from dashboard.
- Redirected to a dedicated transfer page.
- Confirmation and success message on completion.

**User Goal:** Seamlessly transfer funds to youth account with minimal friction.
**Business Goal:** Encourage responsible funding, track parental engagement.

**Screens:**
1.0 Youth Account Dashboard
2.0 Fund Transfer Modal (Pu.1) / 2.0 Fund Transfer Page
3.0 Transfer Confirmation (Pu.2) / 3.0 Success State

---

### Scenario 3: Set Spending Limit
**Context:** Parent wants to set or update a weekly spending limit for youth account.

#### Variation 3A: Inline Limit Edit
- Parent sees current limit on dashboard.
- Clicks "Edit" to modify limit inline.
- Confirmation prompt before saving.

#### Variation 3B: Separate Limit Management Page
- Parent navigates to "Manage Limits" page.
- Sets/updates limit with contextual guidance.
- Confirmation and feedback.

**User Goal:** Easily configure or adjust spending limits for youth.
**Business Goal:** Promote financial literacy, provide safety controls.

**Screens:**
1.0 Youth Account Dashboard
2.0 Inline Limit Edit (2.1) / 2.0 Limit Management Page
3.0 Confirmation (Pu.3)

---

### Scenario 4: View Youth Spending Activity
**Context:** Parent wants to review youth's recent transactions.

#### Variation 4A: Activity Tab on Dashboard
- Parent clicks "Activity" tab on dashboard.
- Recent transactions displayed with filters.

#### Variation 4B: Full Activity Page
- Parent selects "View All Activity."
- Redirected to detailed activity page with advanced filters.

**User Goal:** Monitor youth spending and identify patterns.
**Business Goal:** Provide transparency, build trust, and offer actionable insights.

**Screens:**
1.0 Youth Account Dashboard
2.0 Activity Tab (2.2) / 2.0 Full Activity Page

---

### Scenario 5: Handle Insufficient Balance During Fund Allocation
**Context:** Parent attempts to transfer more funds than available in their account.

#### Variation 5A: Inline Error Message
- Error appears below amount input in transfer modal/page.
- Parent can adjust amount without leaving flow.

#### Variation 5B: Error Pop-up
- Upon submitting, error pop-up explains insufficient funds.
- Option to retry or cancel.

**User Goal:** Understand why transfer failed and how to resolve.
**Business Goal:** Reduce failed transactions, guide users to resolution.

**Screens:**
1.0 Fund Transfer Modal/Page
Er.1 Inline Error
Pu.4 Error Pop-up

---

## Minimum Viable Experience (MVE)

### Scenario Example: Allocate Funds to Youth Account
**User:** Priya, a parent, wants to add $50 to her son's youth account for weekly expenses.

**User Goal:** Quickly and securely transfer funds to youth account.
**Business Goal:** Ensure smooth parental control over youth account funding.

### Screen List & Details

#### 1.0 Youth Account Dashboard
- **Goal:** Provide comprehensive overview of youth account, quick access to actions.
- **Description:**
  - Shows current balance, recent activity, spending limit, and quick actions (Add Funds, Manage Limits).
- **Design Problems:**
  - HMW make key actions visible without clutter?
  - HMW prioritize information for quick scanning?
- **Design Opportunities:**
  - What if dashboard adapts based on usage patterns?
  - What if quick tips are shown for first-time users?

#### 2.0 Fund Transfer Modal (Pu.1)
- **Goal:** Allow parent to enter transfer details efficiently.
- **Description:**
  - Inputs for source account, amount, and optional note.
  - Inline validation for amount and available balance.
- **Design Problems:**
  - HMW prevent accidental large transfers?
  - HMW clarify available balance?
- **Design Opportunities:**
  - What if preset amounts are suggested?
  - What if parent can schedule recurring transfers?

#### 3.0 Transfer Confirmation (Pu.2)
- **Goal:** Confirm transfer details before execution.
- **Description:**
  - Summarizes source, destination, amount, and confirms action.
- **Design Problems:**
  - HMW ensure parent reviews before confirming?
- **Design Opportunities:**
  - What if confirmation includes educational tips on allowance?

#### 4.0 Success State
- **Goal:** Provide positive feedback and next steps.
- **Description:**
  - Shows success message, updated balance, and option to view activity.
- **Design Problems:**
  - HMW encourage further engagement after transfer?
- **Design Opportunities:**
  - What if parent can share a message with youth about the transfer?

#### Er.1 Inline Error / Pu.4 Error Pop-up
- **Goal:** Clearly communicate errors (e.g., insufficient funds), allow easy correction.
- **Description:**
  - Error message with actionable suggestion.
- **Design Problems:**
  - HMW avoid frustration during failed transactions?
- **Design Opportunities:**
  - What if system offers to top up parent account or adjust transfer amount?

---

## Sequence of Screens (Sample Workflow: Fund Allocation)
1.0 Youth Account Dashboard -> 2.0 Fund Transfer Modal (Pu.1) -> 3.0 Transfer Confirmation (Pu.2) -> 4.0 Success State

Alternative: 1.0 Youth Account Dashboard -> 2.0 Fund Transfer Page -> 3.0 Success State

---

## Additional Screen Flows

### Spending Limit Configuration
1.0 Youth Account Dashboard -> 2.0 Inline Limit Edit (2.1) -> 3.0 Confirmation (Pu.3)
OR
1.0 Youth Account Dashboard -> 2.0 Limit Management Page -> 3.0 Confirmation (Pu.3)

### Viewing Activity
1.0 Youth Account Dashboard -> 2.0 Activity Tab (2.2)
OR
1.0 Youth Account Dashboard -> 2.0 Full Activity Page

### Error Handling
Fund Transfer Modal/Page -> Er.1 Inline Error
OR
Fund Transfer Modal/Page -> Pu.4 Error Pop-up

---

## Accessibility & Scalability Considerations
- All actions are accessible via keyboard and screen readers.
- Clear focus states, color contrast, and alt text for icons.
- Responsive layouts for desktop and tablet.
- Modular design supports future features (e.g., scheduled transfers, spending insights).

---

## Summary Table: Screens & Goals
| Screen # | Title                         | Goal                                      |
|----------|-------------------------------|-------------------------------------------|
| 1.0      | Youth Account Dashboard       | Overview, quick actions                   |
| 2.0      | Fund Transfer Modal/Page      | Input transfer details                    |
| 2.1      | Inline Limit Edit             | Edit spending limit                       |
| 2.2      | Activity Tab                  | View recent transactions                  |
| 3.0      | Confirmation/Success State    | Confirm and acknowledge actions           |
| Pu.1     | Fund Transfer Modal           | Input transfer details (popup)            |
| Pu.2     | Transfer Confirmation         | Confirm transfer (popup)                  |
| Pu.3     | Limit Change Confirmation     | Confirm spending limit change             |
| Pu.4     | Error Pop-up                  | Communicate errors                        |
| Er.1     | Inline Error                  | Show validation errors                    |

---

## Design Problems & Opportunities (Examples)
- HMW (How Might We) help parents understand and control youth spending?
- HMW minimize friction in fund allocation?
- HMW provide reassurance and transparency?
- What if we offer parental tips based on youth spending patterns?
- What if we enable collaborative goal-setting between parent and youth?

---

## End of Documentation
