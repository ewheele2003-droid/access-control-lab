# User Access Control Policy

## Purpose
This policy establishes procedures for managing user access requests, approvals, and exceptions at SealGames Studios to ensure appropriate access control aligned with the principle of least privilege and NIST 800-171 controls.

## Scope
Applies to all employees, contractors, and temporary staff requiring access to critical systems including cloud storage and game servers.

## Roles and Responsibilities

### Requestor (Employee)
- Submit access requests with business justification
- Notify manager of access needs
- Provide required information (name, role, systems, access level, duration)

### Manager/Tech Lead (Approver Level 1)
- Review requests for appropriateness to role
- Verify business justification
- Approve or deny requests within 2 business days
- Document approval rationale
- Notify requestor of decision

### Director (Approver Level 2)
- Review escalations and exceptions
- Approve high-risk or sensitive access requests
- Review quarterly access reports
- Authorize exceptions to policy

### System Administrator
- Process approved requests
- Grant access within 24 hours of approval
- Document access changes in audit log
- Revoke access when employment ends or access expires

### Security Officer
- Monitor access compliance
- Conduct quarterly access reviews
- Report violations to management
- Update policy as needed

## Access Request Process

### Step 1: Identify Need
- Employee determines what systems/access they need for their role
- Consults with manager if unclear

### Step 2: Submit Request
- Employee completes Access Request Form with:
  - Full name and employee ID
  - Current role and department
  - Systems requesting access to (Cloud Storage, Game Servers, etc.)
  - Required access level (Admin, Read/Write, Read-only)
  - Business justification (why they need this access)
  - Expected duration (permanent or temporary)
  - Manager name for approval routing

**Control Reference:** NIST 800-171 AC-2 (Account Management)

### Step 3: Manager Review
- Tech Lead reviews request within 2 business days
- Verifies access aligns with employee role
- Confirms business justification is valid
- Checks for principle of least privilege (minimum access needed)
- Approves or denies with written explanation

**Control Reference:** NIST 800-171 AC-3 (Access Enforcement)

### Step 4: System Administrator Implementation
- Upon approval, System Administrator receives request
- Provisions access to requested systems within 24 hours
- Logs all access changes with timestamp and administrator ID
- Provides confirmation to requestor and manager

**Control Reference:** NIST 800-171 AC-2(1) (Account Management - Privileged Access)

### Step 5: Documentation & Audit
- Access request and approval added to audit trail
- Stored in Access Control Registry
- Quarterly reviews conducted to verify access is still needed
- Access revoked if employee role changes or employment ends

**Control Reference:** NIST 800-171 AU-2 (Audit Events)

## Access Levels Defined

### Cloud Storage
- **Read-only** — View files, cannot modify or delete
- **Read/Write** — View, create, modify, but cannot delete or change permissions
- **Admin** — Full access including create, modify, delete, and user management

### Game Servers
- **Read-only** — View server status and logs, cannot make changes
- **Read/Write** — Deploy builds, modify configurations, restart services
- **Admin** — Full access including user management, security groups, backups

## Approval Authority

| Access Level | System | Approver |
|--------------|--------|----------|
| Read-only | Cloud Storage | Tech Lead |
| Read/Write | Cloud Storage | Tech Lead |
| Admin | Cloud Storage | Tech Lead (≤3 people), Director (>3 people) |
| Read-only | Game Servers | Tech Lead |
| Read/Write | Game Servers | Tech Lead |
| Admin | Game Servers | Director |

## Timeline

| Step | Owner | Timeline |
|------|-------|----------|
| Submit Request | Requestor | Day 1 |
| Manager Review | Tech Lead | Day 1-2 |
| Approval Decision | Tech Lead | Day 3 |
| System Administrator Implementation | System Admin | Day 3-4 |
| Access Granted | System Admin | Day 4 |
| Confirmation to Requestor | System Admin | Day 4 |

**Typical Total Duration: 3-5 business days** (up to 1 week if escalation needed)

## Exceptions & Escalations

### Emergency Access
- If urgent access needed outside normal process:
  - Requestor contacts Tech Lead
  - Tech Lead contacts Director for expedited approval
  - Access can be provisioned within 4 hours with verbal approval
  - Formal documentation must follow within 1 business day
  - Access automatically expires after 7 days unless formalized

**Control Reference:** NIST 800-171 AC-2(7) (Account Management - Role-based schemes)

### Access Exceptions
- If requested access exceeds policy guidelines:
  - Tech Lead documents exception reason
  - Director must formally approve in writing
  - Exception stored with business justification
  - Reviewed quarterly

### Denied Requests
- If request denied:
  - Approver provides written reason
  - Requestor can appeal to Director within 5 business days
  - Director issues final decision

## Offboarding

### Upon Employment Termination
- HR notifies System Administrator of termination date
- System Administrator revokes ALL access on termination date
- All credentials disabled or deleted
- Exit interview conducted to review any data access concerns
- Access revocation logged in audit trail

**Control Reference:** NIST 800-171 AC-2(2) (Account Management - Removal)

## Access Reviews

### Quarterly Review
- Security Officer pulls current access report
- Tech Lead and Manager review each employee's access
- Verify access still aligns with current role
- Revoke unnecessary access
- Document review in audit file

### Annual Review
- Director reviews all admin-level access
- Ensures principle of least privilege is maintained
- Identifies and removes privileged access for employees who changed roles

**Control Reference:** NIST 800-171 AC-2(1) (Account Management - Privileged Access)

## Compliance & Audit

- All access requests and approvals retained for minimum 3 years
- Audit trail maintained with timestamps and user IDs
- Quarterly reports provided to management
- Annual compliance certification required

**Control Reference:** NIST 800-171 AU-2 (Audit Events)

## Policy Violations

Unauthorized access attempts or access misuse will result in:
1. Immediate revocation of access
2. Investigation by Security Officer
3. Disciplinary action up to and including termination
4. Potential legal action if criminal activity suspected

---

## Revision History

| Date | Version | Changes |
|------|---------|---------|
| 2026-09-18 | 1.0 | Initial policy creation |

---

**Policy Owner:** Security Officer, SealGames Studios  
**Approval Date:** 2026-09-18  
**Effective Date:** 2026-09-18  
**Next Review Date:** 2026-12-18
