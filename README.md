# Name : Abhishek Gurav
# University : Indian Institute of Technology (ISM) Dhanbad
# Department : Environmental Engineering

# Getting Started with Create React App

First download or clone repository.


### `npm install` in client folder then `npm start` in same folder

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

### `npm install` in Server folder then `node app` in same folder

Launches the Backend

# Endpoint
## POST [ ```./user/login-user``` ]
```bash
# On Sucess
{
    status: "ok", 
    data :  <token>
}

# User not Found
{
    message:"User not found"
}

# Error
{
    status: "error", 
    error : 'Invalid username/password'
} 
```
## POST [```./user/register-user```]
```bash
# On Sucess
{
    status: "ok"
}

# User Already Exists
{
    message:"User already exists"
}

# Error
{
    status:"error",
    error : error
} 
```
## POST [```./user/userDetails```]
```bash
# On Sucess
{
    status: "ok",
    data : data
}

# Token Not Found
{
    error:"Invalid token"
}

# Error
{
    status:"error",
    err : err
} 
```
## POST [```./api/sentiment```]
```bash
# On Sucess
{
    intent: {
        intent: <Max name>,
        score: <Max score>
    },
    keywords: [
        { 
            keywords:<word>,
            confidence:<conf score>
        }
    ],
    emotion: {
        emotion: <Max name>,
        score: <Max score>
    }
}

```
