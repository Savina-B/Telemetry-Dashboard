# Telemetry-Dashboard

**Overview**

This project is an interactive telemetry and usage analytics dashboard built with Dash to monitor application adoption, user activity, and engagement trends across a multi-app environment.

The dashboard provides both high-level system metrics (users, applications, server context) and deep-dive analytics at individual application level, including time-series analysis and user interaction breakdowns.

⚠️ **Note**:
This public version uses anonymised and/or representative data. All organisation-specific identifiers, internal infrastructure details, and proprietary logic have been removed or abstracted.

**Key Features**

- System-level metrics
  - Summary cards for total users, licensed users, app count, and server identifier

- Application metrics table
  - Searchable and sortable grid showing usage statistics per application

- User Actions View (modal)
  - Cross-application time-series analysis with date filtering and export

- App-level deep dive
  - Views over time
  - User breakdown
  - Filter by user inclusion/exclusion
  - Downloadable datasets (CSV)

- Live refresh pattern
  - Periodic data refresh via dcc.Interval
  - Dynamic UI updates without page reload

**Tech Stack**
- Python
- Dash
- Dash Design Kit
- Dash Bootstrap Components
- Dash Mantine Components
- Pandas

**Architecture & Design**
- Modular callback structure separating:
  - Global analytics
  - App-specific analytics
  - UI state handling

- Data abstraction layer (CSV / DB interchangeable)

- Scalable layout designed for multi-application environments

- Export-friendly outputs for downstream analysis

**Data Handling & Anonymisation**

To make this repository public-safe:

- Organisation names and logos removed

- Internal server names replaced with placeholders

- Usernames treated as anonymised identifiers

- File paths and helper utilities abstracted

- Database connections replaced with flat-file examples
