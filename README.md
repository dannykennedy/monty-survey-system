# Monty Survey System

This is a survey system developed to gauge course effectiveness and engagement.

**External Python libraries used**

`flask`, `flask_login`, `flask_sqlalchemy`, `werkzeug.security`, `csv`

**Running the project**

To run the project from scratch (if there is no app.db database), run: `./setup.sh`

This will run 

`python3 db_create.py`

`python3 user_upload.py`

`python3 courses_upload.py`

`python3 run.py`

WARNING: This process can take ~3 minutes, depending on your computer

If the database has been created, run: `python3 run.py`

**Homepage** 

URL of home page: http://127.0.0.1:2001

**Tests**

To run the tests:

`python3 tests.py`

*All tests contained in tests.zip:*

class TestLogin(unittest.TestCase):

	def test_invalid_login(self):
	def test_student_login(self):
	def test_admin_login(self):
	def test_staff_login(self):
	
class TestSurveys(unittest.TestCase):

	def test_create_survey(self):
	def test_create_invalid_survey(self):
	def test_add_question_to_survey(self):
	def test_answer_question(self):
	def test_delete_survey(self):
	
class TestQuestions(unittest.TestCase):

	def test_create_invalid_question(self):
	def test_create_optional__MC_question(self):
	def test_create_mandatory__MC_question(self):
	def test_create_optional_open_question(self):
	def test_create_mandatory_open_question(self):
	def test_delete_question(self):
	
class TestUsers(unittest.TestCase):

	def test_create_invalid_user(self):
	def test_create_student_user(self):
	def test_create_staff_user(self):
	def test_create_admin_user(self):
	def test_student_enrol(self):
	def test_staff_for_course(self):
	def test_invalid_student_enrol(self):
	def test_invalid_staff_for_course(self):
	def test_nonstaff_nonstudent_for_courses(self):
	
class TestCourseOffering(unittest.TestCase):

	def test_create_invalid_course_offering(self):
	def test_create_course_offering(self):
	def test_course_enrolment_data(self):
