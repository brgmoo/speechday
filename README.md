# SpeechDay

This project can be used to easily and effectively hold a speechday (a parent-teacher-meeting) in your school.
The administrator can import data for teachers and students and create a speechday-event.
The newsletter filled with the needed access data so that parents can log in and book their desired time slots for the teachers they want to meet can then be created automatically. 

## Installation

You can create the needed database with the SQL script provided in the setup folder.
Furthermore you have to enter your database credentials in the settings.ini file contained in code/dao.
If you want to quickly try out the tool there is also a SQL script provided in the setup folder which puts some dummy test data in your newly created database. 

Be aware that the UI is in german.

## Usage

As an administrator:

1. Import teachers via a CSV file.
2. Import student data via a CSV file.
3. Upload a newsletter template in ODT format.
4. Create a speechday-event.
5. Create the newsletter and distribute it among the students / parents.

As a teacher (optional):

1. Set the time range you are present.

As a student / parent:

1. Log in with the credentials provided on the newsletter.
2. Book the desired slots for the desired teacher.
3. Print your time-table.

## ToDo
- [ ] Global: admin can be a teacher (add room)
- [x] Global: print timetable isn't styled
- [ ] Global: export timetable as pdf
- [ ] Global: add config.php for some variable text (e.g. "Eltern Sprechtags Verwaltung")
- [ ] Global: add slots to added teacher, when event is active
- [ ] Global: add eventId to room db for handle different events
- [ ] Global: deleting slot needs confirmation
- [ ] Global: update bootstrap and the libs
- [ ] Admin: room configuration (add, rename, delete, (un)set to teacher)
- [ ] Admin: unset rooms from all teacher (for new event)
- [x] Admin: import rooms
- [ ] Admin: modify action_csvPreview for room import
- [ ] Admin: use datetimepicker for bookingDate
- [ ] Admin: detailed error msg
- [ ] Teacher: set user to slot (if a speech needs more time)?
- [ ] Teacher: deleting booked slot needs confirmation
- [x] Teacher: select room from a list of free rooms
- [ ] User: request double slot for intensive speech? (maybe before a pause?)
- [ ] User: possibilty to add a text to a booked slot
- [ ] User: show presence of all teachers on book.php (+only selected teachers)
