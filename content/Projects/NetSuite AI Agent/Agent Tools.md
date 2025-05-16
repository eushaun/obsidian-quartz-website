### Tools / Functions

#### Databricks tools documentations:
[Create custom AI agent tools with Unity Catalog functions | Databricks Documentation](https://docs.databricks.com/aws/en/generative-ai/agent-framework/create-custom-tool)
[Connect AI agent tools to external services | Databricks Documentation](https://docs.databricks.com/aws/en/generative-ai/agent-framework/external-connection-tools#-create-a-tool-in-agent-code)

1. GET calls
    - To get internal IDs for subsidiary, department, location, etc.
    - To search for newly created transaction once created
2. Build JSON payload
    - **Option 1:** Create vector search index containing schema and endpoint for transactions we want (salesOrd, transferOrd, inventoryAdj, etc)
    - **Option 2:** Create functions containing JSON payload for each transaction type
3. Item ID mapping
    - **Option 1:** Upload csv file with mapping
    - **Option 2:** Create GET call to search everytime
	- **Hybrid:** Create bulk GET call at the start to update CSV mapping
4. POST calls
    - To create transaction