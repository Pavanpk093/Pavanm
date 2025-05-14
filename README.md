# GitHub Actions Workflow: CI for Dr. Pavan Kumar Murarishetti

name: CI - Regulatory Affairs Projects

on:
  push:
    branches: [ "main" ]
  pull_request:
    branches: [ "main" ]
  workflow_dispatch:

jobs:
  build:
    runs-on: ubuntu-latest

    steps:
      - name: Checkout Repository
        uses: actions/checkout@v4

      - name: Greet and Acknowledge
        run: echo "Hello, world! This CI workflow belongs to Dr. Pavan Kumar Murarishetti."

      - name: Display Professional Information
        run: |
          echo "Email: pavankumarpk093@gmail.com"
          echo "Phone: (617) 256-0821"
          echo "LinkedIn: www.linkedin.com/in/pavankumarmurarishetti"
          echo "Field: Regulatory Affairs | Medical Devices | Clinical Research"

      - name: Print Recent Project Highlights
        run: |
          echo "Recent Projects:"
          echo "- Regulatory strategy for EVOQUE Tricuspid Valve Replacement System"
          echo "- Clinical trial protocol for adalimumab"
          echo "- Design control and development plan for MeDioStar"
          echo "- Product lifecycle strategy for Magic Dust"

      - name: Display Technical Skills
        run: |
          echo "Key Skills:"
          echo "- FDA, EMA, ISO Regulations, CE Marking"
          echo "- 510(k), IND, eCTD submissions, GCP, GMP"
          echo "- Risk Management (FMEA, CAPA), QMS, PMS"
          echo "- Tools: SQL, Power BI, Excel, Visio"

      - name: Final Message
        run: echo "CI workflow executed successfully. Regulatory Excellence in Action!"
