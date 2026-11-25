1. docker build -tag greeter:v1 lessons/02-docker-basics/homework/greeter
2. docker run -d -p 9000:8000 --name greeter greeeter:v1
3. GREETING=Shalom
4. {"message":"Shalom, Rivka!"}
5.FROM, WORKDIR, COPY requirements.txt ו-RUN pip install יסומנו CACHED, כי הם לא השתנו. COPY app.py ירוץ מחדש כי הקובץ השתנה, ואחרי שכבה שהשתנתה כל השכבות שאחריה נבנות מחדש. בגלל זה מעתיקים את התלויות לפני הקוד: שינוי בקוד לא מפעיל שוב את ההתקנה.
