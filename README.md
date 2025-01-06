# final

# Project Name: IdeaSphere

## Overview
This project is a web application designed for [brief description of the project]. It provides a user-friendly interface and efficient functionality for [purpose of the application].

## Endpoints

The application exposes the following endpoints for interacting with the server:

### 1. **Individual Competition CRUD**
- **Create Competition**: `POST /competitions`
- **Read Competition**: `GET /competitions/{id}`
- **Update Competition**: `PUT /competitions/{id}`
- **Delete Competition**: `DELETE /competitions/{id}`
- **Extend Competition**: `POST /individual-competition/extend-competition`
- **Cancel Competition**: `DELETE /individual-competition/cancel-competition/{id}`

### 2. **Individual Organizer CRUD**
- **Create Organizer**: `POST /organizers`
- **Read Organizer**: `GET /organizers/{id}`
- **Update Organizer**: `PUT /organizers/{id}`
- **Delete Organizer**: `DELETE /organizers/{id}`

### 3. **Monthly Draw CRUD**
- **Create Monthly Draw**: `POST /monthly-draws`
- **Read Monthly Draw**: `GET /monthly-draws/{id}`
- **Update Monthly Draw**: `PUT /monthly-draws/{id}`
- **Delete Monthly Draw**: `DELETE /monthly-draws/{id}`
- **Get All Monthly Draws**: `GET /monthlyDraw/get-all-monthly-draws`
- **Get Eligible Monthly Draws**: `GET /monthlyDraw/eligible`
- **Find Draws by Prize or Name**: `GET /monthlyDraw/findDrawsByPrizeOrName/{prize}/{name}`
- **Find Draws by Prize or Name (Gift Card)**: `GET /monthlyDraw/findDrawsByPrizeOrName/Gift Card`
- **Find Draws by Prize or Name (Lucky Draw)**: `GET /monthlyDraw/findDrawsByPrizeOrName/Lucky Drawd`

### 4. **Monthly Draw Participant CRUD**
- **Create Participant**: `POST /monthly-draw-participants`
- **Read Participant**: `GET /monthly-draw-participants/{id}`
- **Update Participant**: `PUT /monthly-draw-participants/{id}`
- **Delete Participant**: `DELETE /monthly-draw-participants/{id}`
- **Get All Monthly Draw Participants**: `GET /monthly-draw-participants`

You can find detailed documentation for the API in the link below:

- [Postman API Documentation](https://documenter.getpostman.com/view/39709949/2sAYJAcwWX)

## User Interface
The project’s user interface is designed with a focus on simplicity and usability. You can explore the design on Figma:

- [Figma Design Prototype](https://www.figma.com/proto/oUBCUch383eDZlzbEHI1jv/IdeaSphere?node-id=61-497&p=f&t=1zzA4JYAwr813AdI-1&scaling=contain&content-scaling=fixed&page-id=0%3A1)

## Presentation
A detailed presentation of the project, including goals and outcomes, can be found at the following link:

- [Canva Presentation](https://www.canva.com/design/DAGbau1CiMA/fg470odHkUVnt0vgD1Unmg/edit?utm_content=DAGbau1CiMA&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)

## Installation
### Prerequisites
- Node.js
- Java (if applicable)
- Any other software or libraries required for your project.

### Steps
1. Clone the repository: `git clone <repository-url>`
2. Navigate to the project directory.
3. Install the required dependencies: `npm install` or equivalent.
4. Start the application: `npm start` or equivalent.

## Contributing
If you would like to contribute to this project, please fork the repository and submit a pull request with your proposed changes.

## License
Include licensing information if applicable.
