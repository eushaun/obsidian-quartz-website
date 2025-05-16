1. Ask user what transaction to create
2. Get inputs from user (subsidiary, department, location, status, date, items, quantity, etc)
    1. + any other fields
    2. + Any other fields
3. If unable to get internal ID mapping for any field, ask if user would like to change or input their own internal ID
4. Ask if sandbox or production
5. Confirm inputs / JSON payload to user
6. Create transaction
    1. If success, return tranId and URL to new transaction
    2. If error, provide error message and explanation