# Johan-fako-27.10.2010
Software J.F 2010
class TaskManager:
    def __init__(self):
        self.tasks = []

    def add_task(self, task):
        self.tasks.append(task)
        print(f"Úloha '{task}' bola pridaná.")

    def list_tasks(self):
        print("Zoznam úloh:")
        for task in self.tasks:
            print(f"- {task}")

    def remove_task(self, task):
        if task in self.tasks:
            self.tasks.remove(task)
            print(f"Úloha '{task}' bola odstránená.")
        else:
            print(f"Úloha '{task}' sa nenašla.")

# Príklad použitia
manager = TaskManager()
manager.add_task("Nakúpiť potraviny")
manager.add_task("Zavolať doktorovi")
manager.list_tasks()
manager.remove_task("Zavolať doktorovi")
manager.list_tasks()
