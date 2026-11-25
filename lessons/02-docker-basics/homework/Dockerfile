# (בוחר אימג בסיס בגרסה מוקטנת)
FROM python:3.11-slim

# (יוצר את תקיית העבודה בתוך הקונטיינר)
WORKDIR /app

# (מעתיקים קודם רק את רשימת התלויות, כדי ששינוי בקוד לא יפעיל את ההתקנה מחדש)
COPY requirements.txt .

# (התקנת רשימת התלויות)
RUN pip install --no-cache-dir --trusted-host pypi.org --trusted-host files.pythonhosted.org -r requirements.txt

# הקוד בעצמו
COPY app.py .

# (מתעד שהשרת מאזין על פורט 8000 (זה לא פותח את הפורט.
EXPOSE 8000

# (מריץ את השרת כשה-container עולה)
CMD ["python", "app.py"]
