## Flask Application Design for Quiz Platform

### HTML Files

- `index.html`: This is the home page of the platform. It should have a navigation bar with links to the quizzes, the grading section, and the admin panel (for adding and managing quizzes and questions). The home page should also provide a brief overview of the platform and its functionality.

- `quiz.html`: This HTML file will display the actual quiz. It should have a header with the quiz title, a list of questions, and a submit button to submit the quiz for grading. The questions should be displayed in a clear and structured manner, with each question having a unique identifier associated with it.

- `grade.html`: This HTML file will display the graded quiz. It should have a header with the quiz title, a list of questions, and the corresponding grades for each question. The questions should be displayed in the same order as they appeared in the quiz, and the grades should be clearly indicated next to each question.

- `admin.html`: This HTML file will provide an interface for managing quizzes and questions. It should have a navigation bar with options to add a new quiz, add questions to an existing quiz, and edit or delete quizzes and questions. The admin interface should also provide a way to view the results of graded quizzes.

### Routes

- `/`: This route will handle the home page of the platform. It will display the `index.html` file.

- `/quizzes`: This route will display a list of available quizzes. It can be used to navigate to the individual quiz pages.

- `/quiz/<quiz_id>`: This route will handle the individual quiz page. It will display the `quiz.html` file and populate it with the questions for the selected quiz.

- `/grade/<quiz_id>`: This route will handle the grading of a quiz. It will receive the submitted answers and calculate the grades for each question. The graded quiz will then be displayed in the `grade.html` file.

- `/admin`: This route will handle the admin interface of the platform. It will display the `admin.html` file and allow the user to manage quizzes and questions.