## 1. Student Item Listing (Enhancement, Estimate: 5, Sprint 1)
As a **student**, I need **to list an item for barter**, so that **others can see it and propose trades**.

### Acceptance Criteria
- Given I am logged in, When I submit a form with title, description, image, and category, Then the item appears in the public listings.
- Given the form has missing fields, When I submit, Then I see validation errors and cannot proceed.

---

## 2. Student Registration (Enhancement, Estimate: 2, Sprint 1)
As a **student**, I need **to create an account**, so that **I can list items and receive trade proposals**.

### Acceptance Criteria
- Given valid email/password/university ID, When I register, Then I receive a confirmation email and can log in.
- Given duplicate email, When I register, Then I see an error and prompted to log in instead.

---

## 3. Search Items (Technical Debt - Req 9, Estimate: 3, Sprint 1)
As a **student**, I need **to search items by category/keyword**, so that **I find relevant barter opportunities quickly**.

### Acceptance Criteria
- Given I enter "books" in search, When I submit, Then only matching items show with filters applied.
- Given no results, When searching, Then I see "No items found" with suggestion to broaden search.

---

## 4. Send Trade Proposal (Enhancement, Estimate: 5, Sprint 1)
As a **student**, I need **to propose a trade with my item**, so that **the owner can accept or counter**.

### Acceptance Criteria
- Given I view an item, When I select my item and send proposal, Then owner gets notification with details.
- Given no items owned by me, When proposing, Then I see prompt to list one first.

---

## 5. View Proposals (Enhancement, Estimate: 2, DONE)
As a **student**, I need **to view incoming trade proposals**, so that **I can accept, reject, or counter**.

### Acceptance Criteria
- Given I have proposals, When I check dashboard, Then list shows sender item, message, and actions.
- Given accepted proposal, When viewing, Then status updates to "Trade Confirmed" for both.

**Assignees:** Aneesh Tayal

---

## 6. Admin Fraud Flagging (Technical Debt - Req 10, Estimate: 3, In Progress)
As an **admin**, I need **to flag fraudulent listings**, so that **the community stays safe from scams**.

### Acceptance Criteria
- Given suspicious item, When admin flags it, Then item is hidden pending review and user notified.
- Given flagged items queue, When reviewing, Then approve/remove with audit log.

**Assignees:** Aneesh Tayal

---

## 7. Profile Management (Enhancement, Estimate: 1, Review/QA)
As a **student**, I need **to manage my profile and inventory**, so that **others trust my listings**.

### Acceptance Criteria
- Given logged in, When editing profile, Then university ID, bio, and photo update immediately.
- Given my items list, When deleting one, Then it's removed from search and my inventory.

**Assignees:** Aneesh Tayal

---

## 8. Notifications (Enhancement, Estimate: 5, In Progress)
As a **student**, I need **real-time notifications for proposals**, so that **I respond promptly**.

### Acceptance Criteria
- Given new proposal, When received, Then email + in-app alert appears.
- Given read notification, When marking, Then it clears from unread list.

**Assignees:** Aneesh Tayal

---

## 9. Categories Setup (Enhancement, Estimate: 2, Product Backlog)
As an **admin**, I need **predefined categories**, so that **students organize listings effectively**.

### Acceptance Criteria
- Given admin access, When adding new category, Then it appears in item listing form.
- Given active categories, When listing item, Then students must select one.

---

## 10. Trade History (Enhancement, Estimate: 3, Sprint Backlog)
As a **student**, I need **past trade history**, so that **I track completed barters**.

### Acceptance Criteria
- Given completed trades, When viewing history, Then shows date, items traded, and partner.
- Given filtered by date range, When searching history, Then only matching trades display.
