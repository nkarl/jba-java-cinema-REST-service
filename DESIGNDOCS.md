## Design Docs for Project: Cinema Room REST Service
This project conists of four stages.

### Stage 1/4: Construct a a virtual movie theater with REST service.
This movie theater shall have 9 rows,9 seats for each row.  In this stage I will need to create a simple *endpoint* to return the information about the cinema in JSON format.

#### Implementation
I need to implement the `/seats` endpoint that handles `GET` requests and returns the information about the movie theater.

The response should contain these following information:
    - rows
    - columns
    - available seats

The response is a JSON object and has format similar to this:
```
{
   "total_rows":5,
   "total_columns":6,
   "available_seats":[
      {
         "row":1,
         "column":1
      },

      ........

      {
         "row":5,
         "column":5
      },
      {
         "row":5,
         "column":6
      }
   ]
}
```
