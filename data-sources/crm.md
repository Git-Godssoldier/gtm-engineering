# CRM Data Sources

## Salesforce

### Connection
- Use OAuth or Connected App
- REST API: `https://[instance].salesforce.com`

### Key Objects

**Account:**
```javascript
GET /services/data/v58.0/sobjects/Account/{accountId}

Fields: Name, Industry, EmployeeCount, AnnualRevenue, Type, OwnerId
```

**Opportunity:**
```javascript
GET /services/data/v58.0/sobjects/Opportunity/{oppId}

Fields: Name, StageName, Amount, CloseDate, Probability, AccountId
```

**Contact:**
```javascript
GET /services/data/v58.0/sobjects/Contact/{contactId}

Fields: Name, Email, Title, AccountId, OwnerId
```

### Key Queries

**Account Summary:**
```sql
SELECT Id, Name, Industry, Type, Owner.Name,
       (SELECT Id, Name, StageName, Amount FROM Opportunities),
       (SELECT Id, Name, Email FROM Contacts)
FROM Account
WHERE Id = '{accountId}'
```

**Activity History:**
```sql
SELECT Id, Subject, ActivityDate, Description, Owner.Name
FROM Task
WHERE AccountId = '{accountId}'
ORDER BY ActivityDate DESC
LIMIT 50
```

## HubSpot

### Connection
- API Key or Private App token
- REST API: `https://api.hubapi.com`

### Key Objects

**Company:**
```javascript
GET /crm/v3/objects/companies/{companyId}

Properties: name, industry, company_size, annualrevenue
```

**Deal:**
```javascript
GET /crm/v3/objects/deals/{dealId}

Properties: dealname, amount, dealstage, closedate
```

**Contact:**
```javascript
GET /crm/v3/objects/contacts/{contactId}

Properties: firstname, lastname, email, jobtitle
```

## Data Mapping

| Business Concept | Salesforce | HubSpot |
|-----------------|------------|---------|
| Company | Account | Company |
| Deal | Opportunity | Deal |
| Person | Contact | Contact |
| Activity | Task/Event | Engagement |
