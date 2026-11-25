# (הערה: מה עושה השורה הזו?)
FROM python:___-slim

# (הערה)
WORKDIR /app

# (הערה: למה מעתיקים קודם רק את הקובץ הזה?)
COPY ___ .

# (הערה)
RUN pip install --no-cache-dir --trusted-host pypi.org --trusted-host files.pythonhosted.org -r requirements.txt

# (הערה)
COPY app.py .

# (הערה)
EXPOSE ___

# (הערה: מה רץ כשה-container עולה?)
CMD ["python", "___"]
