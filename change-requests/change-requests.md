# Change Requests

## CR-01 — Emergency Safety

### Original Requirement

**FR-04:**
The rover shall enter Safe Mode when a critical battery or thermal condition is detected.

### New Requirement

**FR-04:**
The rover shall enter Safe Mode within 3 seconds when battery temperature exceeds the critical threshold or battery capacity falls below the defined emergency level.

### Impact

The requirement becomes measurable because a specific response time of 3 seconds is defined. The Safe Mode implementation and test cases will need to be reviewed.

---

## CR-02 — Mission Expansion

### Original Requirement

**NFR-04:**
The system shall support communication with multiple rovers simultaneously.

### New Requirement

**NFR-04:**
The system shall support at least 20 simultaneously connected rovers.

### Impact

The requirement is now measurable. The system architecture, communication resources, performance configuration, and testing need to support at least 20 connected rovers.

---

## CR-03 — Security Upgrade

### Original Requirement

**NFR-02:**
Only authenticated Mission Control operators shall be permitted to issue rover commands.

### New Requirement

**NFR-02:**
The system shall require authenticated and role-authorized operators before accepting rover commands.

### Impact

The security design and command authorization logic need to be reviewed. Test cases must verify both authentication and operator role authorization.
