# SeatPlan AI — Clean Starter

## Run on macOS
```bash
cd ~/Downloads/ExamSeatAI_Clean
python3 -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
python -m streamlit run app.py
```

## Input CSV columns
- Registrations: `student_id, exam_id, start_time, end_time`
- Rooms: `room_id, rows, cols`
- Invigilators: `invigilator_id`

Times should look like `2026-10-10 09:00`.

## Notes
This is a hackathon prototype. It validates overlapping exams and room capacity, enforces no orthogonally adjacent seats with the same exam ID, supports unavailable room/invigilator inputs, and exports assignments and roster. The seating solver has a search-node limit; for large or highly constrained sessions it may report that it could not find a layout. Invigilator assignment is a simple prototype policy, not a production rostering system.
