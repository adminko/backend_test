# Api server

## Description

Test API server for Backend test task

## Server

```
http://localhost:3000/
```

## Authorization

For each request use specific header
```
X-Client: 237cd6a8-5a0e-4ff0-b7e2-0bf34675d058
```

## Enpoints
### Get users

`GET /users?page=5`

```json
{
  "users":[
    {
      "Id":"5a963e9b-ac97-4bd3-94af-64513f4ee3a0",
      "LastName":"Axelroad",
      "FirstName":"Robert",
      "Email":"b.axelroad@example.com"
    },
    ...
  ]
}
```

### Get companies


`GET /companies?page=5`

```json
{
  "companies":[
    {
      "Id":"1ee15eed-6baa-4732-afc0-f12c35b7dc25",
      "Name":"Mixtape Inc.",
      "Address":"1693 Alice Court, Annapolis MD 21401"
    },
    ...
  ]
}
```

### Get company positions
`GET /company/{company_id}`

```json
{
  "positions":[
    {
      "CompanyId":"6e285aea-6487-4771-8062-f782e43792bc",
      "UserId":"5a963e9b-ac97-4bd3-94af-64513f4ee3a0",
      "Position":"CEO"
    },
    ...
  ]
}
```
