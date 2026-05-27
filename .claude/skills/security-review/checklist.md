# Security Review Checklist

## Input Validation
- [ ] All user input sanitized before DB queries
- [ ] File upload MIME types validated
- [ ] Path traversal prevented on file operations

## Authentication
- [ ] JWT tokens expire appropriately
- [ ] API keys stored in environment variables, never hardcoded
- [ ] Passwords hashed with bcrypt or argon2

## Authorization
- [ ] Every route checks user permissions
- [ ] Resource ownership verified before mutation
- [ ] Admin-only endpoints protected

## Data Exposure
- [ ] No sensitive fields returned in API responses
- [ ] Error messages don't leak internals
- [ ] Logs don't contain credentials or PII
