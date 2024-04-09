# employeemanager

This is the README file for the `employeemanager` project.

## Description

The `employeemanager` project api is a software application that helps manage employee information. It provides functionality to add, update, and delete employee records, as well as view employee details and enable export the data to a file in the root of the project.

## Installation

To install and run the `employeemanager` project api, follow these steps:

1. Clone the repository: `git clone https://github.com/LuizCampedelli/employeemanager.git`
2. Navigate to the project directory: `cd employeemanager`
3. If you are using VSCode, type: code ., than install Extension Pack for Java, in the left panel click in Run and Debug.
4. If you are in Intellij IDEA, just hit the play green button.

## Usage

Once the API is running, you can access it by opening Insominia or using HTTPie in terminal.
To use Insominia, download it from: https://insomnia.rest/
To use HTTPie, download it from: https://httpie.io/cli

In Httpie, using the following commands:
http :8080/employee/all - it will display all employees in the application.
http POST :8080/employee/add < data.json - where i can write the data.json to add more employees.
http PUT :8080/employee/update < data.json - where i can change parameters, like email, name etc.
http DELETE :8080/employee/delete/{id} - {id} = a number, like 55
http :8080/employee/export - it will export all employees to a file in root of the project, named employee.json

In Insominia, using the following commands:
GET http://localhost:8080/employee/all - to show all employees
POST http://localhost:8080/employee/add - adding the JSON text
PUT http://localhost:8080/employee/update - adding the JSON text + the proper id to update
DELETE http://localhost:8080/employee/delete/{id} - {id} = a number, like 55
GET http://localhost:8080/employee/export - it will export all employees to a file in root of the project, named employee.json



## Contributing

If you would like to contribute to the `employeemanager` project, please follow these guidelines:

1. Fork the repository.
2. Create a new branch: `git checkout -b feature/your-feature-name`
3. Make your changes and commit them: `git commit -m "Add your commit message"`
4. Push to the branch: `git push origin feature/your-feature-name`
5. Submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).
