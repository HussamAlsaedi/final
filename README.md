# IdeaSphere API Documentation

**System Description**

- IdeaSphere is a dedicated platform that empowers individuals to showcase their creativity and innovation through organizing and participating in competitions across various fields.
- فضاء الحلول هو منصة مخصصة تمكن الأفراد من عرض إبداعاتهم وابتكاراتهم من خلال تنظيم والمشاركة في مسابقات في مختلف المجالات.

## Summary

- **Total Endpoints**: 43
- **Controllers**: 8

---

## Endpoints by Controller

### IndividualCompetitionController

1. **GET** `/competitions` - Get all individual competitions.
2. **POST** `/competitions` - Create a new individual competition.
3. **GET** `/competitions/{id}` - Get individual competition details by ID.
4. **PUT** `/competitions/{id}` - Update competition details.
5. **DELETE** `/competitions/{id}` - Delete an individual competition.
6. **POST** `/individual-competition/extend-competition` - Extend the competition dates and participant numbers.
7. **DELETE** `/individual-competition/cancel-competition/{id}` - Cancel an individual competition.

**Total**: 7 endpoints

### IndividualOrganizerController

1. **GET** `/organizers` - Get all individual organizers.
2. **POST** `/organizers` - Create a new organizer.
3. **GET** `/organizers/{id}` - Get organizer details by ID.
4. **PUT** `/organizers/{id}` - Update organizer details.
5. **DELETE** `/organizers/{id}` - Delete an individual organizer.
6. **POST** `/individual-organizer/send-inquiry` - Send an inquiry to the support team with a subject and message body.
   - **Parameters**:
     - `subject`: The subject of the inquiry (e.g., "sign up page not working").
     - `text`: The body of the inquiry (e.g., "sign up page not working, please fix it as soon as possible").
   - **Example URL**: `POST http://localhost:8080/api/v1/individual-organizer/send-inquiry?subject=sign up page not working&text=sign up page not working, please fix it as soon as possible`

**Total**: 6 endpoints

### MonthlyDrawController

1. **GET** `/monthlyDraw/get-all-monthly-draws` - Get all monthly draws.
2. **GET** `/monthlyDraw/eligible` - Get eligible monthly draws.
3. **GET** `/monthlyDraw/findDrawsByPrizeOrName/{prize}/{name}` - Find monthly draws by prize or name.
4. **GET** `/monthlyDraw/findDrawsByPrizeOrName/Gift Card` - Find monthly draws for "Gift Card".
5. **GET** `/monthlyDraw/findDrawsByPrizeOrName/Lucky Drawd` - Find monthly draws for "Lucky Draw".

**Total**: 5 endpoints

### MonthlyDrawParticipantController

1. **POST** `/monthly-draw-participants` - Create a new participant for monthly draw.
2. **GET** `/monthly-draw-participants/{id}` - Get participant details by ID.
3. **PUT** `/monthly-draw-participants/{id}` - Update participant details.
4. **DELETE** `/monthly-draw-participants/{id}` - Delete a monthly draw participant.
5. **GET** `/monthly-draw-participants` - Get all monthly draw participants.

**Total**: 5 endpoints

### SchedulerService

1. **Automatically scheduled task**: `checkLatePaymentCompetition` - Check and update competitions with late payments.
2. **Automatically scheduled task**: `assignMonthlyWinner` - Assign the winner for the monthly draw based on predefined criteria.

**Total**: 2 tasks (automated, not API endpoints)

---

**Grand Total (API Endpoints)**: 43
