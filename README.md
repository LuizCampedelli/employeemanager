# Employeemanager api

This is the README file for the `employeemanager` project.

## Description

The `employeemanager` project api is a software application that helps manage employee information. It provides functionality to add, update, and delete employee records, as well as view employee details and enable export the data to a file in the root of the project.

## Stack

**Back-end:** Java 17, MySql8

1. Java 17: https://www.oracle.com/br/java/technologies/downloads/
2. MySQL 8: https://dev.mysql.com/downloads/installer/

## Local deploy

To install and run the `employeemanager` project api, follow these steps:

1. Clone the repository: `git clone https://github.com/LuizCampedelli/employeemanager.git`
2. Navigate to the project directory: `cd employeemanager`
3. If you are using VSCode, type: `code .`, than install Extension Pack for Java, in the left panel click in Run and Debug.
4. If you are in Intellij IDEA, just hit the play green button.

## Usage
```
Once the API is running, you can access it by opening Insominia or using HTTPie in terminal.
To use Insominia, download it from: https://insomnia.rest/
To use HTTPie, download it from: https://httpie.io/cli
```

### Using Httpie

#### Return all employees

```http
  http :8080/employee/all
```

| Parâmetro   | Descrição                           |
| :---------- | :---------------------------------- |
| `GET` | Return all employees|

#### Add an employee

```http
  http POST :8080/employee/add < data.json
```

| Parâmetro   | Descrição                           |
| :---------- | :---------------------------------- |
| `POST`      | Add employee using parameters from data.json |

#### Update an employee

```http
  http :8080/employee/update < data.json
```

| Parâmetro   | Descrição                           |
| :---------- | :---------------------------------- |
| `PUT` | Update employee with changed parameters from data.json |

#### Delete an employee

```http
  http DELETE :8080/employee/delete/{id}
```

| Parâmetro   | Descrição                           |
| :---------- | :---------------------------------- |
| `DELETE` | Delete employee by id |

#### Export employees to a file.

```http
  http :8080/employee/export
```

| Parâmetro   | Descrição                           |
| :---------- | :---------------------------------- |
| `GET` | Export all employees to an file named employee.json to the root folder |

### Using Insominia

#### Return all employees

```http
  http://localhost/employee/all
```

| Parâmetro   | Descrição                           |
| :---------- | :---------------------------------- |
| `GET` | Return all employees|

#### Add an employee

```http
  http://localhost/employee/add < data.json
```

| Parâmetro   | Descrição                           |
| :---------- | :---------------------------------- |
| `POST`      | Add employee using parameters from data.json |

#### Update an employee

```http
  http://localhost/update < data.json
```

| Parâmetro   | Descrição                           |
| :---------- | :---------------------------------- |
| `PUT` | Update employee with changed parameters from data.json |

#### Delete an employee

```http
 http://localhost/employee/delete/{id}
```

| Parâmetro   | Descrição                           |
| :---------- | :---------------------------------- |
| `DELETE` | Delete employee by id |

#### Export employees to a file.

```http
  http://localhost/employee/export
```

| Parâmetro   | Descrição                           |
| :---------- | :---------------------------------- |
| `GET` | Export all employees to an file named employee.json to the root folder |




# Diagrama API:


![Diagram - Emplyee Manager API drawio](https://github.com/LuizCampedelli/employeemanager/assets/108758747/d461cadf-5532-478d-af13-b4b90d530e8e)


## Contributing

If you would like to contribute to the `employeemanager` project, please follow these guidelines:

1. Fork the repository.
2. Create a new branch: `git checkout -b feature/your-feature-name`
3. Make your changes and commit them: `git commit -m "Add your commit message"`
4. Push to the branch: `git push origin feature/your-feature-name`
5. Submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).
