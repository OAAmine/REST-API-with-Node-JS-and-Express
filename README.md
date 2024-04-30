# Patient Records API

This is a simple Express.js API for managing patient records.

## Endpoints

### GET /records

- **Description**: Retrieve medical records of a patient.
- **Request Headers**:
  - `ssn`: Social Security Number (SSN) of the patient.
  - `firstname`: First name of the patient.
  - `lastname`: Last name of the patient.
- **Request Body**: 
  - `reasonforvisit`: Reason for the request (optional).
- **Response Codes**:
  - `200`: Success, returns medical records.
  - `401`: Unauthorized, first or last name doesn't match SSN.
  - `404`: Not Found, patient not found.
  - `501`: Not Implemented, unable to complete the request.

### POST /

- **Description**: Create a new patient.
- **Request Headers**:
  - `ssn`: Social Security Number (SSN) of the patient.
  - `firstname`: First name of the patient.
  - `lastname`: Last name of the patient.
  - `phone`: Phone number of the patient.
- **Response Codes**:
  - `200`: Success, returns updated patient records.

### PUT /

- **Description**: Update existing patient phone number.
- **Request Headers**:
  - `ssn`: Social Security Number (SSN) of the patient.
  - `firstname`: First name of the patient.
  - `lastname`: Last name of the patient.
- **Request Body**: 
  - `phone`: New phone number.
- **Response Codes**:
  - `202`: Accepted, returns updated patient records.
  - `401`: Unauthorized, first or last name doesn't match SSN.
  - `404`: Not Found, patient not found.

### DELETE /

- **Description**: Delete patient records.
- **Request Headers**:
  - `ssn`: Social Security Number (SSN) of the patient.
  - `firstname`: First name of the patient.
  - `lastname`: Last name of the patient.
- **Response Codes**:
  - `200`: Success, patient records successfully deleted.
  - `401`: Unauthorized, first or last name doesn't match SSN.
  - `404`: Not Found, patient not found.

## Usage

1. Run the server by executing the script in a Node.js environment.
2. Use an API testing tool like Postman to interact with the endpoints.

## Dependencies

- `express`: For building the RESTful API.
- `body-parser`: For parsing request bodies.

## Disclaimer

This code is provided for educational purposes only. Please use responsibly and ensure compliance with applicable laws and regulations regarding patient data privacy and security.
