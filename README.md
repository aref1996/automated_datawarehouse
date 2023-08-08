# automated_datawarehouse
1. Project Goal:
To design and implement an automated data warehouse system that, when provided with entity specifications, can generate SQL queries tailored to the user's reporting needs.

2. Project Description:
The automated data warehouse system is designed to understand and interact with a given database. It focuses on:

    Allowing users to define entities, which are anticipated to correspond to columns in the tables that bear the same name.
    Letting users specify facts, numerical entities that get integrated into the query.
    Allowing users to determine tables that connect these entities by indicating which tables possess specific entities as their columns.

Given the following example entities:

    shop, city, region, day, month, year, product, category
    And the fact: sales
    Along with the tables:
        Transactions (containing sales, product, shop, day)
        Time (containing day, month, year)
        Product (containing product, category)
        Location (containing shop, city, region)

Users can request a specific report by specifying the entities they wish to be displayed. For instance, if someone wants the total monthly sales delineated by region, they would input "sales, region, month". The system then processes this request and outputs the correct SQL query to fetch the required data, ensuring the tables are joined appropriately to obtain the stipulated entities.

3. Project Success:
The project was successful as it efficiently generated accurate SQL queries based on user-defined entity specifications. By automating the process of query generation, it eradicated the need for manual coding, reducing errors and saving time. The system adeptly identified which tables to join and how to do so, ensuring that the generated queries fetched the precise data as requested by users. This system brought about a more user-friendly approach to report generation and data fetching, streamlining the data analysis process.
