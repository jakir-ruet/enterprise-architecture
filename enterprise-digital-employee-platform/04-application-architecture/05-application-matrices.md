# Application Architecture Matrices

## Application / Organization

| Application | Employee | Manager |   HR | Payroll |   IT |
| ----------- | -------: | ------: | ---: | ------: | ---: |
| Portal      |        X |       X |    X |         |      |
| IAM         |        X |       X |    X |       X |    X |
| HR Core     |          |         |    X |         |    X |
| Leave       |        X |       X |    X |         |      |
| Performance |        X |       X |    X |         |      |
| Recruitment |          |       X |    X |         |      |
| Payroll     |          |         |      |       X |    X |
| Analytics   |          |       X |    X |       X |    X |

## Application / Data

| Application   | Employee | Payroll | Leave | Performance | Recruitment |
| ------------- | -------: | ------: | ----: | ----------: | ----------: |
| HR Core       |        X |         |       |             |             |
| Payroll       |        X |       X |       |             |             |
| Leave         |        X |         |     X |             |             |
| Performance   |        X |         |       |           X |             |
| Recruitment   |        X |         |       |             |           X |
| Data Platform |        X |       X |     X |           X |           X |
