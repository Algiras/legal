# Privacy Policy

**Last updated:** September 21, 2026

This Privacy Policy applies to all software applications, web tools, integrations, and extensions published by **Lumostera, MB** ("Lumostera", "we", "us", or "our") across software marketplaces, web platforms, and app ecosystems (including the Wix App Market, standalone web tools, and related software platforms) (collectively, the **"Apps"**).

If you are an end user, site visitor, or customer of a business or merchant using one of our Apps, and you have questions regarding your personal data, please contact the respective site owner or business directly, as they act as the data controller of their own site and customer records. You may also contact Lumostera, MB at `info@lumostera.com`.

> ### **Core Architecture & Data Privacy Notice**
> - **Native Platform Storage & Zero External Databases**: All data processed or stored by our Apps resides exclusively within the user's or merchant's own platform data layer (for example, native Wix Data / CMS collections for Wix Apps, or client-side storage for browser extensions). Lumostera, MB operates no external servers, databases, or third-party cloud data warehouses (no AWS, Google Cloud, Azure, Supabase, or private server endpoints).
> - **Native Platform Execution**: The Apps execute within official platform serverless runtimes or client environments and communicate exclusively via official platform APIs. No business, customer, or order data is ever exfiltrated, sold, or stored on external servers.

---

## 1. Who controls this data

When an App is installed or used within a merchant or user site (such as a Wix site):
- The merchant or site owner is the **data controller** of all store, customer, and order data.
- Lumostera, MB acts strictly as a software provider. Our software extensions execute within the host platform environment and interact solely via official platform APIs.

## 2. Where data is stored

**All data stored by any App is stored in user- or merchant-owned storage on the host platform — entirely within host platform infrastructure, and never on independent developer servers.** 

For example, for applications running within the Wix ecosystem, all configuration rules and workflow records are saved in the merchant's own private Wix Data collections using official `@wix/data` SDK interfaces. The software contains no external database drivers, no third-party cloud storage clients, and makes no outbound network requests to any external third-party servers.

**We do not operate independent servers or cloud storage for your data**, and there are **no third parties** with whom any App shares merchant or customer data, beyond the host platform itself as the underlying eCommerce and hosting provider.

The only information transmitted to the developer is diagnostic and operational telemetry, described in Section 6 below, transmitted via native platform event pipelines — strictly limited to non-identifying operational health signals, never customer personal content.

## 3. What the Apps collect, and why

The Apps collect and persist only what is strictly necessary to deliver their configured functionality:

1. **Business & App Configuration**:
   - Includes user- or merchant-defined rules, settings, thresholds, display options, and templates (such as fee rules, validation criteria, pricing tiers, delivery settings, or document templates).
   - Stored in app-specific private storage collections within the merchant's or user's host platform account.
   - **Not customer-linked:** Contains purely operational configuration settings.

2. **Operational Workflow Data**:
   - Includes staff-authored internal notes, fulfillment stage tracking, or layaway/deposit schedule records created by store teams to manage internal operations.
   - Stored in app-specific private platform collections, linked to internal order or contact identifiers.

3. **Payment & Credential Security**:
   - **None.** The Apps do not read, process, or store payment card numbers, bank details, or passwords. All payment transactions, checkouts, and subscription billings are handled exclusively by the host platform (such as Wix Payments, Wix Billing, or official platform payment gateways).

## 4. How long data is retained, and uninstall behavior

Because all data lives in the merchant's or user's own host platform collections, data retention is managed directly within the host site.

When an App is uninstalled from a host site:
- **Operational Workflow Records**: Operational order-linked records are purged upon uninstall via automated platform lifecycle handlers where applicable.
- **Business Configuration**: Configuration rules and settings are retained within the site's private collections so that an accidental uninstallation does not destroy business configuration upon reinstall.
- **Manual Deletion**: Site owners maintain administrative control to view, export, or delete any app-specific collection directly through their host platform dashboard (e.g., via Wix CMS / Wix Data).

## 5. Third-party disclosure

We do not sell, rent, trade, or transfer personal or customer data to third parties. All processing occurs within secure, official platform infrastructure.

## 6. Diagnostic and operational telemetry

To monitor availability and provide technical support, the Apps emit structured operational events to native platform telemetry pipelines. These events contain:
- `app_version`, `schema_version`, `timestamp`
- `outcome` (`success`, `failure`, `timeout`)
- `surface` (`dashboard`, `backend_event`, `service_plugin`, etc.)
- Sanitized operational `error_code` and platform `request_id`

**No customer personal data, note text, recipient details, or raw exception stack traces containing free text are ever transmitted.** All string identifiers pass through strict sanitization filters that discard non-whitelisted tokens prior to transmission.

## 7. Your rights and how to request deletion

### For Merchants & Site Owners
Merchants may access, export, or delete any data persisted by the Apps directly through their host platform dashboard (e.g., via Wix Business Manager CMS). Additionally, merchants may request manual assistance with data purging by contacting `info@lumostera.com`.

### For Customers of Merchants
If you are a consumer or buyer whose order or profile is referenced within a merchant's internal notes or fulfillment timeline, please direct your data subject request (access, correction, or deletion) to the respective merchant or business. If the merchant requires developer assistance to fulfill an erasure request, the merchant may contact us at `info@lumostera.com`.

### European Economic Area (EEA) & UK Rights
Under the EU General Data Protection Regulation (GDPR) and UK GDPR, data subjects have the right to:
- Request access to and a copy of their personal data.
- Request rectification of inaccurate personal data.
- Request erasure ("right to be forgotten") of personal data where retention is no longer lawful.
- Request restriction of processing or object to processing.
- Request data portability.
- Lodge a complaint with a supervisory authority. In Lithuania, the relevant authority is the State Data Protection Inspectorate (*Valstybinė duomenų apsaugos inspekcija* — VDAI, [vdai.lrv.lt](https://vdai.lrv.lt)).

## 8. Children's privacy

The Apps are professional and utility tools intended for businesses and site owners. We do not knowingly collect or solicit personal data from children under the age of 16. If you believe an App has inadvertently received personal data relating to a child, please contact `info@lumostera.com` so we may promptly assist with deletion.

## 9. Changes to this policy

We may update this Privacy Policy from time to time to reflect operational, legal, or regulatory changes. Any modifications will be posted to this page with an updated "Last updated" date. Continued use of the Apps after any update constitutes acknowledgment of the revised terms.

## 10. Contact
 
**Developer / Company:** Lumostera, MB  
**Company Code:** `305928828`  
**Address:** Aušros g. 4, Tauralaukio k., LT-54415 Kauno r., Republic of Lithuania  
**Contact Email:** `info@lumostera.com`  
**Governing Law:** Republic of Lithuania
