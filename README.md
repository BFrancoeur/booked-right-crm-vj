# BookedRight CRM App - the Vanilla JavaScript version

An alternative build of the BookedRight app without the additional overhead of libraries and frameworks. 



## Architecture

This app will be built with a core that houses features and functions that will be used across some or all of the software. Non-core features and functionality will be packaged as modules that can be 'plugged in' with an import statement at the top of each file. 



## Technology Stack

The stack is as follows: 

    - Prisma for Object-Relational Mapper (ORM)
        - Maps database to code to simplify the creation of queries
    - Supabase for Backend as a Service (BaaS)
        - Hosts Postgres database
        - File storage
        - Authentication
        - Auto-generated APIs
        - Row Level Security (RLS)
        - Built-in subscriptions to database changes via WebSockets
    - Postgres for the database (runs in Supabase)
        - ORM maps db to Typescript or JavaScript for simpler data querying and modeling
        - Connects to any database, including Postgres
        - Queries run server-side through Prisma Client to generate SQL queries
        - Must implement authentication logic or integrate a third-party provider (Supabase)
        - Must set up a WebSocket server or polling mechanism



## Scripts to be used

    - JavaScript
    - HTML5
    - CSS3


## Foreseeable challenges

    - Authentication
    - APIs
    - API Routes



## Basic Structure 

-- app
    |-- core
    |-- models
    |-- routes
    |-- views
    |-- apis
    |-- templates
    |-- modules
        |-- crm
        |-- payment processing
        |-- chatbot
        |-- dynamic updates
