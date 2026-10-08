# Application Services

| Service          | Provider             | Consumers             |
| ---------------- | -------------------- | --------------------- |
| Employee Profile | HR Core              | Portal, HR, Analytics |
| Organization     | HR Core              | Portal, Analytics     |
| Leave Balance    | Leave Service        | Portal, Manager       |
| Leave Request    | Leave Service        | Employee, Manager     |
| Attendance       | Attendance Service   | HR, Manager           |
| Payroll Summary  | Payroll Integration  | Employee, HR          |
| Performance      | Performance Service  | Employee, Manager, HR |
| Recruitment      | Recruitment Service  | Recruiter, Manager    |
| Identity         | IAM                  | All applications      |
| Notification     | Notification Service | Business services     |
| Reporting        | Analytics            | Management, HR        |

## Service Design Principles

- Business capability aligned
- Reusable
- Governed
- Secure
- Observable
- Versioned
