# Invoicing and payment reminder web app

### Description

#### 1. 5G
[Description website](https://www.codementor.io/projects/mobile/invoicing-and-payment-reminder-mobile-app-atx32o85yj)

#### 2. Dayra
```markdown
# Invoicing and payment reminder web app
Challenge Brief:Using Node js and MySQL database you should be building a RestFul API for a web application that generates, savesinvoices and send automated reminders to clients for their overdue invoices.

---

### Requirements

- Admin can generate an invoice with the following details:
    - Full Name
    - Mobile
    - email
    - Amount
    - Due Date of the invoice
- Saving clients information could happen through two different scenarios:
    - On generating their first invoice
    - Admin can add new client with the required information
- Once the invoice is generated the system sends it to the client to his email
- In case of overdue invoice payment, the system should send the client a reminder to his email reminding him with the invoice
```
---

### Recommend technologies

- Node.js
- MySQL
- REST Full API

---

### APIs

- Users
- Clients
- Invoices

---

### Invoices Features

- Receive, Save invoices
  - CRUD
- Generate invoices
  - Email template
  - PDF template send via Email
- Send invoices
  - Node mailer
- Send automated follow-up reminders for Overdue payments
  - CORN Job

---

### Users Features

- Admin generate an invoice

---

### Invoices Features

- Fields: [client: [FullName, Email, Phone], invoice: [Amount, DueDate]]
- *Pay an invoice
- *Cancel an invoice

---

### Clients Features

- Fields: [Full name, Email, Phone]
- Save on generate there first invoice
- Admin add new client with required fields

---

### Requirements

- Users can save client information in the app
- Users can quickly generate a new invoice for a saved client
- Users can send invoices to clients from within the app

---

### Integration

- Send email
  <!-- - Sms via Twillio -->
  <!-- - Generate via jsPDF -->

---

### Bonus

- Admin dashboard
- Invoice generator page

---

### Email templates

```bash
# Overdue invoice
Title: Follow up on payment of \$${invoice_amount | money dd,ddd.dd}
To: ${client_email}
Message:
Dear ${client_name | title_case},

This message is to formally notify you that the payment owed by you is more than ${difference_date = today - due_date | three day, four weeks} overdue. The amount of \$${invoice_amount | money dd,ddd.dd} was due on ${due_date | Month, dd yyyy}.

If you have already paid this invoice, please disregard this email.

Otherwise, please send the payment as soon as possible.

Thank you very much for your attention to this matter!

Should you need any further information, please do not hesitate to contact me.

With best regards,
${APP_NAME}
```

```bash
# Income invoice reminder
Title: Follow up on payment of \$${invoice_amount | money dd,ddd.dd}
To: ${client_email}
Message:
Dear ${client_name | title_case},

For the convenience I just wanted to send you a gentle reminder that your payment for payment of \$${invoice_amount | money dd,ddd.dd} is due on ${due_date | Month, dd yyyy}.

I hope you have a wonderful rest of the week and looking forward to doing business with you again soon!

Kind regards,
${APP_NAME}
```
