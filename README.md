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
Credits & Acknowledgements
​Project Lead & Core Developer: Somchand Ratangwal
​Contributions: Streamlit dashboard development, exam seating allocation logic, room-capacity validation, rapid replanning, debugging, testing, and documentation.
​Technology Stack: Python, Streamlit, Pandas.
​Developed as a hackathon project to simplify examination seating management and support faster replanning when rooms or invigilators become unavailable.
​©️ 2026 Somchand Ratangwal