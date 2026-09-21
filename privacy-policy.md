# Privacy Policy

**Last updated:** September 21, 2026

This Privacy Policy applies to software side projects, web applications, and extensions published by **Lumostera, MB** on the Wix App Market (collectively, the **"Apps"** or **"Wix Apps"**).


If you are a site visitor or customer of a merchant using one of our Apps, and you have questions about your personal data, please contact the merchant (site owner) directly, as the merchant controls their own site's data. You may also contact Lumostera, MB at `info@lumostera.com`.

> ### **Key Summary: 100% Native Wix Infrastructure & Zero External Data Storage**
> - **All Data Held Exclusively on Wix**: Every record processed or stored by our Apps resides solely within the merchant's own Wix Data (CMS) collections and site settings on Wix's official cloud infrastructure.
> - **Zero External DevOps or Databases**: Lumostera, MB operates no external servers, databases, or third-party cloud storage (no AWS, Google Cloud, Azure, Supabase, or private endpoints).
> - **Exclusively Native Wix APIs**: The Apps run 100% on Wix serverless compute and communicate exclusively via official Wix APIs. No merchant, store, order, or customer data is ever sent to, shared with, or stored on external servers.

---

## 1. Who controls this data

Each App is installed by a merchant onto their own Wix site. The merchant is the **data controller** of all store and order data. We (Lumostera, MB, the developer) provide the software extensions, which execute strictly inside the merchant's own Wix environment and interact solely with Wix platform APIs.

## 2. Where data is stored

**All data stored by any App is stored in the merchant's own Wix Data (CMS) collections, on the merchant's own Wix site — entirely within Wix infrastructure, and never on developer servers.** 

The Apps use Wix's native platform data layer (`@wix/data` items and collections APIs) exclusively for query, insert, update, remove, and readiness checks. The software contains no external database client, no third-party object-storage SDK, and makes no outbound network requests to any non-Wix domain.

**We do not operate independent servers or cloud storage for your data**, and there are **no third parties** with whom any App shares merchant or customer data, beyond Wix itself as the underlying hosting and eCommerce platform.

The only information transmitted to the developer is diagnostic and operational telemetry, described in Section 6 below, transmitted via Wix's native BI event pipeline — strictly limited to non-identifying operational health signals, never customer content.

## 3. What the Apps collect, and why

The Apps collect and persist only what is strictly necessary to provide their merchant-configured functionality:

1. **Merchant Business Configuration**:
   - Includes merchant-defined rules, options, thresholds, templates, and display settings (such as fee amounts, validation criteria, discount tiers, delivery rules, pipeline stages, or document templates).
   - Stored in app-specific private Wix Data collections on the merchant's site.
   - **Not customer-linked:** Contains purely operational merchant settings.

2. **Operational Workflow Data**:
   - Includes staff-authored internal notes, fulfillment stage tracking, or layaway/deposit schedule records created by the merchant's team to manage store operations.
   - Stored in app-specific private Wix Data collections on the merchant's site, linked to internal order or contact identifiers.

3. **Payment & Credential Security**:
   - **None.** The Apps do not read, process, or store customer payment cards, bank details, or account passwords. All checkouts, billing, and transactions are handled exclusively by Wix Payments and official Wix eCommerce infrastructure.

## 4. How long data is retained, and uninstall behavior

Because all data lives in the merchant's own Wix Data collections, data retention is managed directly within the merchant's Wix site.

When a merchant uninstalls an App from their site, the platform delivers an `app-removed` webhook event:
- **Operational Workflow Records**: Operational order-linked data is purged upon uninstall via automated platform lifecycle handlers.
- **Merchant Business Configuration**: Configuration settings and rule definitions are retained within the merchant's site storage so that an accidental uninstallation does not destroy business configuration upon reinstall.
- **Manual Deletion**: Merchants have full administrative access to view, export, or delete any app-specific collection directly in the Wix Business Manager (via CMS / Wix Data).

## 5. Third-party disclosure

We do not sell, rent, trade, or transfer merchant or customer data to third parties. All processing occurs within Wix's secure platform infrastructure.

## 6. Diagnostic and operational telemetry

To monitor availability and provide technical support, the Apps emit structured operational events to Wix's BI telemetry pipeline. These events contain:
- `app_version`, `schema_version`, `timestamp`
- `outcome` (`success`, `failure`, `timeout`)
- `surface` (`dashboard`, `backend_event`, `service_plugin`)
- Sanitized operational `error_code` and `wix_request_id`

**No customer personal data, note text, recipient details, or raw exception stack traces containing free text are ever transmitted.** All string identifiers pass through strict sanitization filters that discard non-whitelisted tokens prior to transmission.

## 7. Your rights and how to request deletion

### For Merchants
Merchants may access, export, or delete any data persisted by the Apps directly through the Wix Business Manager (via Wix Data / CMS collections). Additionally, merchants may request manual purging of configuration or historical records by contacting `info@lumostera.com`.

### For Customers of Merchants
If you are a consumer or buyer whose order or profile is referenced within a merchant's internal notes or fulfillment timeline, please direct your data subject request (access, correction, or deletion) to the respective merchant. If the merchant requires developer assistance to fulfill an erasure request, the merchant may contact us at `info@lumostera.com`.

### European Economic Area (EEA) & UK Rights
Under the EU General Data Protection Regulation (GDPR) and UK GDPR, data subjects have the right to:
- Request access to and a copy of their personal data.
- Request rectification of inaccurate personal data.
- Request erasure ("right to be forgotten") of personal data where retention is no longer lawful.
- Request restriction of processing or object to processing.
- Request data portability.
- Lodge a complaint with a supervisory authority. In Lithuania, the relevant authority is the State Data Protection Inspectorate (*Valstybinė duomenų apsaugos inspekcija* — VDAI, [vdai.lrv.lt](https://vdai.lrv.lt)).

## 8. Children's privacy

The Apps are professional, business-to-business tools intended solely for merchants and commercial site owners. We do not knowingly collect or solicit personal data from children under the age of 16. If you believe an App has inadvertently received personal data relating to a child, please contact `info@lumostera.com` so we may promptly assist the merchant with deletion.

## 9. Changes to this policy

We may update this Privacy Policy from time to time to reflect operational, legal, or regulatory changes. Any modifications will be posted to this page with an updated "Last updated" date. Continued use of the Apps after any update constitutes acknowledgment of the revised terms.

## 10. Contact
 
**Developer / Company:** Lumostera, MB  
**Company Code:** `305928828`  
**Address:** Aušros g. 4, Tauralaukio k., LT-54415 Kauno r., Republic of Lithuania  
**Contact Email:** `info@lumostera.com`  
**Governing Law:** Republic of Lithuania
