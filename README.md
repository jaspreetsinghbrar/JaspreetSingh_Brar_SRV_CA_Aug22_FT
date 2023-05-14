**Hosted Link**

https://lazy-lime-swallow-ring.cyclic.app

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
AWS_REGION=ap-northeast-1
AWS_ACCESS_KEY_ID=ASIAQT3YWULOSGH7L6LM
AWS_SECRET_ACCESS_KEY=+UQixY45GDMOjkVHIFnzSHwIK6w57RZ9QZlselO8
AWS_SESSION_TOKEN=IQoJb3JpZ2luX2VjEL///////////wEaCmFwLXNvdXRoLTEiRzBFAiEA3Rjwwt6PQtQdMCCRsezi7yj0Sj5pcBVvs4EhbsUXnB4CICoONHzChX0dti7d9slNmido5f4bHNuHE/ADioMiK/G7KrkCCNj//////////wEQABoMMDQyNjY1OTQzNzczIgzHXXihiqrGpQ3WnhEqjQJr8qnsbtyUDBp3ZNhoLYf4IO/fIfa0bU9JNrkUqNRCfrJR1DsncSYCOVca3LxUC0M9l4XIS98niXSIG2Djc2JECMuT3yIfRTAtHfxGgdpzEwZYkur4W/4OfKbJ3A7PchlPYSf9AjHKeMWPAvla3UHIWiReWgjfVd48vLY+/i6N4LcOSB7CjLibbNkEgza1r448nXPr4+ObaX7ga+4rxTPN6fFZSgUW0l4SQ2f/rRfCGEC8yiXOa1/D36P30x/xo4aN0FPGucuxRQFgiXefqZhE3U9oiyPI6lUyHMU6W5/RS9TsCRw1neC2DSng5QX34Qx2SsZjehV+JqMIZPF87nnr7IHbw/fdxUSNr+R0ZzDYx/6iBjqdAWujczx4XIxik4ydo3vUZipNNVt+uBFaQrrpDZBv4AOOY7xqg9wC08FnWYAuq/lxRgiCrrIvyHXq43vcpceZQGORk2gYXbNrFKONQ6z8lCvL/+6EngkygeWOZbSds2VF8ZVInHzrlBf1cWR23JTQ+DiRTBOo/BNAycHqrugWVKJ4ICihyLQRVKqbGnLlU/O10ZQNdeHIIthtCx9kYFc=
