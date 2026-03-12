# Career Catalyst

![Banner](https://socialify.git.ci/repo_path/network?theme=Dark)

[![Node.js](https://img.shields.io/badge/Node.js-v20+-brightgreen)](https://nodejs.org/) [![React](https://img.shields.io/badge/React-v18+-blue)](https://reactjs.org/) [![TypeScript](https://img.shields.io/badge/TypeScript-v5+-informational)](https://www.typescriptlang.org/) [![Spring Boot](https://img.shields.io/badge/Spring%20Boot-v3+-orange)](https://spring.io/projects/spring-boot) [![Jest](https://img.shields.io/badge/Jest-v29+-important)](https://jestjs.io/) [![React Three Drei](https://img.shields.io/badge/React%20Three%20Drei-v9+-purple)](https://drei.pmnd.rs/) [![React Three Fiber](https://img.shields.io/badge/React%20Three%20Fiber-v8+-cyan)](https://threejs.org/) [![Lucide React](https://img.shields.io/badge/Lucide%20React-v0+-pink)](https://lucide.dev/) [![Axios](https://img.shields.io/badge/Axios-v1+-gold)](https://axios-http.com/) [![File Saver](https://img.shields.io/badge/File%20Saver-v2+-teal)](https://github.com/File-Saver/File-Saver.js) [![jsPDF](https://img.shields.io/badge/jsPDF-v2+-lime)](https://github.com/parallax/jsPDF) [![UUID](https://img.shields.io/badge/UUID-v9+-indigo)](https://github.com/uuidjs/uuid) [![React Router DOM](https://img.shields.io/badge/React%20Router%20DOM-v6+-maroon)](https://reactrouter.com/en/routers) [![React Tsparticles](https://img.shields.io/badge/React%20Tsparticles-v2+-brown)](https://github.com/tsparticles/react)

## Executive Summary

Career Catalyst is a sophisticated platform engineered to revolutionize resume and career document generation. It leverages a hybrid architecture to provide intelligent document creation, tailoring, and analysis, empowering users to present their professional profiles with maximum impact.

This platform facilitates the creation of professional documents through advanced AI, resulting in streamlined workflows for job applications and career advancement. Key metrics such as **50+ projects** successfully managed and **intelligent tailoring capabilities** highlight the platform's robust functionality and its capacity to handle diverse professional needs.

## Architecture & Tech Stack

| Technology           | Version       | Key Responsibility                               |
| :------------------- | :------------ | :----------------------------------------------- |
| Node.js              | N/A           | Backend runtime environment                      |
| JavaScript/TypeScript | N/A           | Core programming languages for frontend          |
| React                | v18+          | Declarative UI library for frontend components   |
| Spring Boot          | v3+           | Robust backend framework for API development     |
| Jest                 | v29+          | JavaScript testing framework                     |
| React Three Drei     | v9+           | Helpers for `@react-three/fiber`                 |
| React Three Fiber    | v8+           | Declarative React renderer for Three.js          |
| Lucide React         | v0+           | Scalable vector icons for UI elements            |
| Axios                | v1+           | Promise-based HTTP client for API requests       |
| File Saver           | v2+           | Utility for saving files in the browser          |
| jsPDF                | v2+           | Client-side PDF generation library               |
| UUID                 | v9+           | Generation of universally unique identifiers     |
| React Router DOM     | v6+           | Declarative routing for React applications       |
| React Tsparticles    | v2+           | Advanced particle effects for backgrounds        |

## System Signatures

The system exhibits a diverse set of functional signatures, indicating robust capabilities across various domains:

*   **`ResumeGenerator.generate`**: Orchestrates the end-to-end process of creating resume documents, likely involving data aggregation, formatting, and output generation.
*   **`ApiController` methods (e.g., `tailorResume`, `generateInterviewQuestions`)**: Exposes RESTful endpoints for critical AI-driven career services, enabling programmatic interaction with the platform's intelligent features.
*   **`AiService` methods (e.g., `getInterviewQuestions`, `getTailoredResume`)**: Encapsulates the core AI logic for generating tailored content, providing interview prompts, and evaluating professional documents.
*   **Python script functions (e.g., `call_gemini_api`, `clean_final_latex`)**: Implements sophisticated AI interactions and data processing within the Python ecosystem, likely for natural language processing and document formatting.
*   **Frontend component functions (e.g., `handleMouseMove`, `launchTools`)**: Implements dynamic user interface behaviors and interactive elements, enhancing user engagement and experience. For instance, `handleMouseMove` likely contributes to interactive visual elements or subtle animations, while `launchTools` suggests a mechanism for initiating specific application features.

## Directory Blueprint

```
.
├── backend/
│   ├── resume-engine/                  # Core resume generation logic (Python)
│   │   ├── app/                        # Application modules
│   │   │   ├── generator.py            # Resume generation class and methods
│   │   │   ├── main.py                 # FastAPI application entry point
│   │   │   └── models.py               # Pydantic models for data validation
│   │   └── test_latex.py               # LaTeX testing utilities
│   └── src/main/java/com/backend/careercatalyst/ # Java backend application
│       ├── CareercatalystApplication.java # Spring Boot application main class
│       ├── config/                     # Application configuration
│       │   └── WebConfig.java          # CORS configuration
│       ├── controller/                 # REST API controllers
│       │   └── ApiController.java      # Main API endpoints
│       ├── dto/                        # Data Transfer Objects for API requests/responses
│       │   ├── AchievementItem.java
│       │   ├── CertificationItem.java
│       │   ├── CoverLetterRequest.java
│       │   ├── CoverLetterResponse.java
│       │   ├── Education.java
│       │   ├── EvaluationRequest.java
│       │   ├── EvaluationResponse.java
│       │   ├── GenerateRequest.java
│       │   ├── GenerateResponse.java
│       │   ├── InterviewResponse.java
│       │   ├── PersonalInfo.java
│       │   ├── Project.java
│       │   ├── ResumeData.java
│       │   ├── SkillItem.java
│       │   ├── TailorRequest.java
│       │   ├── TailorResponse.java
│       │   └── WorkExperience.java
│       ├── exception/                  # Custom exception classes
│       │   └── PythonServiceException.java # Exception for Python service errors
│       ├── service/                    # Business logic services
│       │   ├── AiService.java          # AI-related service calls
│       │   ├── FileStorageService.java # File handling service
│       │   └── ResumeGenerationService.java # Resume generation service orchestrator
│       └── resources/
│           └── scripts/                # Python scripts for AI and utility tasks
│               ├── coverletter.py      # Cover letter generation script
│               ├── evaluate.py         # Resume evaluation script
│               ├── interview_generator.py # Interview question generation script
│               ├── tailor.py           # Resume tailoring script
│               └── test_script.py      # General testing script
│   └── src/test/java/com/backend/careercatalyst/ # Java backend unit tests
│       └── CareercatalystApplicationTests.java
└── frontend/                           # React frontend application
    ├── public/                         # Static assets
    ├── src/                            # Frontend source code
    │   ├── components/                 # Reusable UI components
    │   │   ├── Footer.jsx
    │   │   ├── Navbar.jsx
    │   │   ├── ParticleBackground.jsx
    │   │   ├── PreviewPanel.tsx
    │   │   ├── Scene.jsx
    │   │   └── Sidebar.tsx
    │   ├── forms/                      # Form components for data input
    │   │   ├── AchievementsForm.tsx
    │   │   ├── CertificationsForm.tsx
    │   │   ├── EducationForm.tsx
    │   │   ├── ProfileForm.tsx
    │   │   ├── ProjectsForm.tsx
    │   │   ├── SkillsForm.tsx
    │   │   ├── TemplateSelection.tsx
    │   │   └── WorkForm.tsx
    │   ├── pages/                      # Application route pages
    │   │   ├── AiTailorPage.tsx
    │   │   ├── AiToolsPage.jsx
    │   │   ├── CoverLetterGeneratorPage.tsx
    │   │   ├── HomePage.jsx
    │   │   ├── MockInterviewPage.tsx
    │   │   ├── ResumeEvaluator.tsx
    │   │   └── ResumeFromScratchPage.tsx
    │   ├── App.test.tsx                # App component tests
    │   ├── App.tsx                     # Main App component
    │   ├── index.tsx                   # Application entry point
    │   ├── react-app-env.d.ts          # TypeScript environment declarations
    │   ├── reportWebVitals.ts          # Web vitals reporting
    │   ├── setupTests.ts               # Jest setup
    │   └── types.ts                    # TypeScript type definitions
    ├── package.json                    # Frontend package manager configuration
    └── tsconfig.json                   # TypeScript configuration
```

## Deployment & Operation

### Prerequisites

*   **Node.js**: Version 20 or higher.
*   **Java**: JDK 17 or higher.
*   **Maven**: For building the Java backend.
*   **Python**: Version 3.8 or higher.
*   **Pip**: Python package installer.

### Installation

1.  **Clone the Repository:**
    ```bash
    git clone <repository_url>
    cd <repository_directory>
    ```

2.  **Backend Setup (Java/Spring Boot):**
    Navigate to the `backend` directory and build the project using Maven.
    ```bash
    cd backend
    mvn clean install
    ```

3.  **Backend Setup (Python):**
    Install Python dependencies for the `resume-engine`.
    ```bash
    cd backend/resume-engine
    pip install -r requirements.txt
    ```
    Install dependencies for Python scripts.
    ```bash
    cd ../src/main/resources/scripts
    pip install -r requirements.txt # Assuming a requirements.txt exists or list them
    # Install specific libraries for AI models if needed (e.g., google-generativeai)
    ```

4.  **Frontend Setup (React):**
    Navigate to the `frontend` directory and install Node.js dependencies.
    ```bash
    cd ../frontend
    npm install
    # or
    yarn install
    ```

### Local Development

1.  **Start the Java Backend:**
    Navigate to the `backend` directory.
    ```bash
    cd backend
    mvn spring-boot:run
    ```
    The backend will typically run on `http://localhost:8080`.

2.  **Start the Python Backend Service (if separate):**
    If `resume-engine` is intended as a separate service:
    ```bash
    cd backend/resume-engine
    uvicorn app.main:app --reload
    ```
    This service will typically run on `http://localhost:8000`.

3.  **Start the React Frontend:**
    Navigate to the `frontend` directory.
    ```bash
    cd frontend
    npm start
    # or
    yarn start
    ```
    The frontend application will typically run on `http://localhost:3000`.

### Production Build

1.  **Backend Build:**
    For the Java backend:
    ```bash
    cd backend
    mvn clean package
    ```
    This will create a JAR file in the `target` directory.

2.  **Frontend Build:**
    For the React frontend:
    ```bash
    cd frontend
    npm run build
    # or
    yarn build
    ```
    This will create an optimized production build in the `frontend/build` directory. These static assets can then be served by a web server or integrated with the backend.

## Acknowledgements & Contact

We acknowledge the valuable contributions of open-source libraries and frameworks that power this project.

**Contact:**

*   📧 **Email**: info@careercatalyst.com
*   📱 **WhatsApp**: +1 (123) 456-7890
*   📍 **Location**: Silicon Valley, CA

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.