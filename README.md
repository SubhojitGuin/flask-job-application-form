## Job Application Form

The Job Application Form is a web application developed using Flask, SQLAlchemy, and Flask-Mail. It allows job applicants to fill out a form with their personal information and submit it. The submitted form data is stored in a SQLite database and an email notification is sent to the applicant with the submitted details.

### Features

- **Form Submission**: Users can fill out the job application form by providing their first name, last name, email, available start date, and current occupation.
- **Database Storage**: The submitted form data is stored in a SQLite database (`data.db`) using SQLAlchemy.
- **Email Notification**: After successful form submission, an email is sent to the applicant's provided email address using Flask-Mail.
- **Flash Messages**: Flash messages are used to display a success message to the applicant after form submission.
- **Responsive Design**: The form is designed using Bootstrap to ensure a responsive and user-friendly interface.

### Requirements

The application requires the following dependencies:

- blinker==1.6.2
- click==8.1.3
- colorama==0.4.6
- Flask==2.3.2
- Flask-Mail==0.9.1
- Flask-SQLAlchemy==3.0.5
- greenlet==2.0.2
- itsdangerous==2.1.2
- Jinja2==3.1.2
- MarkupSafe==2.1.3
- SQLAlchemy==2.0.17
- typing_extensions==4.7.0
- Werkzeug==2.3.6

Please refer to the [requirements.txt](requirements.txt) file for detailed version information.

### How to Run

To run the Job Application Form:

1. Make sure you have the required dependencies installed in your Python environment.
2. Execute the `app.py` script using Python.
3. The application will start running locally.
4. Open a web browser and go to `http://localhost:5001` to access the form.
5. Fill out the form fields with the required information.
6. **Note: Replace the `MAIL_USERNAME` and `MAIL_PASSWORD` in `app.py` with your own email address and password to enable email notifications.**
7. Click the "Submit" button to submit the form.
8. If the form submission is successful, a success message will be displayed, and an email notification will be sent to the provided email address.

### Database

The submitted form data is stored in a SQLite database named `data.db`. The database file will be created automatically when the application is run for the first time. The `Form` model class in `app.py` defines the table structure and columns for storing the form data.

### Templates

The application uses the `index.html` template file to render the job application form. The template file is located in the `templates` directory. It is designed using HTML and Bootstrap to provide an intuitive and responsive form interface.

### License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

### Acknowledgements

We would like to acknowledge the developers and contributors of the open-source libraries used in this project. Their contributions and dedication have greatly facilitated the development of this Job Application Form. We express our gratitude to the following projects:

- [Flask](https://pypi.org/project/Flask/)
- [SQLAlchemy](https://pypi.org/project/SQLAlchemy/)
- [Flask-Mail](https://pypi.org/project/Flask-Mail/)

Their efforts have played a vital role in making this project possible.