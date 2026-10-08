# Data Entities

| Entity       | Key Attributes                         | Owner   | Sensitivity         |
| ------------ | -------------------------------------- | ------- | ------------------- |
| Employee     | employee_id, name, status              | HR      | Confidential        |
| Organization | org_id, name, parent                   | HR      | Internal            |
| Position     | position_id, title, grade              | HR      | Internal            |
| Employment   | employee_id, start, end, type          | HR      | Confidential        |
| Payroll      | employee_id, period, gross, net        | Payroll | Highly Confidential |
| Leave        | leave_id, employee_id, type, dates     | HR      | Confidential        |
| Attendance   | employee_id, date, status              | HR      | Confidential        |
| Performance  | employee_id, goals, rating             | HR      | Highly Confidential |
| Candidate    | candidate_id, status, application      | HR      | Confidential        |
| Benefit      | employee_id, benefit_type, eligibility | HR      | Confidential        |
