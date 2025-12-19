# daily_update.p
import datetime
import random

print("Daily GitHub activity - Day 36")

today = datetime.date.today()

# Generate random tasks and mark them as done or pending
tasks = ["Refactor code", "Write tests", "Fix bug", "Update docs", "Review PR"]
status = {task: random.choice(["Done", "Pending"]) for task in tasks}

completed = [t for t, s in status.items() if s == "Done"]

print(f"Today's date: {today}")
print("Task status:")
for task, s in status.items():
    print(f"- {task}: {s}")

print("Completed tasks count:", len(completed))
