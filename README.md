**Eazi Tour - Backend**
The **Eazi Tour Backend** is responsible for fetching images from the Unsplash API based on user input from the frontend. The backend serves data to the frontend, allowing users to discover destinations via the Eazi Destination Tool (Eazi destination cards show images of random country selections based on the user's continent selection).

**Features**
**Image Search API:** Fetches country-specific images from Unsplash based on queries sent by the frontend.

**Rate Limiting:** Due to the Unsplash API free-tier limitations, the app can only handle 50 requests per hour. Each search request in the Eazi Destination Tool consumes 4 of those available requests.

**API Endpoint**
**/api/photos?query={country-name}:** Fetches an image for the specified country. Example: /api/photos?query=Pakistan.

**Tech Stack**
1. Node.js with Express

2. Unsplash API

3. CORS and dotenv for environment variable management

**Deployed Version**
You can access the backend API here: [Eazi Tour Backend](https://eazi-tour-backend.vercel.app/)
