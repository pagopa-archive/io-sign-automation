# @io-sign/io-sign

## 1.0.0

### Major Changes

- e6a3334: BREAKING CHANGE: Added `formFields` attribute to `DocumentMetadata` in `io-sign` package
  [SFEQS-1266] Added validation of signature fields and pages during `ValidateUpload` in `io-func-sign-issuer`
  [SFEQS-1216] Fixed infra dependencies

### Minor Changes

- 76f46cc: Added health-check on the whole infra. [SFEQS-1273]
  `makeFetchWithTimeout` has been moved to the `io-sign` package.
- 5481a80: Require at least one mandatory signature for each dossier
- a0a818d: expand signature request to include issuer e-mail and description
- 0eef39c: Test Change
- 2e646fd: Added billing event

### Patch Changes

- 045b0eb: Added third_party_data to notification
- 12100f7: Added custom SAML mock and implement getFieldValue in PDF infra
- 3e00bff: Notification send refactor
  [SFEQS-1323,1329] Fixed sent notification messages
  [SFEQS-1325] Bug fix on updatedAt field
  [SFEQS-1311] Bug fix multiple notifications
- 6a3d7b6: fix minor bugs on REST API serialization and error responses
- 78ae07d: Added support for REJECTED status for signature request. [SFEQS-1277]
  Added a preliminary status check before signature creation
- ec71e65: pre-authenticate urls on signed signature requests (issuer)
- 22fee87: Add WAIT_FOR_QTSP status to signature request
- 62f8a61: Add environment to issuer data model
- 8afb588: Implement endpoints for third party message attachments
- 8afb588: Moved `getDocument` and `SignatureRequestDraft` to @io-sign package

## 0.9.0

### Minor Changes

- deb99dd: [SFEQS-1204, SFEQS-1214] Implement `CreateSignatureRequest`, `GetSignatureRequest`, `MarkAsWaitForSignature` Azure Functions

### Patch Changes

- 336cd7a: document state machine now correctly resets state-specific attributes [SFEQS-1146]
