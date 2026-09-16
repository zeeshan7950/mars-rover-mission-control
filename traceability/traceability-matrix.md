# Traceability Matrix

| Requirement | Type           | Change Request | Design Impact                          | Test Impact                                                  |
| ----------- | -------------- | -------------- | -------------------------------------- | ------------------------------------------------------------ |
| FR-01       | Functional     | None           | Command processing module              | Test valid command execution                                 |
| FR-02       | Functional     | None           | Rover status monitoring                | Test position, battery, temperature and communication status |
| FR-03       | Functional     | None           | Authentication module                  | Test authenticated operator access                           |
| FR-04       | Functional     | CR-01          | Safe Mode control logic                | Test Safe Mode activation within 3 seconds                   |
| FR-05       | Functional     | None           | Safe Mode mechanism                    | Test critical battery and thermal conditions                 |
| FR-06       | Functional     | None           | Command status reporting               | Test command execution status                                |
| FR-07       | Functional     | None           | Event logging system                   | Test timestamp and operator ID logging                       |
| NFR-01      | Non-Functional | None           | Communication recovery mechanism       | Test temporary communication interruption                    |
| NFR-02      | Non-Functional | CR-03          | Authentication and role authorization  | Test authentication and role-based authorization             |
| NFR-03      | Non-Functional | None           | Command processing performance         | Test processing time                                         |
| NFR-04      | Non-Functional | CR-02          | Multi-rover communication architecture | Test at least 20 simultaneously connected rovers             |
