# Phone Book Management System (Java Swing + JDBC + SQLite)

## Requirements
- JDK 17 or later
- Maven 3.8+

## Run
Open a terminal in this project folder and run:

```bash
mvn clean package
java -jar target/phone-book-app-1.0.0.jar
```

The SQLite database `phonebook.db` is created automatically in the folder from which the application is launched. Default groups Family, Friends and Work are added on first launch.

## Features
- Add, edit, delete and list personal/business contacts
- Search contacts by name or phone number
- Create and delete groups; assign contacts to groups
- Manually record incoming, outgoing and missed calls
- Export contacts, groups and call logs to CSV files
- Duplicate phone numbers are rejected with `DuplicateContactException`

## Syllabus mapping
- Classes/objects: `Contact`, `PersonalContact`, `BusinessContact`, `Group`, `CallLog`
- Inheritance: `PersonalContact` and `BusinessContact` extend `Contact`
- Interface: `Searchable`
- Exception handling: `DuplicateContactException`
- String methods: `trim`, `toLowerCase`, `contains`, `isBlank`, `replace`
- File handling: `File`, `FileWriter`, `PrintWriter`
- JDBC: `Database`, `PreparedStatement`, `ResultSet`
- CRUD: `PhoneBookService`
- Swing: `JFrame`, `JTabbedPane`, `JTable`, `JTextField`, `JButton`, action events
- Layouts: `BorderLayout`, `FlowLayout`, `GridLayout`
- Database tables: `contacts`, `groups`, `call_log`

Note: This is a desktop phone-book app. Call records are entered manually; it does not place or detect real phone calls.
