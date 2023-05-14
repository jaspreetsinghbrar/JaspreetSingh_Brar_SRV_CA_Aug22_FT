**Hosted Link**

https://raspberry-dugong-fez.cyclic.app/

**Endpoints**

The following endpoints are available:

- **POST /participants/add** - adds a participant to the database.
- **GET /participants** - returns a list of all participants.
- **GET /participants/details** - returns a list of all participants' personal details.
- **GET /participants/details/deleted** - returns a list of all deleted participants' personal details.
- **GET /participants/details/:email** - returns the personal details of a single participant.
- **GET /participants/work/:email** - returns the work details of a single participant.
- **GET /participants/home/:email** - returns the work details of a single participant.
- **DELETE /participants/:email** - delete a single participant (soft delete).
- **PUT /participants/:email** - update a single participant.

**Validation**

The API includes three functions for validating email addresses, dates, and objects with empty properties.

**Responses**

Responses to valid requests include a status and a data property, which contains the results of the request. In the case of an error, a status and a message are sent instead.

**Object Design**
{
"personal": {
"email": "test@test.com",
"first_name": "f_name",
"last_name": "l_name",
"dob": "1998/12/01"
},
"work": {
"company_name": "cname",
"salary": "100000",
"currency": "USD"
},
"home": {
"country": "UK",
"ciry": "London"
},
"active": true
}

**Env**
AWS_REGION=ap-southeast-1
AWS_ACCESS_KEY_ID=ASIAWHQT5GFGUEJPUKBO
AWS_SECRET_ACCESS_KEY=S5yTLtQFouBYFtc6NLN3Q+vpUWpqcsOS9Upp+h6z
AWS_SESSION_TOKEN=IQoJb3JpZ2luX2VjEM3//////////wEaCmFwLXNvdXRoLTEiRzBFAiEAtvZvADTF3l658nP/Ju6bRl/niLjiY7rHrQ/Po0pNz3ACIAcwlgV+ZajYyyzwCssxw7cZdLGqqP2gsQUgU/ihZGsTKrcCCOf//////////wEQABoMNDI4NDY0NzQ2ODI5IgyVzDBWBWtDos+dCEkqiwKsy4CXqWK2wp3NThRov7SwQOva3Wv/2AEvRihUeeR3sr5Hto4mO8bp8XNrLhLhDFtSA0aUeeMudpqgB/zsR89hzBO4D6Up6yxMOS0GDC3JLfKi0KcnW6RGbs6y2IiY5FuVcLqJbc4nVl7t9H8SSsvGqMGcMdGwHm4xIXArQ4IURUhwynpDYvTkuOyGPF1QswJbU6EkdWeLFaUCzerQqPoJqgxiRb05UqiRPYBlZNjFyq0iGE7C8XSgepN2wODn3fHY/fVqLeM6WHMrW6jCHjk2+9c0jMM2SU17KTGoQsUu69K5pl7QSvekAVA++SDTqYT2skA+CCRncyY+zm9KzJOUpxO5E96S4Y2qSUUwyuGBowY6nQHIKsaWCYCOatNaYsV9H0dB+3xk/Fg3quw5ZeHLrd9M/JqLmtrrEB4X62AhcvqGVmZIG7QgjZepqIpPixl1V24Lay+w3Ad8F+UN6sLkaqTLxMFJ91ea9d9UCK6F5K2XNoCSnmdiyew0/NwCpZiSrik3HaZB6c/XCPftlswEdoKXJMGgg489hJcDZ1+0arYaQPAZw2H2gkFDfSWs0qze
