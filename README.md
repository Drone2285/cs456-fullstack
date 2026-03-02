# CS-465 Full Stack Development - Travlr Getaways

## Architecture
The Express HTML pages are server‑rendered with Handlebars, which is simple and good for static content. The client‑side JavaScript adds light interactivity to those pages. The Angular SPA is a richer admin interface with routing, services, and reusable components, which enables fast updates without full page reloads. The backend uses MongoDB because the data is document‑oriented, maps well to JSON, and supports flexible schemas for trips and related data as the app evolves.

## Functionality
JSON is a lightweight data format, while JavaScript is a full programming language. JSON acts as the data contract between the frontend and backend: the API returns JSON, and the SPA consumes it to render views and send updates. I refactored by moving API calls into a shared service and by breaking the UI into reusable components like trip cards and listings. Reusable components reduce duplication, make the UI consistent, and simplify maintenance and testing.

## Testing
I tested endpoints using GET, POST, PUT, and DELETE through the browser, dev tools network tab, and tools like Postman. Each endpoint has a clear purpose and URL, and the client should receive predictable status codes and JSON responses. Security adds complexity because protected routes require authentication, so tests need need more requirements. Logging in the console also helped a lot with testing when something was silently breaking, which was an issue I faced with my Angular version.

## Reflection
This course helped me build confidence with full-stack development, especially integrating an Angular SPA with an Express/MongoDB backend. I strengthened my skills in API design, component‑based UI development, and end‑to‑end testing.
