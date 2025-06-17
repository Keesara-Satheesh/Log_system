# Log Management System
**Overview**
The Log Management System is a Python application that organizes and manages log entries. It provides functionality for parsing logs, grouping them by user, counting log levels, filtering logs by keywords, and retrieving recent logs while adhering to a specified capacity. This project is ideal for tracking and analyzing log entries in various applications.

**Features**
* Add logs: Parses and stores logs from a specified format.
* Grouped logs per user: Provides access to log entries for specific users.
* Log level frequency count: Keeps track of how many logs exist for each log level (e.g., INFO, ERROR, WARN).
* Keyword filtering: Retrieves all log entries that contain a specified keyword (case-insensitive).
* Recent logs: Maintains a list of recent logs up to a defined capacity.

**Requirements**
Python 3.x
collections and re (included in the Python standard library)

**Example log data:**
python
logs_data = [
    "[2025-06-16T10:00:00] INFO user1: Started process",
    "[2025-06-16T10:00:01] ERROR user1: Failed to connect",
    "[2025-06-16T10:00:02] INFO user2: Login successful",
    "[2025-06-16T10:00:03] WARN user3: Low memory",
    "[2025-06-16T10:00:04] ERROR user2: Timeout occurred",
    "[2025-06-16T10:00:05] INFO user1: Retrying connection"
]

**Code Overview**
* The LogSystem class contains methods to manage and manipulate logs:
* add_log(self, line: str): Adds a log entry to the system.
* get_user_logs(self, user_id: str): Fetches logs for a specified user.
* count_levels(self): Returns the frequency of each log level.
* filter_logs(self, keyword: str): Retrieves logs containing the specified keyword.
* get_recent_logs(self): Returns the most recent logs according to the defined capacity.

**Example Output**
Running the system will display details such as added logs, user-specific logs, log level frequencies, filtered logs, and recent logs.


