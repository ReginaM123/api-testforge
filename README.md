 API TestForge

A lightweight API testing framework for validating REST APIs using simple YAML files.

 Features

* GET, POST, PUT, PATCH, DELETE support
* YAML test definitions
* JSON response assertions
* Environment configuration
* Report generation
* CI/CD integration

 Installation

```bash
git clone https://github.com/yourname/api-testforge.git
cd api-testforge

python -m venv venv

 Linux/macOS
source venv/bin/activate

 Windows
venv\Scripts\activate

pip install -r requirements.txt
```

 Project Structure

```text
api-testforge/
├── src/
│   ├── client/
│   ├── assertions/
│   ├── runners/
│   ├── reports/
│   └── config/
├── tests/
├── reports/
├── docs/
├── examples/
├── main.py
└── requirements.txt
```

 Running Tests

```bash
python main.py run tests/users_api.yaml
```

 Example Test

```yaml
name: Get User

request:
  method: GET
  url: https://jsonplaceholder.typicode.com/users/1

assertions:
  - status_code: 200
```

 Generate Report

```bash
python main.py run tests/users_api.yaml
```

Reports are automatically generated in the reports directory.

 Future Roadmap

* OAuth2 support
* Swagger/OpenAPI validation
* Parallel execution
* Docker support
* Web dashboard
* AI-generated test cases

