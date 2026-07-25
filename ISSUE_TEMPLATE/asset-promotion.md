name: Asset Promotion Request
description: Propose promoting a local vault asset into the official GitMoney OS GitHub record.
title: "[PROMOTION]: "
labels: ["governance", "promotion-request"]
body:
  - type: markdown
    attributes:
      value: |
        Use this template to request promoting a local vault note or agent artifact into an official GitHub record.
  - type: input
    id: asset_title
    attributes:
      label: Asset Title
      description: Name of the asset being promoted.
    validations:
      required: true
  - type: textarea
    id: source_location
    attributes:
      label: Source Vault Path
      description: Exact internal path inside The Mothership vault.
    validations:
      required: true
  - type: dropdown
    id: target_repo
    attributes:
      label: Target GitHub Repository
      options:
        - GitMoneyOS/gitmoney-public-framework
        - GitMoneyOS/mothership-office
        - GitMoneyOS/gitmoney-os
        - GitMoneyOS/gitbuilt-proof-sprint
        - GitMoneyOS/gitmoney-audit-system
        - GitMoneyOS/gitmoney-client-delivery
        - GitMoneyOS/gitmoney-saas
    validations:
      required: true
  - type: textarea
    id: asset_test
    attributes:
      label: GitMoney Asset Test Verification
      description: State the Owner, Classification, Evidence Location, Approval Path, and Lifecycle.
    validations:
      required: true
