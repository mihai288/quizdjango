# Quiz Web App

Aplicatie web făcută în Django care te ajută să creezi și să distribui quiz-uri online.

## Ce poți face cu ea?

- **Creezi quiz-uri** cu întrebări și răspunsuri (poți alege dacă sunt multiple choice sau nu)
- **Distribui link-uri publice** către quiz-urile tale - oricine poate accesa și răspunde
- **Vezi rezultatele** oamenilor care au răspuns la quiz-urile tale
- **Închizi quiz-urile** când vrei să nu mai primești răspunsuri
- **Primești explicații AI** pentru răspunsurile greșite (folosind OpenAI GPT-4o-mini)


## Cum o folosești?

1. **Înregistrează-te** - creează un cont nou din pagina de register
2. **Loghează-te** cu username-ul și parola
3. **Creează un quiz** - apasă pe "Create +" și adaugă întrebări cu răspunsuri
4. **Distribuie link-ul** - după ce creezi quiz-ul, primești un link pe care îl poți trimite oricui
5. **Vezi rezultatele** - în dashboard-ul tău vei vedea toate răspunsurile primite

## Structura proiectului

- `quizappDjango/` - folder-ul principal cu setările Django
  - `models.py` - modelele de date (User, Quiz, Question, Answer, QuizResult)
  - `views.py` - logica aplicației (autentificare, creare quiz, jucare, rezultate)
  - `urls.py` - rutele aplicației
  - `settings.py` - configurația Django
- `templates/` - template-urile HTML
- `static/` - fișierele CSS și JavaScript
- `db.sqlite3` - baza de date (se creează automat)

## Funcționalități tehnice

- **Autentificare** - sistem de login/register cu Django's built-in auth
- **Link-uri publice** - fiecare quiz are un UUID unic pentru accesare fără autentificare
- **Status quiz** - poți închide quiz-urile să nu mai primească răspunsuri
- **Tracking răspunsuri** - sistemul ține minte cine a răspuns deja la un quiz
- **Integrare OpenAI** - explică automat de ce răspunsurile greșite sunt greșite



---

