# Functional Requirements

## 1. User Registration and Authentication

The application will require users to register and authenticate themselves.

There will be two main user roles:

- **Administrator:** The manager or shift supervisor of a hospitality business.
- **Employee:** A regular employee or student worker.

The administrator will register an account and enter the relevant information about their business. They will then configure a weekly schedule template adapted to the business's operating hours and staffing requirements.

Each business will receive a unique QR code associated with its account. Employees will first register as regular users. After scanning the QR code and receiving approval from the administrator, they will be added to the business's employee list.

The administrator will be able to remove employees from the business at any time.

## 2. Shift Planning and Weekly Schedule Management

Shifty will provide an interactive calendar synchronized across all users belonging to the same business.

The administrator will be able to define the required number of employees and working hours for each day and shift in advance.

Employees will be able to enter their availability directly into the calendar. The application will then display, in real time, which employees have signed up for each shift.

Additionally, the administrator will be able to see whether any employee has requested a day off or reported sick leave.

Before the schedule is finalized, it will require administrator approval.

Since not all shifts are expected to be filled voluntarily every week, the administrator will also be able to manually assign employees and make changes to the schedule.

Once the administrator or shift manager is satisfied with the schedule, they will be able to confirm it with a single action. All employees will then receive a notification informing them that the finalized schedule is available.

## 3. Shift Exchange Requests

Employees will be able to request shift exchanges with their colleagues.

If an employee is unable to work a shift they have already been assigned, they will be able to submit a request asking another employee to take over their shift.

Other employees will be able to accept or decline the request. If someone accepts, the administrator will be notified about the successful exchange.

If no employee is willing to take over the shift, the responsibility for finding a replacement will remain with the shift manager.

In such cases, the administrator will be able to manually update the schedule. The replacement employee will receive a notification about their newly assigned shift.

## 4. Working Hours Tracking and Reports

Shifty will allow employees to record the beginning and end of their working shifts using dedicated clock-in and clock-out buttons.

The application will automatically record the hours worked by each employee.

Employees will be able to review their working hours, including historical records. Their total working hours will be calculated automatically for each month.

Administrators will have access to the working hours of all employees and will be able to manually correct records if an employee forgets to clock in or clock out.

The application will also provide PDF export functionality. Administrators will be able to generate:

- An individual working hours report for a selected employee.
- A summary report containing the working hours of all employees for a selected month.

These records can be used for internal monitoring and as a basis for payroll calculations.

## 5. Shared Notice Board and Announcements

Depending on the available development time, we may also implement additional features.

One of these features will be a shared notice board where administrators can publish announcements and important information for all employees.

For example, administrators will be able to quickly inform employees about:

- Temporary business closures.
- Collective holidays or days off.
- Important announcements.
- Tasks and responsibilities that employees need to complete.

The notice board will provide a predefined template consisting of a title and message content, while the actual information will be entered by the responsible person.

## 6. Employee Roles and Work Categories

Another potential additional feature will be the ability to define more detailed employee roles and categories.

An employee's role could be extended to include their specific work position, such as:

- Bar staff.
- Floor staff / waitstaff.
- Support staff.

Employees could also be categorized according to their employment status, for example:

- Regular employees.
- Student workers.

This additional classification would allow administrators to define more specific staffing requirements when planning shifts.

For example, a shift could require one regular employee and one student worker. Alternatively, certain shifts could be restricted to regular employees only.

The application could also support defining the required monthly working hours for different employment categories. Regular employees may have a minimum monthly working hour requirement (e.g. 140–160 hours), whereas student workers would not be subject to the same requirements.

These categories and requirements would help administrators create more balanced schedules that comply with the staffing needs of their business.

## 7. Project Scope and Additional Features

The features described above represent the planned functionality of Shifty.

The implementation of additional features will depend on the available development time and the overall progress of the project.
