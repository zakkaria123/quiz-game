#Quiz game by zirabamuzaale zakaria about various tech personalities for fun
#using python programming language
#7th jan 2023

import random
my_quiz={'Which Programming lanaguage is best popular for Data Science and Machine Learnig':['Python','JavaScript','C#','Ruby on Rails'],
'Who created Python Programming Language':['Auto Van Rosum','TimeCook','Mark Zukerburg','Bill Gates'],
'Who Created Twitter':['Jack Dossy','Dew Houston','Steve Jobs','Elon Mask'],
'Which Year was Facebook officially Launced':['2004','1998','2001','1954'],
'Who is the current CEO of Tesla and SpaceX':['Elon Mask','Jeff Bezzos','Tim Cook','Satya Nadella'],
'Who is the current CEO of Google':['Sundar Pichai','Satya Nadella','Lisa Su','Tim cook'],
'Who is the current CEO of Advanced Micro Devices (AMD)':['Lisa Su','Machael Sayman','CS Dojo','Jonathan Ma'],
'What is the bigest tech valley in the world':['Silcon Valley','California Valley','San Francisco valley','None of the above'],}
import pygame
pygame.init()

def Quiz_game():
    from string import ascii_lowercase
    import random
    import winsound
    import time
    questions_=random.sample(my_quiz.items(),k=len(my_quiz))
    score=0
    print(f'## Welcome to this simple Personality quiz prepared Zirabamuzaale Zakaria,hope you enjoy it\n')
    for num,(question, answers) in enumerate(questions_,start=1):
        print(f'\nQuestion {num}:')
        print(f'{question} ?')
        correct_answer=answers[0]
        list_answers =dict(zip(ascii_lowercase,sorted(answers)))
        for label,answer in list_answers.items():
            print(f'{label}) {answer}')
        while(user_answer:=input('\nAnswer: ')) not in list_answers:
            print(f"Please user {','.join(list_answers)}")
        print('\n')
        user_answer=list_answers[user_answer]
        if user_answer==correct_answer:
            pygame.mixer.music.load('d:\\inspire\\pysounds\\interface-124464.mp3')
            pygame.mixer.music.play()
            time.sleep(1)
            print (f'Your answer {user_answer!r} is Correct')
            score+=5
        else:
            pygame.mixer.music.load('d:\\inspire\\pysounds\\buzzer-or-wrong-answer-20582.mp3')
            pygame.mixer.music.play()
            time.sleep(2)
            pygame.mixer.music.load('d:\\inspire\\pysounds\\and-the-correct-answer-is-39671.mp3')
            pygame.mixer.music.play()
            time.sleep(1)
            print(f'Your answer {user_answer!r}, is Wrong {correct_answer!r} is the Correct answer')

            time.sleep(2)
    value=score
    if value>=20:
        print(f'\nGreat!! Your score {value!r}/40 is above average kudos you passed the test')
    else:
        print(f'\nYour Score {value!r} is slightly below average ')


Quiz_game()
