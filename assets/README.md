# Sanitized evidence

This directory contains screenshots used as technical evidence in the case studies.

## Expected structure

```text
assets/
├── gran-frutiver/
│   ├── storefront-home.webp
│   ├── login.webp
│   ├── user-management.webp
│   ├── cart.webp
│   └── checkout.webp
├── concurrent-hospital-auditing/
│   ├── indicators-dashboard.webp
│   ├── census-workflow.webp
│   ├── roles-permissions.webp
│   └── security-headers.webp
├── financial-applications-platform/
│   ├── dashboard.webp
│   ├── applications-list.webp
│   └── application-analysis.webp
├── clinical-record-auditing/
│   └── security-headers.webp
└── clinical-research-management/
    ├── document-management.webp
    └── security-headers.webp
```

## Before publishing

Verify that every image removes or obscures:

- patient, applicant, customer or employee names;
- identity/document numbers;
- email addresses and phone numbers;
- financial or clinical information that is not required for the case study;
- internal domains, hostnames and IP addresses;
- credentials, tokens and identifiers;
- private infrastructure;
- confidential product/client logos;
- unnecessary implementation details.

For security-assessment screenshots, prefer showing the **result and high-level controls** while hiding hostnames, IP addresses and detailed raw configuration.
