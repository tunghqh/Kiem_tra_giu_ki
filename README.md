# Kiem_tra_giu_ki

# How to run

1. Stop and remove old container: ```docker stop flask-backend && docker rm flask-backend```
1. Build image: ```docker build -t backend .```
1. Run the container: ```docker run -d --name flask-backend -e password=postgres -p 5000:5000 backend```

# Entity
## Customer (BANG 1)
* id: int
* customer_name: string
* contact_name: string
* address: string
* city: string
* postal_code: string
* country: string


# API
## Customer
### Get all customer
* Request
    * Method: GET
    * Endpoint: /customer/all
    * Params: None
    * Body: None
* Response: [Customer]
### Add a customer
* Request
    * Method: POST
    * Endpoint: /customer
    * Body:
        * customer_name: string
        * contact_name: string
        * address: string
        * city: string
        * postal_code: string
        * country: string
* Response: Message
### Update a customer
* Request:
    * Method: PUT
    * Endpoint: /customer/:customer_id
    * Body:
        * customer_name: string
        * contact_name: string
        * address: string
        * city: string
        * postal_code: string
        * country: string
* Response: Message

### Delete a customer
* Request:
    * Method: DELETE
    * Endpoint: /customer/:customer_id
* Response: message


*=======================================================================

# Entity
## Categories (BANG 2)
* category_id: int
* category_name: string
* description: string

# API
## Categories
### Get all categories
* Request
    * Method: GET
    * Endpoint: '/categories/all'
    * Params: None
    * Body: None
* Response: [Categories]
### Add a categories
* Request
    * Method: POST
    * Endpoint: /categories
    * Body:
         * category_name: string
         * description: string

* Response: Message
### Update a categories
* Request:
    * Method: PUT
    * Endpoint: /categories/:category_id
    * Body:
         * category_name: string
         * description: string
* Response: Message

### Delete a categories
* Request:
    * Method: DELETE
    * Endpoint: /categories/:category_id
* Response: message

*=======================================================================

# Entity
## Employees (BANG 3)
* employee_id: int
* lastname: string
* firstname: string
* birthdate: date
* photo: string
* notes: string



# API
## Employees
### Get all employees
* Request
    * Method: GET
    * Endpoint: /employees/all
    * Params: None
    * Body: None
* Response: [Employees]
### Add a employees
* Request
    * Method: POST
    * Endpoint: /employees
    * Body:
         * lastname: string
         * firstname: string
         * birthdate: date
         * photo: string
         * notes: string
         * Response: Message
### Update a employees
* Request:
    * Method: PUT
    * Endpoint: /employees/:employee_id
    * Body:
         * lastname: string
         * firstname: string
         * birthdate: date
         * photo: string
         * notes: string
         * Response: Message
* Response: Message

### Delete a employees
* Request:
    * Method: DELETE
    * Endpoint: /employees/:employee_id
* Response: message


*=======================================================================

