# IdeaSphere API Documentation

**System Description**

- IdeaSphere is a dedicated platform that empowers individuals to showcase their creativity and innovation through organizing and participating in competitions across various fields.
- فضاء الحلول هو منصة مخصصة تمكن الأفراد من عرض إبداعاتهم وابتكاراتهم من خلال تنظيم والمشاركة في مسابقات في مختلف المجالات.

## Summary

- **Total Endpoints**: 28
- **Controllers**: 7

---

## Endpoints by Controller

### IndividualOrganizerController

1. **POST** `/individual-organizer/register` - Register a new individual organizer.
2. **GET** `/individual-organizer/get-profile` - Get the profile of the authenticated individual organizer.
3. **PUT** `/individual-organizer/update` - Update the profile of the authenticated individual organizer.
4. **POST** `/individual-organizer/send-inquiry` - Send an inquiry to the support team with a subject and message body.
   - **Example URL**: `POST http://localhost:8080/api/v1/individual-organizer/send-inquiry?subject=sign up page not working&text=sign up page not working, please fix it as soon as possible`

**Total**: 4 endpoints

### IndividualCompetitionController

1. **GET** `/individual-competition/get` - Get all individual competitions.
2. **GET** `/competition-payment/get-my-competition-payment-individual` - Get payment details for the authenticated individual.
3. **GET** `/individual-competition/get-my-competitions` - Get competitions for the authenticated individual.
4. **GET** `/individual-competition/get-competitions-by-status/Waiting payment` - Get individual competitions with a status of "Waiting payment".
5. **POST** `/individual-competition/add` - Create a new individual competition.
6. **POST** `/individual-competition/add-competition-payment` - Add competition payment details.
7. **PUT** `/individual-competition/update` - Update individual competition details.
8. **PUT** `/individual-competition/cancel-competition/1` - Cancel a competition with the given ID (e.g., "1").
9. **POST** `/individual-competition/extend-competition` - Extend the competition dates and participant numbers.

**Total**: 9 endpoints

### MonthlyDrawController

1. **GET** `/monthlyDraw/get-all-monthly-draws` - Get all monthly draws.
2. **GET** `/monthlyDraw/eligible` - Get eligible monthly draws.
3. **GET** `/monthlyDraw/findDrawsByName/Lucky Drawd` - Find monthly draws by name ("Lucky Drawd").
4. **GET** `/monthlyDraw/findDrawsByPrize/Gift Card` - Find monthly draws with "Gift Card" prize.
5. **POST** `/monthlyDraw/add` - Create a new monthly draw.
6. **PUT** `/monthlyDraw/update` - Update monthly draw details.

**Total**: 6 endpoints

### MonthlyDrawParticipantController

1. **POST** `/monthly-draw-participant/add/1` - Add a participant to the monthly draw with a specific ID (e.g., "1").
2. **GET** `/monthlyDrawParticipant/get` - Get details of all monthly draw participants.

**Total**: 2 endpoints

---

**Grand Total (API Endpoints)**: 28
- **Total Endpoints**: 28
- **Controllers**: 7
