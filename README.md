### Hi there 👋 I'm Samuel Arjuna Queen Bernard, u can call me Jun.
### 💻  About Me 
  Exploring new technologies and developing software solutions and quick hacks.
  Studying Information System at TELKOM UNIVERSITY.
  Learning more about Fullstack Dev.
  Pursuing Coding as hobbies


🛠  Tech Stack

    - Fullstack Developer
    - Laravel
    - Docker
    - Postgre
    - XAMPP
    - DBeaver
    
I often use Gitlab for developer needs

import requests

def get_gitlab_stats(arjunaber):
    url = f"https://gitlab.com/api/v4/users/{arjunaber}/projects"
    response = requests.get(url)
    if response.status_code == 200:
        projects = response.json()
        # Proses data proyek untuk statistik
        return projects
    else:
        return None

username = "your_gitlab_username"
stats = get_gitlab_stats(username)
if stats:
    print(stats)
else:
    print("Failed to retrieve data")

