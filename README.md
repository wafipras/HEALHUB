
# HEALHUB-API


## Deployment

1. Method POST 
Path /register

Input
```bash
  {
  "username": "namefour",
  "email": "fourname@example.com",
  "password": "password"
}
```
Output
```bash
 {
    "status": "success",
    "message": "User registered successfully"
}
```
2. Method POST
Path /login

Input
```bash
 {
  "email": "fourname@example.com",
  "password": "password"
}
```
Output
```bash
 {
    "status": "success",
    "message": "Login successful"
}
```
3. Method POST
Path /predictions

**_NOTE: The input can only 4 to 6 Number "1" and the rest is "0" until 70 numbers_** 

Input
```bash
 {
    "inputData": [
        1, 0, 1, 0, 0, 0, 0, 1, 0, 1,
        0, 0, 0, 1, 0, 0, 0, 0, 0, 0,
        0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
        0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
        0, 0, 0, 0, 0, 0, 1, 0, 0, 0,
        0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
        0, 0, 0, 0, 0, 0, 0, 0, 0, 0
    ]
}
```
Output
```bash
 {
    "status": "success",
    "message": "Model is predicted successfully",
    "data": {
        "id": "3e66798d-19a7-443a-a701-eb7cae29b458",
        "classResult": 15,
        "label": "Paru-Paru Basah",
        "createdAt": "2024-06-13T12:23:50.127Z"
    }
}
```
4. Method GET
Path /predict/histories

Output
```bash
 {
    "status": "success",
    "data": [
        {
            "id": "fbad58cc-6650-44be-8e61-43a85153d7cc",
            "history": {
                "createdAt": "2024-06-12T13:49:28.162Z",
                "classResult": 18,
                "id": "fbad58cc-6650-44be-8e61-43a85153d7cc",
                "label": "Tuberkulosis"
            }
        }
    ]
}
```
