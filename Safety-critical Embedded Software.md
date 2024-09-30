---
created: 2024-09-30T08:50
updated: 2024-09-30T09:06
---

# Safety-Critical Embedded Software

## Characteristics

- DO-178C, EN-50128, IEC-61508, ISO-26262, …
- Maintained for decades

Most safety critical applications are [[Digital Controller|digital controllers]]

## Avionics Certification Standard

- DO-178C; Supplements: DO-330, DO-331, DO-332, DO-333
- Design Assurance Level
- Tool Qualification Level (DO-330)

## Tools

- SCADE (Safety Critical Application Development Environment)
    - Synchronous language
    - Dialect of Lustre with major extensions (state machines, arrays)
    - Direct correlation between block diagrams and state machines
    - Software runs in finite memory with bounded reaction time, deterministic
    - _Can be used to develop safety critical software without having to verify its output_
