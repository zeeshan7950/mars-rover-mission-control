# Mars Rover Mission Control
SVV Requirements Verification and Change Impact Analysis for Mars Rover Mission Control
# Mars Rover Mission Control

## Project Overview

Mars Rover Mission Control is a software system designed to remotely control and monitor exploration rovers on Mars.

The system allows Mission Control operators to send commands, receive rover status information, detect communication failures, protect the rover through Safe Mode, and record mission events.

## Mission 1 — Analyze the Engineering Note

### Functional Requirements

1. The rover shall receive and execute valid commands.
2. The rover shall report its current position, battery level, temperature, and communication status.
3. Only authenticated operators shall be allowed to issue commands.
4. The system shall reject invalid or unauthorized commands.
5. The rover shall enter Safe Mode during critical battery or thermal conditions.
6. Mission Control shall receive command execution status.
7. Commands and critical rover events shall be recorded with timestamp and operator ID.

### Non-Functional Requirements

1. The system shall continue operating despite temporary communication interruptions.
2. Only authenticated operators shall be permitted to issue commands.
3. Command processing should normally complete within 5 seconds.
4. The system should support communication with multiple rovers simultaneously.

## Mission 2 — Change Requests

### CR-01 — Emergency Safety

Safe Mode must now be activated within 3 seconds when the battery temperature exceeds the critical threshold or battery capacity falls below the emergency level.

### CR-02 — Mission Expansion

The system must support at least 20 simultaneously connected rovers.

### CR-03 — Security Upgrade

The system must require both authentication and role authorization before accepting rover commands.

## Change Impact Summary

| Change Request | Affected Areas                                                            |
| -------------- | ------------------------------------------------------------------------- |
| CR-01          | Requirement, Safe Mode Design, Code, Test Cases                           |
| CR-02          | Requirement, System Architecture, Communication Design, Performance Tests |
| CR-03          | Requirement, Security Design, Authorization Code, Security Tests          |

## Repository Structure

```text
requirements/
├── functional-requirements.md
└── non-functional-requirements.md

change-requests/
└── change-requests.md

traceability/
└── traceability-matrix.md
```
