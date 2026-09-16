# Functional Requirements

## Mars Rover Mission Control

### FR-01 — Command Execution

The rover shall receive commands from Mission Control and execute valid commands.

### FR-02 — Rover Status Reporting

The rover shall report its current position, battery level, temperature, and communication status.

### FR-03 — Command Authentication

Only authenticated Mission Control operators shall be allowed to issue rover commands.

### FR-04 — Invalid Command Rejection

The system shall reject invalid or unauthorized commands.

### FR-05 — Safe Mode

The rover shall enter Safe Mode when a critical battery or thermal condition is detected.

### FR-06 — Command Execution Status

Mission Control shall receive the command execution status from the rover.

### FR-07 — Mission Event Logging

All commands and critical rover events shall be recorded with a timestamp and operator ID.
