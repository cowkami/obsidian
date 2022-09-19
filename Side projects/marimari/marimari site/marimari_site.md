## requirements
### for Users 
 - view opening date/time
 - view news
 - view menu
 - view location

### for Admin
- edit opening date/time
	- date
	- time
	- branch
- edit news
	- title
	- body
- edit menu
- edit branch information
	- name
	- location
- edit admin user
	- name
	- role
	- permissions

## architecture


```mermaid
graph LR
admin([Admin]) -->|request| lambda_be[AWS Lambda Backend]
lambda_be -->|admin page| admin
lambda_be --> db[(DB)]
db --> lambda_be

user([User]) -->|request| lambda_be
lambda_be -->|website| user

```
