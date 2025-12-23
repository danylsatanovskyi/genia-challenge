Personal AI Assistant (CLI)

A command-line Personal AI Assistant written in Python 3.12 that uses the OpenRouter API
to provide multiple interactive AI-powered capabilities through a simple menu-driven interface.

------------------------------------------------------------
FEATURES
------------------------------------------------------------

- Code Explainer
- Language Translator
- Recipe Suggester
- Supportive Coach
- Mock Interviewer
- Debate Partner (Devil’s Advocate)

All features run locally via the command line.

------------------------------------------------------------
TECHNICAL REQUIREMENTS
------------------------------------------------------------

- Python 3.12 (latest stable recommended)
- OpenRouter API key
- Internet connection

------------------------------------------------------------
INSTALLATION
------------------------------------------------------------

git clone https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
cd YOUR_REPO_NAME
python -m venv .venv
source .venv/bin/activate        (macOS / Linux)
.venv\Scripts\activate           (Windows)
pip install -r requirements.txt

------------------------------------------------------------
ENVIRONMENT SETUP
------------------------------------------------------------

cp .env.example .env

Edit .env:

OPENROUTER_API_KEY=your_real_api_key_here

WARNING:
Never commit your .env file.

------------------------------------------------------------
RUNNING THE APPLICATION
------------------------------------------------------------

python assistant.py

------------------------------------------------------------
EXAMPLE USAGE (FEATURE CHATS)
------------------------------------------------------------

------------------------------------------------------------
1) CODE EXPLAINER
------------------------------------------------------------

User:
Choose an option: 1
Paste code to explain.
Enter snippet.

for i in range(5):
    print(i)
DONE

Assistant:
This code loops from 0 to 4 and prints each number on a new line.
The range(5) function generates five values starting at 0.

------------------------------------------------------------
2) LANGUAGE TRANSLATOR
------------------------------------------------------------

User:
Choose an option: 2
Language Translator
Type DONE to finish entering text.
Type QUIT on a new line to exit.

Source language (e.g., English, French, Spanish) or 'auto': english
Target language (e.g., English, French, Spanish): french

Enter the text you want to translate.
i love you
DONE

Assistant:
------------------------------------------------------------
TRANSLATION
------------------------------------------------------------
je t’aime
------------------------------------------------------------

User:
Source language (e.g., English, French, Spanish) or 'auto': spanish
Target language (e.g., English, French, Spanish): english

Enter the text you want to translate.
hola como estas
DONE

Assistant:
------------------------------------------------------------
TRANSLATION
------------------------------------------------------------
Hello, how are you?
------------------------------------------------------------

------------------------------------------------------------
3) RECIPE SUGGESTER
------------------------------------------------------------

Recipe Suggester
Enter ingredients (one per line). Type DONE to finish a set.
Type QUIT on a new line to exit.

Enter ingredients for this request:
fish and chips
DONE

Cuisine preference (optional, e.g., Italian, Asian, none): asian
Max cooking time (optional, e.g., 15 min, 30 min, none): 30 min
Dietary constraints (optional, e.g., vegetarian, halal, none): vegetarian

------------------------------------------------------------
RECIPE IDEAS
------------------------------------------------------------

1) Korean Gochujang Tofu “Fish” & Chips Bowl
Why it fits:
Asian flavors, vegetarian, fast to prepare.

Ingredients used:
chips (fries)

Steps:
1. Pat tofu dry and slice into slabs.
2. Pan-fry tofu until golden.
3. Mix sauce ingredients.
4. Toss chips with sauce.
5. Brush tofu with sauce.
6. Serve hot.

------------------------------------------------------------
4) SUPPORTIVE COACH (NON-CLINICAL)
------------------------------------------------------------

Supportive Coach
Talk about what's on your mind.
Type DONE to send a message.
Type QUIT to end the session.

User:
ive been overwhelmed with school
DONE

Assistant:
That sounds really heavy. When school starts to feel like it’s piling up,
it can be exhausting and hard to know where to begin.

Suggestions:
- Brain dump tasks
- Pick one small next step
- Short reset breaks
- Ask for help if possible

------------------------------------------------------------
5) MOCK INTERVIEWER
------------------------------------------------------------

Mock Interviewer
Answer the questions.
Type DONE to submit each answer.
Type QUIT to end the interview.

Role you're interviewing for: swe
Focus: technical

Assistant:
You’re given an array of integers nums and an integer k.
Return the k most frequent elements.

User:
i dont know...
DONE

Assistant:
You were honest about uncertainty, which is good.
Let’s break the problem down step by step.

------------------------------------------------------------
6) DEBATE PARTNER (DEVIL’S ADVOCATE)
------------------------------------------------------------

Debate Partner
State an opinion or claim.
Type DONE to submit.
Type QUIT to end the debate.

User:
messi is the best soccer player in the world
DONE

Assistant:
That depends on what you mean by “best.”
Are you referring to peak ability, current performance,
or historical greatness?

User:
yes most ballon dors
DONE

Assistant:
Ballon d’Ors support historical greatness,
but they don’t alone prove current superiority.

------------------------------------------------------------
END
------------------------------------------------------------
