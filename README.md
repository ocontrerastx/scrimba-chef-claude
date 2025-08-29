# Chef Claude Recipe Suggestion App

This project involved creating a recipe suggestion application that integrates with the Claude AI API based on the design provided in the following Figma file:
[Figma Design](https://www.figma.com/design/73iyU720zWmrWgJsok5tYE/Chef-Claude?node-id=1-972&t=rZEfcwmHKnUjaKr1-1)

Users can input ingredients they have available at home and receive personalized recipe suggestions from Claude AI. The primary goal was to build an interactive React application that demonstrates modern React patterns, state management, and API integration while providing practical value for meal planning.

## Setup Requirements

To run this project, you'll need to:

1. Create a Claude API key from Anthropic
2. Add your API key to a `.env` file in the project root:
   ```
   VITE_CLAUDE_API_KEY=your_api_key_here
   ```

**Key Concepts Applied:**

- **Interactive React Development:** This project provided hands-on experience building a fully interactive React application from the ground up. The focus was on creating a responsive user interface that dynamically updates based on user input and API responses.

- **Event Handling in React:** Implemented comprehensive event listener management using React's synthetic event system. This included handling form submissions, input changes, and button clicks while maintaining proper event delegation and preventing default browser behaviors where necessary.

- **React State Management:** Gained deep understanding of React's state system and its role in component lifecycle management:

  - Used `useState` hooks to manage ingredient lists, recipe data, and loading states
  - Learned how state changes trigger re-renders and update the user interface
  - Implemented state persistence patterns to maintain data across component updates

- **Conditional Rendering:** Implemented dynamic UI updates based on application state, including showing/hiding recipe suggestions, displaying loading indicators, and handling empty states when no ingredients are provided or when API calls are in progress.

- **Form Data Handling:** Mastered React form management using the FormData API to capture and process user input. This involved extracting ingredient data from form submissions and properly formatting it for API requests while maintaining form validation and user feedback.

- **Component Architecture & State Lifting:** Developed strategic thinking around state management hierarchy in React applications:
  - Identified optimal locations for state instantiation to ensure data accessibility across components
  - Implemented state lifting patterns to share data between sibling components
  - Learned about the limitations of direct child-to-child communication and solved this through proper parent component state management

**Learning Journey Highlights:**

The most significant learning experience was understanding React's unidirectional data flow and how it differs from traditional DOM manipulation. Initially, the challenge was grasping why state couldn't be directly shared between child components and how lifting state to a common parent component solves this architectural challenge. This led to a deeper appreciation of React's component hierarchy and the importance of planning component structure around data flow requirements.

Another key insight came from working with asynchronous operations when integrating the Claude API. Managing loading states and ensuring the user interface remains responsive during network requests required careful consideration of async/await patterns. This experience highlighted the importance of user experience design in applications that depend on external services.

The project also provided valuable experience with modern JavaScript ES6+ features in the context of React development, including destructuring assignment for props and state, arrow functions for event handlers, and template literals for dynamic string generation when formatting ingredients for the API request.

Working with the Claude API specifically taught important lessons about prompt engineering and how to structure ingredient lists in a way that produces the most helpful and relevant recipe suggestions. This involved experimenting with different input formats and learning how to provide enough context to the AI while keeping requests concise and focused.
